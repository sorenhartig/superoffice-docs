---
title: Services87.BatchAgent.GetBatchTaskInfosByNameAndState SOAP
generated: 1
uid: Services87-Batch-GetBatchTaskInfosByNameAndState
---

# Services87 Batch GetBatchTaskInfosByNameAndState

SOAP request and response examples **Remote/Services87/Batch.svc**
Implemented by the <see cref="M:SuperOffice.Services87.IBatchAgent.GetBatchTaskInfosByNameAndState">SuperOffice.Services87.IBatchAgent.GetBatchTaskInfosByNameAndState</see> method.

## GetBatchTaskInfosByNameAndState

Gets an array of BatchTaskInfo with state defined by a BatchTaskState and the batchtask definition name.

* **name:** Batchtask definition name.
* **state:** The BatchTaskState to get batch tasks for.

**Returns:** Returns an array of BatchTaskInfo.

[WSDL file for Services87/Batch](../Services87-Batch.md)

Obtain a ticket from the [Services87/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## GetBatchTaskInfosByNameAndState Request

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices872="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices871="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Batch="http://www.superoffice.net/ws/crm/NetServer/Services87">
  <Batch:ApplicationToken>1234567-1234-9876</Batch:ApplicationToken>
  <Batch:Credentials>
    <Batch:Ticket>7T:1234abcxyzExample==</Batch:Ticket>
  </Batch:Credentials>
 <SOAP-ENV:Body>
   <Batch:GetBatchTaskInfosByNameAndState>
    <Batch:Name xsi:type="xsd:string"></Batch:Name>
    <Batch:State xsi:type="Batch:BatchTaskState">Unknown</Batch:State>
   </Batch:GetBatchTaskInfosByNameAndState>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

## GetBatchTaskInfosByNameAndState Response

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices872="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices871="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Batch="http://www.superoffice.net/ws/crm/NetServer/Services87">
 <SOAP-ENV:Body>
  <Batch:GetBatchTaskInfosByNameAndStateResponse>
   <Batch:Response xsi:type="Batch:ArrayOfBatchTaskInfo">
    <Batch:BatchTaskInfo xsi:type="Batch:BatchTaskInfo">
     <Batch:Id xsi:type="xsd:int">0</Batch:Id>
     <Batch:Name xsi:type="xsd:string"></Batch:Name>
     <Batch:AssociateId xsi:type="xsd:int">0</Batch:AssociateId>
     <Batch:DetailsTable xsi:type="xsd:short">0</Batch:DetailsTable>
     <Batch:DetailsRecord xsi:type="xsd:int">0</Batch:DetailsRecord>
     <Batch:IsSystemTask xsi:type="xsd:boolean">false</Batch:IsSystemTask>
     <Batch:IsInternalTask xsi:type="xsd:boolean">false</Batch:IsInternalTask>
     <Batch:ParameterObject xsi:type="Batch:StringDictionary">
      <Batch:StringKeyValuePair>
       <Batch:Key xsi:type="xsd:string"></Batch:Key>
       <Batch:Value xsi:type="xsd:string"></Batch:Value>
      </Batch:StringKeyValuePair>
     </Batch:ParameterObject>
     <Batch:LastStarted xsi:type="xsd:dateTime">2022-08-26T08:56:25Z</Batch:LastStarted>
     <Batch:Created xsi:type="xsd:dateTime">2022-08-26T08:56:25Z</Batch:Created>
     <Batch:StartCount xsi:type="xsd:int">0</Batch:StartCount>
     <Batch:DatabaseSerialNumber xsi:type="xsd:string"></Batch:DatabaseSerialNumber>
     <Batch:Context xsi:type="xsd:string"></Batch:Context>
     <Batch:Result xsi:type="xsd:string"></Batch:Result>
     <Batch:State xsi:type="Batch:BatchTaskState">Unknown</Batch:State>
     <Batch:Description xsi:type="xsd:string"></Batch:Description>
     <Batch:Response xsi:type="xsd:string"></Batch:Response>
     <Batch:Request xsi:type="xsd:string"></Batch:Request>
     <Batch:ProgressDescription xsi:type="xsd:string"></Batch:ProgressDescription>
     <Batch:ProgressPercent xsi:type="xsd:short">0</Batch:ProgressPercent>
    </Batch:BatchTaskInfo>
   </Batch:Response>
  </Batch:GetBatchTaskInfosByNameAndStateResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```
