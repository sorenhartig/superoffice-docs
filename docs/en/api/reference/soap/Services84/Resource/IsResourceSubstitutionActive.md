---
title: Services84.ResourceAgent.IsResourceSubstitutionActive SOAP
generated: 1
uid: Services84-Resource-IsResourceSubstitutionActive
---

# Services84 Resource IsResourceSubstitutionActive

SOAP request and response examples **Remote/Services84/Resource.svc**
Implemented by the <see cref="M:SuperOffice.Services84.IResourceAgent.IsResourceSubstitutionActive">SuperOffice.Services84.IResourceAgent.IsResourceSubstitutionActive</see> method.

## IsResourceSubstitutionActive

Determine if resource substitution/override is active, globally or for a subset of resources/cultures

* **resourceNames:** Array of names of resources for which overrides are sought; if empty, then get the MASTER on/off
* **culture:** .NET culture string; if empty, then get for all cultures (unless resourceName

**Returns:** Array of override objects, empty if there are none; the ResourceValue member is not set by this call

[WSDL file for Services84/Resource](../Services84-Resource.md)

Obtain a ticket from the [Services84/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## IsResourceSubstitutionActive Request

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices842="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices841="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Resource="http://www.superoffice.net/ws/crm/NetServer/Services84">
  <Resource:ApplicationToken>1234567-1234-9876</Resource:ApplicationToken>
  <Resource:Credentials>
    <Resource:Ticket>7T:1234abcxyzExample==</Resource:Ticket>
  </Resource:Credentials>
 <SOAP-ENV:Body>
   <Resource:IsResourceSubstitutionActive>
    <Resource:ResourceNames xsi:type="NetServerServices842:ArrayOfstring">
     <NetServerServices842:string xsi:type="xsd:string"></NetServerServices842:string>
    </Resource:ResourceNames>
    <Resource:Culture xsi:type="xsd:string"></Resource:Culture>
   </Resource:IsResourceSubstitutionActive>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

## IsResourceSubstitutionActive Response

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices842="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices841="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Resource="http://www.superoffice.net/ws/crm/NetServer/Services84">
 <SOAP-ENV:Body>
  <Resource:IsResourceSubstitutionActiveResponse>
   <Resource:Response xsi:type="Resource:ArrayOfResourceOverride">
    <Resource:ResourceOverride xsi:type="Resource:ResourceOverride">
     <Resource:ResourceName xsi:type="xsd:string"></Resource:ResourceName>
     <Resource:ResourceValue xsi:type="xsd:string"></Resource:ResourceValue>
     <Resource:Culture xsi:type="xsd:string"></Resource:Culture>
     <Resource:IsActive xsi:type="xsd:boolean">false</Resource:IsActive>
    </Resource:ResourceOverride>
   </Resource:Response>
  </Resource:IsResourceSubstitutionActiveResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```
