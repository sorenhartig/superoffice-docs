---
title: Services88.DocumentAgent.CreateTempFile SOAP
generated: 1
uid: Services88-Document-CreateTempFile
---

# Services88 Document CreateTempFile

SOAP request and response examples **Remote/Services88/Document.svc**
Implemented by the <see cref="M:SuperOffice.Services88.IDocumentAgent.CreateTempFile">SuperOffice.Services88.IDocumentAgent.CreateTempFile</see> method.

## CreateTempFile

Create a new temporary file based on the provided stream.  Specified filename may be overridden, and actual name is returned.

* **filename:** Wanted name of file.
* **dataStream:** Data to be added to the file.

**Returns:** Actual used filename.

[WSDL file for Services88/Document](../Services88-Document.md)

Obtain a ticket from the [Services88/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## CreateTempFile Request

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices882="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices881="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Document="http://www.superoffice.net/ws/crm/NetServer/Services88">
  <Document:ApplicationToken>1234567-1234-9876</Document:ApplicationToken>
  <Document:Credentials>
    <Document:Ticket>7T:1234abcxyzExample==</Document:Ticket>
  </Document:Credentials>
 <SOAP-ENV:Body>
   <Document:CreateTempFile>
    <Document:Filename xsi:type="xsd:string"></Document:Filename>
    <Document:DataStream xsi:type="xsd:base64Binary"></Document:DataStream>
   </Document:CreateTempFile>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

## CreateTempFile Response

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices882="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices881="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Document="http://www.superoffice.net/ws/crm/NetServer/Services88">
 <SOAP-ENV:Body>
  <Document:CreateTempFileResponse>
   <Document:Response xsi:type="xsd:string"></Document:Response>
  </Document:CreateTempFileResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```
