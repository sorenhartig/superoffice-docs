---
title: Services85.UserAgent.IsUserNameValidWithReason SOAP
generated: 1
uid: Services85-User-IsUserNameValidWithReason
---

# Services85 User IsUserNameValidWithReason

SOAP request and response examples **Remote/Services85/User.svc**
Implemented by the <see cref="M:SuperOffice.Services85.IUserAgent.IsUserNameValidWithReason">SuperOffice.Services85.IUserAgent.IsUserNameValidWithReason</see> method.

## IsUserNameValidWithReason

* **associateId:**
* **type:**
* **personId:**
* **userName:**

[WSDL file for Services85/User](../Services85-User.md)

Obtain a ticket from the [Services85/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## IsUserNameValidWithReason Request

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices852="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices851="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:User="http://www.superoffice.net/ws/crm/NetServer/Services85">
  <User:ApplicationToken>1234567-1234-9876</User:ApplicationToken>
  <User:Credentials>
    <User:Ticket>7T:1234abcxyzExample==</User:Ticket>
  </User:Credentials>
 <SOAP-ENV:Body>
   <User:IsUserNameValidWithReason>
    <User:AssociateId xsi:type="xsd:int">0</User:AssociateId>
    <User:Type xsi:type="User:UserType">Unknown</User:Type>
    <User:PersonId xsi:type="xsd:int">0</User:PersonId>
    <User:UserName xsi:type="xsd:string"></User:UserName>
   </User:IsUserNameValidWithReason>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

## IsUserNameValidWithReason Response

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices852="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices851="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:User="http://www.superoffice.net/ws/crm/NetServer/Services85">
 <SOAP-ENV:Body>
  <User:IsUserNameValidWithReasonResponse>
   <User:Response xsi:type="User:UserValidationResult">
    <User:Reason xsi:type="xsd:string"></User:Reason>
    <User:Result xsi:type="xsd:boolean">false</User:Result>
   </User:Response>
  </User:IsUserNameValidWithReasonResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```
