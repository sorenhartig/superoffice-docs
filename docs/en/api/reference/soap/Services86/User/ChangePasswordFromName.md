---
title: Services86.UserAgent.ChangePasswordFromName SOAP
generated: 1
uid: Services86-User-ChangePasswordFromName
---

# Services86 User ChangePasswordFromName

SOAP request and response examples **Remote/Services86/User.svc**
Implemented by the <see cref="M:SuperOffice.Services86.IUserAgent.ChangePasswordFromName">SuperOffice.Services86.IUserAgent.ChangePasswordFromName</see> method.

## ChangePasswordFromName

Change password for a user.
<para /><b>Online Restricted:</b> The User agent is not available in Online by default. User management is not allowed for partner apps.

* **associateName:** AssociateId of the user to change password for.
* **oldPassword:** The current password of the user.  Administrators can leave this blank to force a new password upon a user.
* **newPassword:** The new password for the user

**Returns:** True if the password was successfully changed.

[WSDL file for Services86/User](../Services86-User.md)

Obtain a ticket from the [Services86/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## ChangePasswordFromName Request

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices862="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices861="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:User="http://www.superoffice.net/ws/crm/NetServer/Services86">
  <User:ApplicationToken>1234567-1234-9876</User:ApplicationToken>
  <User:Credentials>
    <User:Ticket>7T:1234abcxyzExample==</User:Ticket>
  </User:Credentials>
 <SOAP-ENV:Body>
   <User:ChangePasswordFromName>
    <User:AssociateName xsi:type="xsd:string"></User:AssociateName>
    <User:OldPassword xsi:type="xsd:string"></User:OldPassword>
    <User:NewPassword xsi:type="xsd:string"></User:NewPassword>
   </User:ChangePasswordFromName>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

## ChangePasswordFromName Response

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices862="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices861="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:User="http://www.superoffice.net/ws/crm/NetServer/Services86">
 <SOAP-ENV:Body>
  <User:ChangePasswordFromNameResponse>
   <User:Response xsi:type="xsd:boolean">false</User:Response>
  </User:ChangePasswordFromNameResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```
