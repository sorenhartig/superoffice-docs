---
title: Services84.QuoteAgent.GetQuoteVersionWorkflowImageState SOAP
generated: 1
uid: Services84-Quote-GetQuoteVersionWorkflowImageState
---

# Services84 Quote GetQuoteVersionWorkflowImageState

SOAP request and response examples **Remote/Services84/Quote.svc**
Implemented by the <see cref="M:SuperOffice.Services84.IQuoteAgent.GetQuoteVersionWorkflowImageState">SuperOffice.Services84.IQuoteAgent.GetQuoteVersionWorkflowImageState</see> method.

## GetQuoteVersionWorkflowImageState

Get state icon and name for the Quote version dialog header.

* **quoteVersionId:** Id of the quote version to get the version state for.

**Returns:** Image and state name information

[WSDL file for Services84/Quote](../Services84-Quote.md)

Obtain a ticket from the [Services84/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## GetQuoteVersionWorkflowImageState Request

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices842="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices841="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Quote="http://www.superoffice.net/ws/crm/NetServer/Services84">
  <Quote:ApplicationToken>1234567-1234-9876</Quote:ApplicationToken>
  <Quote:Credentials>
    <Quote:Ticket>7T:1234abcxyzExample==</Quote:Ticket>
  </Quote:Credentials>
 <SOAP-ENV:Body>
   <Quote:GetQuoteVersionWorkflowImageState>
    <Quote:QuoteVersionId xsi:type="xsd:int">0</Quote:QuoteVersionId>
   </Quote:GetQuoteVersionWorkflowImageState>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

## GetQuoteVersionWorkflowImageState Response

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices842="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices841="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Quote="http://www.superoffice.net/ws/crm/NetServer/Services84">
 <SOAP-ENV:Body>
  <Quote:GetQuoteVersionWorkflowImageStateResponse>
   <Quote:Response xsi:type="Quote:QuoteVersionButtonState">
    <Quote:Action xsi:type="Quote:QuoteVersionButtonAction">None</Quote:Action>
    <Quote:ImageHint xsi:type="xsd:string"></Quote:ImageHint>
    <Quote:DisplayText xsi:type="xsd:string"></Quote:DisplayText>
    <Quote:TooltipText xsi:type="xsd:string"></Quote:TooltipText>
    <Quote:Enabled xsi:type="xsd:boolean">false</Quote:Enabled>
   </Quote:Response>
  </Quote:GetQuoteVersionWorkflowImageStateResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```
