---
title: Services84.FreeTextAgent.SetSingleWordOperator SOAP
generated: 1
uid: Services84-FreeText-SetSingleWordOperator
---

# Services84 FreeText SetSingleWordOperator

SOAP request and response examples **Remote/Services84/FreeText.svc**
Implemented by the <see cref="M:SuperOffice.Services84.IFreeTextAgent.SetSingleWordOperator">SuperOffice.Services84.IFreeTextAgent.SetSingleWordOperator</see> method.

## SetSingleWordOperator

Sets the operator used when matching single words

* **freeTextOperator:** The operator

**Returns:** This method has no return value

[WSDL file for Services84/FreeText](../Services84-FreeText.md)

Obtain a ticket from the [Services84/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## SetSingleWordOperator Request

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices842="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices841="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:FreeText="http://www.superoffice.net/ws/crm/NetServer/Services84">
  <FreeText:ApplicationToken>1234567-1234-9876</FreeText:ApplicationToken>
  <FreeText:Credentials>
    <FreeText:Ticket>7T:1234abcxyzExample==</FreeText:Ticket>
  </FreeText:Credentials>
 <SOAP-ENV:Body>
   <FreeText:SetSingleWordOperator>
    <FreeText:FreeTextOperator xsi:type="FreeText:FreeTextOperator">Contains</FreeText:FreeTextOperator>
   </FreeText:SetSingleWordOperator>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

## SetSingleWordOperator Response

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices842="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices841="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:FreeText="http://www.superoffice.net/ws/crm/NetServer/Services84">
 <SOAP-ENV:Body>
  <FreeText:SetSingleWordOperatorResponse>
  </FreeText:SetSingleWordOperatorResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```
