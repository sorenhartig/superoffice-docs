---
title: Services85.QuoteAgent.SaveQuoteLineConfiguration SOAP
generated: 1
uid: Services85-Quote-SaveQuoteLineConfiguration
---

# Services85 Quote SaveQuoteLineConfiguration

SOAP request and response examples **Remote/Services85/Quote.svc**
Implemented by the <see cref="M:SuperOffice.Services85.IQuoteAgent.SaveQuoteLineConfiguration">SuperOffice.Services85.IQuoteAgent.SaveQuoteLineConfiguration</see> method.

## SaveQuoteLineConfiguration

Save a QuoteLineConfiguration object. It is not possible to add a new configuration.

* **quoteLineConfiguration:** The QuoteLineConfiguration to save.

**Returns:** The saved QuoteLineConfiguration.

[WSDL file for Services85/Quote](../Services85-Quote.md)

Obtain a ticket from the [Services85/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## SaveQuoteLineConfiguration Request

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices852="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices851="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Quote="http://www.superoffice.net/ws/crm/NetServer/Services85">
  <Quote:ApplicationToken>1234567-1234-9876</Quote:ApplicationToken>
  <Quote:Credentials>
    <Quote:Ticket>7T:1234abcxyzExample==</Quote:Ticket>
  </Quote:Credentials>
 <SOAP-ENV:Body>
   <Quote:SaveQuoteLineConfiguration>
    <Quote:QuoteLineConfiguration xsi:type="Quote:QuoteLineConfiguration">
     <Quote:QuoteLineConfigurationId xsi:type="xsd:int">0</Quote:QuoteLineConfigurationId>
     <Quote:FieldName xsi:type="xsd:string"></Quote:FieldName>
     <Quote:Label xsi:type="xsd:string"></Quote:Label>
     <Quote:Tooltip xsi:type="xsd:string"></Quote:Tooltip>
     <Quote:Editable xsi:type="xsd:boolean">false</Quote:Editable>
     <Quote:InUse xsi:type="xsd:boolean">false</Quote:InUse>
     <Quote:Mandatory xsi:type="xsd:boolean">false</Quote:Mandatory>
     <Quote:Rank xsi:type="xsd:int">0</Quote:Rank>
     <Quote:RestrictEdit xsi:type="xsd:boolean">false</Quote:RestrictEdit>
    </Quote:QuoteLineConfiguration>
   </Quote:SaveQuoteLineConfiguration>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

## SaveQuoteLineConfiguration Response

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices852="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices851="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Quote="http://www.superoffice.net/ws/crm/NetServer/Services85">
 <SOAP-ENV:Body>
  <Quote:SaveQuoteLineConfigurationResponse>
   <Quote:Response xsi:type="Quote:QuoteLineConfiguration">
    <Quote:QuoteLineConfigurationId xsi:type="xsd:int">0</Quote:QuoteLineConfigurationId>
    <Quote:FieldName xsi:type="xsd:string"></Quote:FieldName>
    <Quote:Label xsi:type="xsd:string"></Quote:Label>
    <Quote:Tooltip xsi:type="xsd:string"></Quote:Tooltip>
    <Quote:Editable xsi:type="xsd:boolean">false</Quote:Editable>
    <Quote:InUse xsi:type="xsd:boolean">false</Quote:InUse>
    <Quote:Mandatory xsi:type="xsd:boolean">false</Quote:Mandatory>
    <Quote:Rank xsi:type="xsd:int">0</Quote:Rank>
    <Quote:RestrictEdit xsi:type="xsd:boolean">false</Quote:RestrictEdit>
   </Quote:Response>
  </Quote:SaveQuoteLineConfigurationResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```
