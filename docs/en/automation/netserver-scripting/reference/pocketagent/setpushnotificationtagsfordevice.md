---
uid: pocketagent-setpushnotificationtagsfordevice
title: PocketAgent.SetPushNotificationTagsForDevice event method
description: Scripting events called on the SetPushNotificationTagsForDevice method on the PocketAgent service agent.
so.generated: true
keywords:
  - "netserver"
  - "scripting"
so.date: 11.29.2022
so.topic: reference
so.envir:
  - "onsite"
---
# PocketAgent.SetPushNotificationTagsForDevice

Scripting events called on the <see cref='M:SuperOffice.CRM.Services.IPocketAgent.SetPushNotificationTagsForDevice'>SetPushNotificationTagsForDevice</see> method on the <see cref='IPocketAgent'>IPocketAgent</see>  service agent.

## BeforeSetPushNotificationTagsForDevice
```cs
    static void BeforeSetPushNotificationTagsForDevice(
       String  deviceIdentifier,
       String  tags,
       ref object  eventState
      );
```
Executes before the service method is invoked.
It can store some state in the *eventState* parameter, that is passed to the **After** and **AfterAsync** methods in this service call.
Event state is not preserved between different service calls. It is set to null at the start of each service call.
## AfterSetPushNotificationTagsForDevice
```cs
    static void AfterSetPushNotificationTagsForDevice(
       String  deviceIdentifier,
       String  tags,
       ref object  eventState
      );
```
Executes after the service method has been invoked. The service waits for this method to complete before returning the result to the caller.
This service call has no return value, so there is no **returnValue** parameter
Any state you set in the **Before** method is passed in through the *eventState* parameter.
## AfterSetPushNotificationTagsForDeviceAsync
```cs
    static void AfterSetPushNotificationTagsForDeviceAsync(
       String  deviceIdentifier,
       String  tags,
       ref object  eventState
      );
```
Executes after the service method is invoked, without waiting for the call to return.
The service call is not blocked waiting for this method to complete.
Any state you set in the **Before** method is passed in through the *eventState* parameter.

