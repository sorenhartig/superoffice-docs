---
title: Services84.ListAgent.SaveQuickReplies SOAP
generated: 1
uid: Services84-List-SaveQuickReplies
---

# Services84 List SaveQuickReplies

SOAP request and response examples **Remote/Services84/List.svc**
Implemented by the <see cref="M:SuperOffice.Services84.IListAgent.SaveQuickReplies">SuperOffice.Services84.IListAgent.SaveQuickReplies</see> method.

## SaveQuickReplies

Method to save all quick replies for a given associate

* **quickReplies:** Array of quick replies

[WSDL file for Services84/List](../Services84-List.md)

Obtain a ticket from the [Services84/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## SaveQuickReplies Request

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices842="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices841="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:List="http://www.superoffice.net/ws/crm/NetServer/Services84">
  <List:ApplicationToken>1234567-1234-9876</List:ApplicationToken>
  <List:Credentials>
    <List:Ticket>7T:1234abcxyzExample==</List:Ticket>
  </List:Credentials>
 <SOAP-ENV:Body>
   <List:SaveQuickReplies>
    <List:QuickReplies xsi:type="List:ArrayOfQuickReply">
     <List:QuickReply xsi:type="List:QuickReply">
      <List:QuickReplyId xsi:type="xsd:int">0</List:QuickReplyId>
      <List:Name xsi:type="xsd:string"></List:Name>
      <List:HtmlBody xsi:type="xsd:string"></List:HtmlBody>
     </List:QuickReply>
    </List:QuickReplies>
   </List:SaveQuickReplies>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

## SaveQuickReplies Response

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices842="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices841="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:List="http://www.superoffice.net/ws/crm/NetServer/Services84">
 <SOAP-ENV:Body>
  <List:SaveQuickRepliesResponse>
  </List:SaveQuickRepliesResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```
