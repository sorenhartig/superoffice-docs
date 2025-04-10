---
title: Services87.ListAgent.GetDocumentTypesForPlugin SOAP
generated: 1
uid: Services87-List-GetDocumentTypesForPlugin
---

# Services87 List GetDocumentTypesForPlugin

SOAP request and response examples **Remote/Services87/List.svc**
Implemented by the <see cref="M:SuperOffice.Services87.IListAgent.GetDocumentTypesForPlugin">SuperOffice.Services87.IListAgent.GetDocumentTypesForPlugin</see> method.

## GetDocumentTypesForPlugin

Get a list of document types supported by a given document plugin. Use the document template type when creating a new template.

* **pluginId:** Numeric document plugin id, corresponding to the doctmpl.AutoeventId, doctmpl.LoadTemplateFromPlugin.

**Returns:** Dictionary mapping document type id=name

[WSDL file for Services87/List](../Services87-List.md)

Obtain a ticket from the [Services87/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## GetDocumentTypesForPlugin Request

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices872="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices871="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:List="http://www.superoffice.net/ws/crm/NetServer/Services87">
  <List:ApplicationToken>1234567-1234-9876</List:ApplicationToken>
  <List:Credentials>
    <List:Ticket>7T:1234abcxyzExample==</List:Ticket>
  </List:Credentials>
 <SOAP-ENV:Body>
   <List:GetDocumentTypesForPlugin>
    <List:PluginId xsi:type="xsd:int">0</List:PluginId>
   </List:GetDocumentTypesForPlugin>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

## GetDocumentTypesForPlugin Response

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices872="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices871="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:List="http://www.superoffice.net/ws/crm/NetServer/Services87">
 <SOAP-ENV:Body>
  <List:GetDocumentTypesForPluginResponse>
   <List:Response xsi:type="List:IntStringDictionary">
    <List:IntStringKeyValuePair>
     <List:Key xsi:type="xsd:int">0</List:Key>
     <List:Value xsi:type="xsd:string"></List:Value>
    </List:IntStringKeyValuePair>
   </List:Response>
  </List:GetDocumentTypesForPluginResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```
