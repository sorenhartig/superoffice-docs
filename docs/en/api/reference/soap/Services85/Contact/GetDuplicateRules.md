---
title: Services85.ContactAgent.GetDuplicateRules SOAP
generated: 1
uid: Services85-Contact-GetDuplicateRules
---

# Services85 Contact GetDuplicateRules

SOAP request and response examples **Remote/Services85/Contact.svc**
Implemented by the <see cref="M:SuperOffice.Services85.IContactAgent.GetDuplicateRules">SuperOffice.Services85.IContactAgent.GetDuplicateRules</see> method.

## GetDuplicateRules

Retrieve all available duplicate rules for contact

**Returns:** All available duplicate rules

[WSDL file for Services85/Contact](../Services85-Contact.md)

Obtain a ticket from the [Services85/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## GetDuplicateRules Request

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices852="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices851="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Contact="http://www.superoffice.net/ws/crm/NetServer/Services85">
  <Contact:ApplicationToken>1234567-1234-9876</Contact:ApplicationToken>
  <Contact:Credentials>
    <Contact:Ticket>7T:1234abcxyzExample==</Contact:Ticket>
  </Contact:Credentials>
 <SOAP-ENV:Body>
   <Contact:GetDuplicateRules>
   </Contact:GetDuplicateRules>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

## GetDuplicateRules Response

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices852="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices851="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Contact="http://www.superoffice.net/ws/crm/NetServer/Services85">
 <SOAP-ENV:Body>
  <Contact:GetDuplicateRulesResponse>
   <Contact:Response xsi:type="Contact:ArrayOfDuplicateRule">
    <Contact:DuplicateRule xsi:type="Contact:DuplicateRule">
     <Contact:Name xsi:type="xsd:string"></Contact:Name>
     <Contact:DisplayName xsi:type="xsd:string"></Contact:DisplayName>
     <Contact:DisplayTooltip xsi:type="xsd:string"></Contact:DisplayTooltip>
     <Contact:IsActive xsi:type="xsd:boolean">false</Contact:IsActive>
    </Contact:DuplicateRule>
   </Contact:Response>
  </Contact:GetDuplicateRulesResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```
