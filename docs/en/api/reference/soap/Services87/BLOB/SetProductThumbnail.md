---
title: Services87.BLOBAgent.SetProductThumbnail SOAP
generated: 1
uid: Services87-BLOB-SetProductThumbnail
---

# Services87 BLOB SetProductThumbnail

SOAP request and response examples **Remote/Services87/BLOB.svc**
Implemented by the <see cref="M:SuperOffice.Services87.IBLOBAgent.SetProductThumbnail">SuperOffice.Services87.IBLOBAgent.SetProductThumbnail</see> method.

## SetProductThumbnail

Stores the product thumbnail that is displayed in the CRM application. The image is scaled down to max 200x200 pixels.

* **productId:** The project id of the product the image belongs to.
* **image:** The image that is stored on the product (System.Drawing.Image); scaled down to no more than 200x200

[WSDL file for Services87/BLOB](../Services87-BLOB.md)

Obtain a ticket from the [Services87/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## SetProductThumbnail Request

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices871="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:BLOB="http://www.superoffice.net/ws/crm/NetServer/Services87">
  <BLOB:ApplicationToken>1234567-1234-9876</BLOB:ApplicationToken>
  <BLOB:Credentials>
    <BLOB:Ticket>7T:1234abcxyzExample==</BLOB:Ticket>
  </BLOB:Credentials>
 <SOAP-ENV:Body>
   <BLOB:SetProductThumbnail>
    <BLOB:ProductId xsi:type="xsd:int">0</BLOB:ProductId>
    <BLOB:Image xsi:type="xsd:base64Binary"></BLOB:Image>
   </BLOB:SetProductThumbnail>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

## SetProductThumbnail Response

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices871="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:BLOB="http://www.superoffice.net/ws/crm/NetServer/Services87">
 <SOAP-ENV:Body>
  <BLOB:SetProductThumbnailResponse>
  </BLOB:SetProductThumbnailResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```
