---
title: Services84.BLOBAgent.SetBlobStream SOAP
generated: 1
uid: Services84-BLOB-SetBlobStream
---

# Services84 BLOB SetBlobStream

SOAP request and response examples **Remote/Services84/BLOB.svc**
Implemented by the <see cref="M:SuperOffice.Services84.IBLOBAgent.SetBlobStream">SuperOffice.Services84.IBLOBAgent.SetBlobStream</see> method.

## SetBlobStream

Store a binary object from it's stream

* **blobEntityId:** Id of the BLOB entity object that the binary data should be stored to.
* **stream:** The binary object as a Stream

[WSDL file for Services84/BLOB](../Services84-BLOB.md)

Obtain a ticket from the [Services84/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## SetBlobStream Request

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices841="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:BLOB="http://www.superoffice.net/ws/crm/NetServer/Services84">
  <BLOB:ApplicationToken>1234567-1234-9876</BLOB:ApplicationToken>
  <BLOB:Credentials>
    <BLOB:Ticket>7T:1234abcxyzExample==</BLOB:Ticket>
  </BLOB:Credentials>
 <SOAP-ENV:Body>
   <BLOB:SetBlobStream>
    <BLOB:BlobEntityId xsi:type="xsd:int">0</BLOB:BlobEntityId>
    <BLOB:Stream xsi:type="xsd:base64Binary"></BLOB:Stream>
   </BLOB:SetBlobStream>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

## SetBlobStream Response

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices841="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:BLOB="http://www.superoffice.net/ws/crm/NetServer/Services84">
 <SOAP-ENV:Body>
  <BLOB:SetBlobStreamResponse>
  </BLOB:SetBlobStreamResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```
