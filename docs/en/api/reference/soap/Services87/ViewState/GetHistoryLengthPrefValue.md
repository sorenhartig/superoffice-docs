---
title: Services87.ViewStateAgent.GetHistoryLengthPrefValue SOAP
generated: 1
uid: Services87-ViewState-GetHistoryLengthPrefValue
---

# Services87 ViewState GetHistoryLengthPrefValue

SOAP request and response examples **Remote/Services87/ViewState.svc**
Implemented by the <see cref="M:SuperOffice.Services87.IViewStateAgent.GetHistoryLengthPrefValue">SuperOffice.Services87.IViewStateAgent.GetHistoryLengthPrefValue</see> method.

## GetHistoryLengthPrefValue

Get the logged on user's preferred history list length. Will return the system preference if no user preferences are available.

**Returns:** The history list lenght

[WSDL file for Services87/ViewState](../Services87-ViewState.md)

Obtain a ticket from the [Services87/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## GetHistoryLengthPrefValue Request

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices872="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices871="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:ViewState="http://www.superoffice.net/ws/crm/NetServer/Services87">
  <ViewState:ApplicationToken>1234567-1234-9876</ViewState:ApplicationToken>
  <ViewState:Credentials>
    <ViewState:Ticket>7T:1234abcxyzExample==</ViewState:Ticket>
  </ViewState:Credentials>
 <SOAP-ENV:Body>
   <ViewState:GetHistoryLengthPrefValue>
   </ViewState:GetHistoryLengthPrefValue>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

## GetHistoryLengthPrefValue Response

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices872="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices871="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:ViewState="http://www.superoffice.net/ws/crm/NetServer/Services87">
 <SOAP-ENV:Body>
  <ViewState:GetHistoryLengthPrefValueResponse>
   <ViewState:Response xsi:type="xsd:int">0</ViewState:Response>
  </ViewState:GetHistoryLengthPrefValueResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```
