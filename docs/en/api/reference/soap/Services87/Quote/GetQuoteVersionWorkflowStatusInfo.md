---
title: Services87.QuoteAgent.GetQuoteVersionWorkflowStatusInfo SOAP
generated: 1
uid: Services87-Quote-GetQuoteVersionWorkflowStatusInfo
---

# Services87 Quote GetQuoteVersionWorkflowStatusInfo

SOAP request and response examples **Remote/Services87/Quote.svc**
Implemented by the <see cref="M:SuperOffice.Services87.IQuoteAgent.GetQuoteVersionWorkflowStatusInfo">SuperOffice.Services87.IQuoteAgent.GetQuoteVersionWorkflowStatusInfo</see> method.

## GetQuoteVersionWorkflowStatusInfo

Get status info for the Quote version dialog header. Collects most important warnings/errors from across all quotelines/alternatives in this quote version.

* **quoteVersionId:** Id of the quote version to get the status info for.

**Returns:** Most important status text + icon information.

[WSDL file for Services87/Quote](../Services87-Quote.md)

Obtain a ticket from the [Services87/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## GetQuoteVersionWorkflowStatusInfo Request

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices872="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices871="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Quote="http://www.superoffice.net/ws/crm/NetServer/Services87">
  <Quote:ApplicationToken>1234567-1234-9876</Quote:ApplicationToken>
  <Quote:Credentials>
    <Quote:Ticket>7T:1234abcxyzExample==</Quote:Ticket>
  </Quote:Credentials>
 <SOAP-ENV:Body>
   <Quote:GetQuoteVersionWorkflowStatusInfo>
    <Quote:QuoteVersionId xsi:type="xsd:int">0</Quote:QuoteVersionId>
   </Quote:GetQuoteVersionWorkflowStatusInfo>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

## GetQuoteVersionWorkflowStatusInfo Response

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices872="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices871="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Quote="http://www.superoffice.net/ws/crm/NetServer/Services87">
 <SOAP-ENV:Body>
  <Quote:GetQuoteVersionWorkflowStatusInfoResponse>
   <Quote:Response xsi:type="Quote:QuoteVersionStatusInformation">
    <Quote:Status xsi:type="Quote:QuoteStatus">Ok</Quote:Status>
    <Quote:IconHint xsi:type="xsd:string"></Quote:IconHint>
    <Quote:DisplayMessage xsi:type="xsd:string"></Quote:DisplayMessage>
    <Quote:DisplayTooltip xsi:type="xsd:string"></Quote:DisplayTooltip>
   </Quote:Response>
  </Quote:GetQuoteVersionWorkflowStatusInfoResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```
