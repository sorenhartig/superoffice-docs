---
title: Services85.ErpSyncAgent.CreateErpActorFromCrm SOAP
generated: 1
uid: Services85-ErpSync-CreateErpActorFromCrm
---

# Services85 ErpSync CreateErpActorFromCrm

SOAP request and response examples **Remote/Services85/ErpSync.svc**
Implemented by the <see cref="M:SuperOffice.Services85.IErpSyncAgent.CreateErpActorFromCrm">SuperOffice.Services85.IErpSyncAgent.CreateErpActorFromCrm</see> method.

## CreateErpActorFromCrm

Create ErpActor from crm entity

* **connectionId:** The connection ID
* **crmEntityId:** The ID of the CRM entity to create an ERP actor from
* **erpActorType:** The ERP actor type
* **crmActorType:** The CRM actor type
* **erpFieldKeyValues:** A map of matching erp field keys and values to set for the new erp entity

**Returns:** Created ERP actor with success

[WSDL file for Services85/ErpSync](../Services85-ErpSync.md)

Obtain a ticket from the [Services85/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## CreateErpActorFromCrm Request

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices852="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices851="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:ErpSync="http://www.superoffice.net/ws/crm/NetServer/Services85">
  <ErpSync:ApplicationToken>1234567-1234-9876</ErpSync:ApplicationToken>
  <ErpSync:Credentials>
    <ErpSync:Ticket>7T:1234abcxyzExample==</ErpSync:Ticket>
  </ErpSync:Credentials>
 <SOAP-ENV:Body>
   <ErpSync:CreateErpActorFromCrm>
    <ErpSync:ConnectionId xsi:type="xsd:int">0</ErpSync:ConnectionId>
    <ErpSync:CrmEntityId xsi:type="xsd:int">0</ErpSync:CrmEntityId>
    <ErpSync:ErpActorType xsi:type="ErpSync:ErpActorType">Unknown</ErpSync:ErpActorType>
    <ErpSync:CrmActorType xsi:type="ErpSync:CrmActorType">Unknown</ErpSync:CrmActorType>
    <ErpSync:ErpFieldKeyValues xsi:type="ErpSync:StringDictionary">
     <ErpSync:StringKeyValuePair>
      <ErpSync:Key xsi:type="xsd:string"></ErpSync:Key>
      <ErpSync:Value xsi:type="xsd:string"></ErpSync:Value>
     </ErpSync:StringKeyValuePair>
    </ErpSync:ErpFieldKeyValues>
   </ErpSync:CreateErpActorFromCrm>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

## CreateErpActorFromCrm Response

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices852="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices851="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:ErpSync="http://www.superoffice.net/ws/crm/NetServer/Services85">
 <SOAP-ENV:Body>
  <ErpSync:CreateErpActorFromCrmResponse>
   <ErpSync:Response xsi:type="xsd:boolean">false</ErpSync:Response>
  </ErpSync:CreateErpActorFromCrmResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```
