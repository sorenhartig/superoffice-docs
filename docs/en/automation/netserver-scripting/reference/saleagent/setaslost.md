---
uid: saleagent-setaslost
title: SaleAgent.SetAsLost event method
description: Scripting events called on the SetAsLost method on the SaleAgent service agent.
so.generated: true
keywords:
  - "netserver"
  - "scripting"
so.date: 11.29.2022
so.topic: reference
so.envir:
  - "onsite"
---
# SaleAgent.SetAsLost

Scripting events called on the <see cref='M:SuperOffice.CRM.Services.ISaleAgent.SetAsLost'>SetAsLost</see> method on the <see cref='ISaleAgent'>ISaleAgent</see>  service agent.

## BeforeSetAsLost
```cs
    static void BeforeSetAsLost(
       Int32[]  saleIds,
       ref object  eventState
      );
```
Executes before the service method is invoked.
It can store some state in the *eventState* parameter, that is passed to the **After** and **AfterAsync** methods in this service call.
Event state is not preserved between different service calls. It is set to null at the start of each service call.
## AfterSetAsLost
```cs
    static void AfterSetAsLost(
       Int32[]  saleIds,
       ref object  eventState
      );
```
Executes after the service method has been invoked. The service waits for this method to complete before returning the result to the caller.
This service call has no return value, so there is no **returnValue** parameter
Any state you set in the **Before** method is passed in through the *eventState* parameter.
## AfterSetAsLostAsync
```cs
    static void AfterSetAsLostAsync(
       Int32[]  saleIds,
       ref object  eventState
      );
```
Executes after the service method is invoked, without waiting for the call to return.
The service call is not blocked waiting for this method to complete.
Any state you set in the **Before** method is passed in through the *eventState* parameter.

