---
title: Services87.ResourceAgent.SetResourceSubstitution SOAP
generated: 1
uid: Services87-Resource-SetResourceSubstitution
---

# Services87 Resource SetResourceSubstitution

SOAP request and response examples **Remote/Services87/Resource.svc**
Implemented by the <see cref="M:SuperOffice.Services87.IResourceAgent.SetResourceSubstitution">SuperOffice.Services87.IResourceAgent.SetResourceSubstitution</see> method.

## SetResourceSubstitution

Create or update a resource substitution

* **resourceName:** The name of the resource, without any brackets
* **resourceValues:** The new value of the resource
* **culture:** The .NET culture string
* **isActive:** Is the subsitution now active

**Returns:** This method has no return value

[WSDL file for Services87/Resource](../Services87-Resource.md)

Obtain a ticket from the [Services87/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## SetResourceSubstitution Request

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices872="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices871="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Resource="http://www.superoffice.net/ws/crm/NetServer/Services87">
  <Resource:ApplicationToken>1234567-1234-9876</Resource:ApplicationToken>
  <Resource:Credentials>
    <Resource:Ticket>7T:1234abcxyzExample==</Resource:Ticket>
  </Resource:Credentials>
 <SOAP-ENV:Body>
   <Resource:SetResourceSubstitution>
    <Resource:ResourceName xsi:type="xsd:string"></Resource:ResourceName>
    <Resource:ResourceValues xsi:type="xsd:string"></Resource:ResourceValues>
    <Resource:Culture xsi:type="xsd:string"></Resource:Culture>
    <Resource:IsActive xsi:type="xsd:boolean">false</Resource:IsActive>
   </Resource:SetResourceSubstitution>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

## SetResourceSubstitution Response

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices872="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices871="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Resource="http://www.superoffice.net/ws/crm/NetServer/Services87">
 <SOAP-ENV:Body>
  <Resource:SetResourceSubstitutionResponse>
  </Resource:SetResourceSubstitutionResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```
