---
uid: documentagent-substitutetemplatevariableswithcustomtags
title: DocumentAgent.SubstituteTemplateVariablesWithCustomTags event method
description: Scripting events called on the SubstituteTemplateVariablesWithCustomTags method on the DocumentAgent service agent.
so.generated: true
keywords:
  - "netserver"
  - "scripting"
so.date: 11.29.2022
so.topic: reference
so.envir:
  - "onsite"
---
# DocumentAgent.SubstituteTemplateVariablesWithCustomTags

Scripting events called on the <see cref='M:SuperOffice.CRM.Services.IDocumentAgent.SubstituteTemplateVariablesWithCustomTags'>SubstituteTemplateVariablesWithCustomTags</see> method on the <see cref='IDocumentAgent'>IDocumentAgent</see>  service agent.

## BeforeSubstituteTemplateVariablesWithCustomTags
```cs
    static void BeforeSubstituteTemplateVariablesWithCustomTags(
       String  source,
       GeneratorEncoding  generatorEncoding,
       String[]  customTags,
       String[]  customValues,
       Int32  contactId,
       Int32  personId,
       Int32  appointmentId,
       Int32  documentId,
       Int32  saleId,
       Int32  selectionId,
       Int32  projectId,
       String  cultureName,
       ref object  eventState
      );
```
Executes before the service method is invoked.
The return value is not calculated yet, so this method can't affect the result.
It can store some state in the *eventState* parameter, that is passed to the **After** and **AfterAsync** methods in this service call.
Event state is not preserved between different service calls. It is set to null at the start of each service call.
## AfterSubstituteTemplateVariablesWithCustomTags
```cs
    static void AfterSubstituteTemplateVariablesWithCustomTags(
       String  source,
       GeneratorEncoding  generatorEncoding,
       String[]  customTags,
       String[]  customValues,
       Int32  contactId,
       Int32  personId,
       Int32  appointmentId,
       Int32  documentId,
       Int32  saleId,
       Int32  selectionId,
       Int32  projectId,
       String  cultureName,
       ref String  returnValue,
       ref object  eventState
      );
```
Executes after the service method has been invoked. The service waits for this method to complete before returning the result to the caller.
The return value has been set. The script may modify the return value by altering the **returnValue** parameter.
Any state you set in the **Before** method is passed in through the *eventState* parameter.
## AfterSubstituteTemplateVariablesWithCustomTagsAsync
```cs
    static void AfterSubstituteTemplateVariablesWithCustomTagsAsync(
       String  source,
       GeneratorEncoding  generatorEncoding,
       String[]  customTags,
       String[]  customValues,
       Int32  contactId,
       Int32  personId,
       Int32  appointmentId,
       Int32  documentId,
       Int32  saleId,
       Int32  selectionId,
       Int32  projectId,
       String  cultureName,
       ref String  returnValue,
       ref object  eventState
      );
```
Executes after the service method is invoked, without waiting for the call to return.
The service call is not blocked waiting for this method to complete.
The async event handler cannot modify the return value of the service call.
Any state you set in the **Before** method is passed in through the *eventState* parameter.

