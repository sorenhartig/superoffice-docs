---
title: Services84.MessagingAgent.CreateMessage SOAP
generated: 1
uid: Services84-Messaging-CreateMessage
---

# Services84 Messaging CreateMessage

SOAP request and response examples **Remote/Services84/Messaging.svc**
Implemented by the <see cref="M:SuperOffice.Services84.IMessagingAgent.CreateMessage">SuperOffice.Services84.IMessagingAgent.CreateMessage</see> method.

## CreateMessage

Create a new message and insert it in the message queue. (inbox)

* **incomingMessage:**

[WSDL file for Services84/Messaging](../Services84-Messaging.md)

Obtain a ticket from the [Services84/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## CreateMessage Request

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices842="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices841="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Messaging="http://www.superoffice.net/ws/crm/NetServer/Services84">
  <Messaging:ApplicationToken>1234567-1234-9876</Messaging:ApplicationToken>
  <Messaging:Credentials>
    <Messaging:Ticket>7T:1234abcxyzExample==</Messaging:Ticket>
  </Messaging:Credentials>
 <SOAP-ENV:Body>
   <Messaging:CreateMessage>
    <Messaging:IncomingMessage xsi:type="Messaging:IncomingMessage">
     <Messaging:To xsi:type="xsd:string"></Messaging:To>
     <Messaging:From xsi:type="xsd:string"></Messaging:From>
     <Messaging:Content xsi:type="xsd:string"></Messaging:Content>
     <Messaging:Format xsi:type="xsd:string"></Messaging:Format>
     <Messaging:SessionKey xsi:type="xsd:string"></Messaging:SessionKey>
     <Messaging:Plugin xsi:type="xsd:string"></Messaging:Plugin>
    </Messaging:IncomingMessage>
   </Messaging:CreateMessage>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

## CreateMessage Response

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices842="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices841="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Messaging="http://www.superoffice.net/ws/crm/NetServer/Services84">
 <SOAP-ENV:Body>
  <Messaging:CreateMessageResponse>
  </Messaging:CreateMessageResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```
