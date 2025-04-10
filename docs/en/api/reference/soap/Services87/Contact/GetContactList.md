---
title: Services87.ContactAgent.GetContactList SOAP
generated: 1
uid: Services87-Contact-GetContactList
---

# Services87 Contact GetContactList

SOAP request and response examples **Remote/Services87/Contact.svc**
Implemented by the <see cref="M:SuperOffice.Services87.IContactAgent.GetContactList">SuperOffice.Services87.IContactAgent.GetContactList</see> method.

## GetContactList

Gets an array of Contact objects.

* **contactIds:** The identifiers of the Contact object

**Returns:** Array of Contact objects

[WSDL file for Services87/Contact](../Services87-Contact.md)

Obtain a ticket from the [Services87/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## GetContactList Request

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices872="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices871="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Contact="http://www.superoffice.net/ws/crm/NetServer/Services87">
  <Contact:ApplicationToken>1234567-1234-9876</Contact:ApplicationToken>
  <Contact:Credentials>
    <Contact:Ticket>7T:1234abcxyzExample==</Contact:Ticket>
  </Contact:Credentials>
 <SOAP-ENV:Body>
   <Contact:GetContactList>
    <Contact:ContactIds xsi:type="NetServerServices872:ArrayOfint">
     <NetServerServices872:int xsi:type="xsd:int">0</NetServerServices872:int>
    </Contact:ContactIds>
   </Contact:GetContactList>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

## GetContactList Response

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices872="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices871="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Contact="http://www.superoffice.net/ws/crm/NetServer/Services87">
 <SOAP-ENV:Body>
  <Contact:GetContactListResponse>
   <Contact:Response xsi:type="Contact:ArrayOfContact">
    <Contact:Contact xsi:type="Contact:Contact">
     <Contact:ContactId xsi:type="xsd:int">0</Contact:ContactId>
     <Contact:Name xsi:type="xsd:string"></Contact:Name>
     <Contact:OrgNr xsi:type="xsd:string"></Contact:OrgNr>
     <Contact:Department xsi:type="xsd:string"></Contact:Department>
     <Contact:URL xsi:type="xsd:string"></Contact:URL>
     <Contact:City xsi:type="xsd:string"></Contact:City>
     <Contact:DirectPhone xsi:type="xsd:string"></Contact:DirectPhone>
     <Contact:AssociateId xsi:type="xsd:int">0</Contact:AssociateId>
     <Contact:CountryId xsi:type="xsd:int">0</Contact:CountryId>
     <Contact:EmailAddress xsi:type="xsd:string"></Contact:EmailAddress>
     <Contact:Kananame xsi:type="xsd:string"></Contact:Kananame>
     <Contact:EmailAddressName xsi:type="xsd:string"></Contact:EmailAddressName>
     <Contact:URLName xsi:type="xsd:string"></Contact:URLName>
     <Contact:AssociateFullName xsi:type="xsd:string"></Contact:AssociateFullName>
     <Contact:BusinessName xsi:type="xsd:string"></Contact:BusinessName>
     <Contact:CategoryName xsi:type="xsd:string"></Contact:CategoryName>
     <Contact:CountryName xsi:type="xsd:string"></Contact:CountryName>
     <Contact:Address xsi:type="Contact:Address">
      <Contact:Wgs84Latitude xsi:type="xsd:double">0.0</Contact:Wgs84Latitude>
      <Contact:Wgs84Longitude xsi:type="xsd:double">0.0</Contact:Wgs84Longitude>
      <Contact:LocalizedAddress xsi:type="Contact:ArrayOfArrayOfLocalizedField">
       <Contact:ArrayOfLocalizedField xsi:type="Contact:ArrayOfLocalizedField">
        <Contact:LocalizedField xsi:type="Contact:LocalizedField">
         <Contact:Name xsi:type="xsd:string"></Contact:Name>
         <Contact:Value xsi:type="xsd:string"></Contact:Value>
         <Contact:Tooltip xsi:type="xsd:string"></Contact:Tooltip>
         <Contact:Label xsi:type="xsd:string"></Contact:Label>
         <Contact:ValueLength xsi:type="xsd:int">0</Contact:ValueLength>
         <Contact:AddressType xsi:type="xsd:string"></Contact:AddressType>
        </Contact:LocalizedField>
       </Contact:ArrayOfLocalizedField>
      </Contact:LocalizedAddress>
      <Contact:Street xsi:type="Contact:StructuredAddress">
       <Contact:AtypeIdx xsi:type="Contact:AddressType">Unknown</Contact:AtypeIdx>
       <Contact:Address1 xsi:type="xsd:string"></Contact:Address1>
       <Contact:Address2 xsi:type="xsd:string"></Contact:Address2>
       <Contact:Address3 xsi:type="xsd:string"></Contact:Address3>
       <Contact:City xsi:type="xsd:string"></Contact:City>
       <Contact:County xsi:type="xsd:string"></Contact:County>
       <Contact:State xsi:type="xsd:string"></Contact:State>
       <Contact:Zipcode xsi:type="xsd:string"></Contact:Zipcode>
       <Contact:Formatted xsi:type="xsd:string"></Contact:Formatted>
      </Contact:Street>
      <Contact:Postal xsi:type="Contact:StructuredAddress">
       <Contact:AtypeIdx xsi:type="Contact:AddressType">Unknown</Contact:AtypeIdx>
       <Contact:Address1 xsi:type="xsd:string"></Contact:Address1>
       <Contact:Address2 xsi:type="xsd:string"></Contact:Address2>
       <Contact:Address3 xsi:type="xsd:string"></Contact:Address3>
       <Contact:City xsi:type="xsd:string"></Contact:City>
       <Contact:County xsi:type="xsd:string"></Contact:County>
       <Contact:State xsi:type="xsd:string"></Contact:State>
       <Contact:Zipcode xsi:type="xsd:string"></Contact:Zipcode>
       <Contact:Formatted xsi:type="xsd:string"></Contact:Formatted>
      </Contact:Postal>
      <Contact:Formatted xsi:type="xsd:string"></Contact:Formatted>
     </Contact:Address>
     <Contact:FormattedAddress xsi:type="xsd:string"></Contact:FormattedAddress>
     <Contact:FullName xsi:type="xsd:string"></Contact:FullName>
     <Contact:IsOwnerContact xsi:type="xsd:boolean">false</Contact:IsOwnerContact>
     <Contact:ActiveErpLinks xsi:type="xsd:int">0</Contact:ActiveErpLinks>
    </Contact:Contact>
   </Contact:Response>
  </Contact:GetContactListResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```
