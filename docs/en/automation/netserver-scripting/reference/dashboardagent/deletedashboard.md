---
uid: dashboardagent-deletedashboard
title: DashboardAgent.DeleteDashboard event method
description: Scripting events called on the DeleteDashboard method on the DashboardAgent service agent.
so.generated: true
keywords:
  - "netserver"
  - "scripting"
so.date: 11.29.2022
so.topic: reference
so.envir:
  - "onsite"
---
# DashboardAgent.DeleteDashboard

Scripting events called on the <see cref='M:SuperOffice.CRM.Services.IDashboardAgent.DeleteDashboard'>DeleteDashboard</see> method on the <see cref='IDashboardAgent'>IDashboardAgent</see>  service agent.

## BeforeDeleteDashboard
```cs
    static void BeforeDeleteDashboard(
       Int32  dashboardId,
       ref object  eventState
      );
```
Executes before the service method is invoked.
It can store some state in the *eventState* parameter, that is passed to the **After** and **AfterAsync** methods in this service call.
Event state is not preserved between different service calls. It is set to null at the start of each service call.
## AfterDeleteDashboard
```cs
    static void AfterDeleteDashboard(
       Int32  dashboardId,
       ref object  eventState
      );
```
Executes after the service method has been invoked. The service waits for this method to complete before returning the result to the caller.
This service call has no return value, so there is no **returnValue** parameter
Any state you set in the **Before** method is passed in through the *eventState* parameter.
## AfterDeleteDashboardAsync
```cs
    static void AfterDeleteDashboardAsync(
       Int32  dashboardId,
       ref object  eventState
      );
```
Executes after the service method is invoked, without waiting for the call to return.
The service call is not blocked waiting for this method to complete.
Any state you set in the **Before** method is passed in through the *eventState* parameter.

