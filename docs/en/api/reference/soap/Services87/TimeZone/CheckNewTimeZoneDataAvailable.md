---
title: Services87.TimeZoneAgent.CheckNewTimeZoneDataAvailable SOAP
generated: 1
uid: Services87-TimeZone-CheckNewTimeZoneDataAvailable
---

# Services87 TimeZone CheckNewTimeZoneDataAvailable

SOAP request and response examples **Remote/Services87/TimeZone.svc**
Implemented by the <see cref="M:SuperOffice.Services87.ITimeZoneAgent.CheckNewTimeZoneDataAvailable">SuperOffice.Services87.ITimeZoneAgent.CheckNewTimeZoneDataAvailable</see> method.

## CheckNewTimeZoneDataAvailable

Check to see if new timezone data is available

**Returns:** Returns true if new timezone info is found available, false otherwise

[WSDL file for Services87/TimeZone](../Services87-TimeZone.md)

Obtain a ticket from the [Services87/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## CheckNewTimeZoneDataAvailable Request

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices871="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:TimeZone="http://www.superoffice.net/ws/crm/NetServer/Services87">
  <TimeZone:ApplicationToken>1234567-1234-9876</TimeZone:ApplicationToken>
  <TimeZone:Credentials>
    <TimeZone:Ticket>7T:1234abcxyzExample==</TimeZone:Ticket>
  </TimeZone:Credentials>
 <SOAP-ENV:Body>
   <TimeZone:CheckNewTimeZoneDataAvailable>
   </TimeZone:CheckNewTimeZoneDataAvailable>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

## CheckNewTimeZoneDataAvailable Response

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices871="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:TimeZone="http://www.superoffice.net/ws/crm/NetServer/Services87">
 <SOAP-ENV:Body>
  <TimeZone:CheckNewTimeZoneDataAvailableResponse>
   <TimeZone:Response xsi:type="xsd:boolean">false</TimeZone:Response>
  </TimeZone:CheckNewTimeZoneDataAvailableResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```
