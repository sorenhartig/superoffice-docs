---
title: Services87.ListAgent.GetConsentSources SOAP
generated: 1
uid: Services87-List-GetConsentSources
---

# Services87 List GetConsentSources

SOAP request and response examples **Remote/Services87/List.svc**
Implemented by the <see cref="M:SuperOffice.Services87.IListAgent.GetConsentSources">SuperOffice.Services87.IListAgent.GetConsentSources</see> method.

## GetConsentSources

Returns all defined Sources.

**Returns:** An array of all defined Sources

[WSDL file for Services87/List](../Services87-List.md)

Obtain a ticket from the [Services87/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## GetConsentSources Request

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices872="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices871="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:List="http://www.superoffice.net/ws/crm/NetServer/Services87">
  <List:ApplicationToken>1234567-1234-9876</List:ApplicationToken>
  <List:Credentials>
    <List:Ticket>7T:1234abcxyzExample==</List:Ticket>
  </List:Credentials>
 <SOAP-ENV:Body>
   <List:GetConsentSources>
   </List:GetConsentSources>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

## GetConsentSources Response

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices872="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices871="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:List="http://www.superoffice.net/ws/crm/NetServer/Services87">
 <SOAP-ENV:Body>
  <List:GetConsentSourcesResponse>
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
  </List:GetConsentSourcesResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```
