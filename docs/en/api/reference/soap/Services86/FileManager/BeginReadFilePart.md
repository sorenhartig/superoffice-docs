---
title: Services86.FileManagerAgent.BeginReadFilePart SOAP
generated: 1
uid: Services86-FileManager-BeginReadFilePart
---

# Services86 FileManager BeginReadFilePart

SOAP request and response examples **Remote/Services86/FileManager.svc**
Implemented by the <see cref="M:SuperOffice.Services86.IFileManagerAgent.BeginReadFilePart">SuperOffice.Services86.IFileManagerAgent.BeginReadFilePart</see> method.

## BeginReadFilePart

[WSDL file for Services86/FileManager](../Services86-FileManager.md)

Obtain a ticket from the [Services86/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## BeginReadFilePart Request

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices861="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:FileManager="http://www.superoffice.net/ws/crm/NetServer/Services86">
  <FileManager:ApplicationToken>1234567-1234-9876</FileManager:ApplicationToken>
  <FileManager:Credentials>
    <FileManager:Ticket>7T:1234abcxyzExample==</FileManager:Ticket>
  </FileManager:Credentials>
 <SOAP-ENV:Body>
   <FileManager:BeginReadFilePart>
    <FileManager:DocumentId xsi:type="xsd:int">0</FileManager:DocumentId>
   </FileManager:BeginReadFilePart>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

## BeginReadFilePart Response

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices861="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:FileManager="http://www.superoffice.net/ws/crm/NetServer/Services86">
 <SOAP-ENV:Body>
  <FileManager:BeginReadFilePartResponse>
   <FileManager:FileName xsi:type="xsd:string"></FileManager:FileName>
   <FileManager:Length xsi:type="xsd:long">0</FileManager:Length>
  </FileManager:BeginReadFilePartResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```
