---
title: Services88.UserDefinedFieldInfoAgent.IsPublishEventActive SOAP
generated: 1
uid: Services88-UserDefinedFieldInfo-IsPublishEventActive
---

# Services88 UserDefinedFieldInfo IsPublishEventActive

SOAP request and response examples **Remote/Services88/UserDefinedFieldInfo.svc**
Implemented by the <see cref="M:SuperOffice.Services88.IUserDefinedFieldInfoAgent.IsPublishEventActive">SuperOffice.Services88.IUserDefinedFieldInfoAgent.IsPublishEventActive</see> method.

## IsPublishEventActive

Check if the publish event is active for the given type

* **type:**

[WSDL file for Services88/UserDefinedFieldInfo](../Services88-UserDefinedFieldInfo.md)

Obtain a ticket from the [Services88/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## IsPublishEventActive Request

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices882="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices881="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:UserDefinedFieldInfo="http://www.superoffice.net/ws/crm/NetServer/Services88">
  <UserDefinedFieldInfo:ApplicationToken>1234567-1234-9876</UserDefinedFieldInfo:ApplicationToken>
  <UserDefinedFieldInfo:Credentials>
    <UserDefinedFieldInfo:Ticket>7T:1234abcxyzExample==</UserDefinedFieldInfo:Ticket>
  </UserDefinedFieldInfo:Credentials>
 <SOAP-ENV:Body>
   <UserDefinedFieldInfo:IsPublishEventActive>
    <UserDefinedFieldInfo:Type xsi:type="UserDefinedFieldInfo:UDefType">Invalid</UserDefinedFieldInfo:Type>
   </UserDefinedFieldInfo:IsPublishEventActive>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

## IsPublishEventActive Response

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices882="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices881="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:UserDefinedFieldInfo="http://www.superoffice.net/ws/crm/NetServer/Services88">
 <SOAP-ENV:Body>
  <UserDefinedFieldInfo:IsPublishEventActiveResponse>
   <UserDefinedFieldInfo:Response xsi:type="xsd:boolean">false</UserDefinedFieldInfo:Response>
  </UserDefinedFieldInfo:IsPublishEventActiveResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```
