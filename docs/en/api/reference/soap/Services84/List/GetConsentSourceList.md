---
title: Services84.ListAgent.GetConsentSourceList SOAP
generated: 1
uid: Services84-List-GetConsentSourceList
---

# Services84 List GetConsentSourceList

SOAP request and response examples **Remote/Services84/List.svc**
Implemented by the <see cref="M:SuperOffice.Services84.IListAgent.GetConsentSourceList">SuperOffice.Services84.IListAgent.GetConsentSourceList</see> method.

## GetConsentSourceList

Gets an array of ConsentSource objects.

* **consentSourceIds:** The identifiers of the ConsentSource object

**Returns:** Array of ConsentSource objects

[WSDL file for Services84/List](../Services84-List.md)

Obtain a ticket from the [Services84/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## GetConsentSourceList Request

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices842="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices841="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:List="http://www.superoffice.net/ws/crm/NetServer/Services84">
  <List:ApplicationToken>1234567-1234-9876</List:ApplicationToken>
  <List:Credentials>
    <List:Ticket>7T:1234abcxyzExample==</List:Ticket>
  </List:Credentials>
 <SOAP-ENV:Body>
   <List:GetConsentSourceList>
    <List:ConsentSourceIds xsi:type="NetServerServices842:ArrayOfint">
     <NetServerServices842:int xsi:type="xsd:int">0</NetServerServices842:int>
    </List:ConsentSourceIds>
   </List:GetConsentSourceList>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

## GetConsentSourceList Response

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices842="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices841="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:List="http://www.superoffice.net/ws/crm/NetServer/Services84">
 <SOAP-ENV:Body>
  <List:GetConsentSourceListResponse>
   <List:Response xsi:type="List:ArrayOfConsentSource">
    <List:ConsentSource xsi:type="List:ConsentSource">
     <List:ConsentSourceId xsi:type="xsd:int">0</List:ConsentSourceId>
     <List:Name xsi:type="xsd:string"></List:Name>
     <List:Tooltip xsi:type="xsd:string"></List:Tooltip>
     <List:Rank xsi:type="xsd:short">0</List:Rank>
     <List:Key xsi:type="xsd:string"></List:Key>
     <List:MailTemplateId xsi:type="xsd:int">0</List:MailTemplateId>
     <List:Deleted xsi:type="xsd:boolean">false</List:Deleted>
    </List:ConsentSource>
   </List:Response>
  </List:GetConsentSourceListResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```
