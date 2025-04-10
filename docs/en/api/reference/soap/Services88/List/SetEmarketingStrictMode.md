---
title: Services88.ListAgent.SetEmarketingStrictMode SOAP
generated: 1
uid: Services88-List-SetEmarketingStrictMode
---

# Services88 List SetEmarketingStrictMode

SOAP request and response examples **Remote/Services88/List.svc**
Implemented by the <see cref="M:SuperOffice.Services88.IListAgent.SetEmarketingStrictMode">SuperOffice.Services88.IListAgent.SetEmarketingStrictMode</see> method.

## SetEmarketingStrictMode

Turn on the Emarketing strict mode, which will enable full GDPR rules concerning Emarketing consents and subscriptions

* **enable:** Set to true to enable strict mode

**Returns:** A void return

[WSDL file for Services88/List](../Services88-List.md)

Obtain a ticket from the [Services88/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## SetEmarketingStrictMode Request

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices882="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices881="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:List="http://www.superoffice.net/ws/crm/NetServer/Services88">
  <List:ApplicationToken>1234567-1234-9876</List:ApplicationToken>
  <List:Credentials>
    <List:Ticket>7T:1234abcxyzExample==</List:Ticket>
  </List:Credentials>
 <SOAP-ENV:Body>
   <List:SetEmarketingStrictMode>
    <List:Enable xsi:type="xsd:boolean">false</List:Enable>
   </List:SetEmarketingStrictMode>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

## SetEmarketingStrictMode Response

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices882="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices881="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:List="http://www.superoffice.net/ws/crm/NetServer/Services88">
 <SOAP-ENV:Body>
  <List:SetEmarketingStrictModeResponse>
  </List:SetEmarketingStrictModeResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```
