---
title: Services88.PersonAgent.GetPhones SOAP
generated: 1
uid: Services88-Person-GetPhones
---

# Services88 Person GetPhones

SOAP request and response examples **Remote/Services88/Person.svc**
Implemented by the <see cref="M:SuperOffice.Services88.IPersonAgent.GetPhones">SuperOffice.Services88.IPersonAgent.GetPhones</see> method.

## GetPhones

Returning all phones that belong to a person, ordered by the phone type.

* **personId:** The person id

**Returns:** An array of Phones

[WSDL file for Services88/Person](../Services88-Person.md)

Obtain a ticket from the [Services88/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## GetPhones Request

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices882="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices881="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Person="http://www.superoffice.net/ws/crm/NetServer/Services88">
  <Person:ApplicationToken>1234567-1234-9876</Person:ApplicationToken>
  <Person:Credentials>
    <Person:Ticket>7T:1234abcxyzExample==</Person:Ticket>
  </Person:Credentials>
 <SOAP-ENV:Body>
   <Person:GetPhones>
    <Person:PersonId xsi:type="xsd:int">0</Person:PersonId>
   </Person:GetPhones>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

## GetPhones Response

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices882="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices881="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Person="http://www.superoffice.net/ws/crm/NetServer/Services88">
 <SOAP-ENV:Body>
  <Person:GetPhonesResponse>
   <Person:Response xsi:type="Person:ArrayOfEntityElement">
    <Person:EntityElement xsi:type="Person:EntityElement">
     <Person:Value xsi:type="xsd:string"></Person:Value>
     <Person:StrippedValue xsi:type="xsd:string"></Person:StrippedValue>
     <Person:Description xsi:type="xsd:string"></Person:Description>
    </Person:EntityElement>
   </Person:Response>
  </Person:GetPhonesResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```
