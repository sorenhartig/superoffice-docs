---
title: Services84.ListAgent.GetDeliveryTerms SOAP
generated: 1
uid: Services84-List-GetDeliveryTerms
---

# Services84 List GetDeliveryTerms

SOAP request and response examples **Remote/Services84/List.svc**
Implemented by the <see cref="M:SuperOffice.Services84.IListAgent.GetDeliveryTerms">SuperOffice.Services84.IListAgent.GetDeliveryTerms</see> method.

## GetDeliveryTerms

Returns all DeliveryTerms in SuperOffice db.

**Returns:** An array of all available DeliveryTerms

[WSDL file for Services84/List](../Services84-List.md)

Obtain a ticket from the [Services84/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## GetDeliveryTerms Request

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
   <List:GetDeliveryTerms>
   </List:GetDeliveryTerms>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

## GetDeliveryTerms Response

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
  <List:GetDeliveryTermsResponse>
   <List:Response xsi:type="List:ArrayOfDeliveryTerm">
    <List:DeliveryTerm xsi:type="List:DeliveryTerm">
     <List:Id xsi:type="xsd:int">0</List:Id>
     <List:Value xsi:type="xsd:string"></List:Value>
     <List:Tooltip xsi:type="xsd:string"></List:Tooltip>
    </List:DeliveryTerm>
   </List:Response>
  </List:GetDeliveryTermsResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```
