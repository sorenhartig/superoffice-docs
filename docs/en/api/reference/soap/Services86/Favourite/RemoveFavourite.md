---
title: Services86.FavouriteAgent.RemoveFavourite SOAP
generated: 1
uid: Services86-Favourite-RemoveFavourite
---

# Services86 Favourite RemoveFavourite

SOAP request and response examples **Remote/Services86/Favourite.svc**
Implemented by the <see cref="M:SuperOffice.Services86.IFavouriteAgent.RemoveFavourite">SuperOffice.Services86.IFavouriteAgent.RemoveFavourite</see> method.

## RemoveFavourite

Remove favourite for a table, record id and associate

* **tableName:** Table name, transformed to and from numeric table id by the service layer.
* **recordId:**
* **associateId:**

[WSDL file for Services86/Favourite](../Services86-Favourite.md)

Obtain a ticket from the [Services86/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## RemoveFavourite Request

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices862="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices861="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Favourite="http://www.superoffice.net/ws/crm/NetServer/Services86">
  <Favourite:ApplicationToken>1234567-1234-9876</Favourite:ApplicationToken>
  <Favourite:Credentials>
    <Favourite:Ticket>7T:1234abcxyzExample==</Favourite:Ticket>
  </Favourite:Credentials>
 <SOAP-ENV:Body>
   <Favourite:RemoveFavourite>
    <Favourite:TableName xsi:type="xsd:string"></Favourite:TableName>
    <Favourite:RecordId xsi:type="xsd:int">0</Favourite:RecordId>
    <Favourite:AssociateId xsi:type="xsd:int">0</Favourite:AssociateId>
   </Favourite:RemoveFavourite>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

## RemoveFavourite Response

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices862="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices861="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Favourite="http://www.superoffice.net/ws/crm/NetServer/Services86">
 <SOAP-ENV:Body>
  <Favourite:RemoveFavouriteResponse>
  </Favourite:RemoveFavouriteResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```
