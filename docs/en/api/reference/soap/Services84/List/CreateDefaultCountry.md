---
title: Services84.ListAgent.CreateDefaultCountry SOAP
generated: 1
uid: Services84-List-CreateDefaultCountry
---

# Services84 List CreateDefaultCountry

SOAP request and response examples **Remote/Services84/List.svc**
Implemented by the <see cref="M:SuperOffice.Services84.IListAgent.CreateDefaultCountry">SuperOffice.Services84.IListAgent.CreateDefaultCountry</see> method.

## CreateDefaultCountry

Gets a new country

**Returns:** A new country with default values

[WSDL file for Services84/List](../Services84-List.md)

Obtain a ticket from the [Services84/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## CreateDefaultCountry Request

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
   <List:CreateDefaultCountry>
   </List:CreateDefaultCountry>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

## CreateDefaultCountry Response

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
  <List:CreateDefaultCountryResponse>
   <List:Response xsi:type="List:Country">
    <List:CountryId xsi:type="xsd:int">0</List:CountryId>
    <List:Name xsi:type="xsd:string"></List:Name>
    <List:CurrencyId xsi:type="xsd:int">0</List:CurrencyId>
    <List:EnglishName xsi:type="xsd:string"></List:EnglishName>
    <List:TwoLetterISOCountry xsi:type="xsd:string"></List:TwoLetterISOCountry>
    <List:ThreeLetterISOCountry xsi:type="xsd:string"></List:ThreeLetterISOCountry>
    <List:ImageDescription xsi:type="xsd:string"></List:ImageDescription>
    <List:OrgNrText xsi:type="xsd:string"></List:OrgNrText>
    <List:InterAreaPrefix xsi:type="xsd:string"></List:InterAreaPrefix>
    <List:DialInPrefix xsi:type="xsd:string"></List:DialInPrefix>
    <List:ZipPrefix xsi:type="xsd:string"></List:ZipPrefix>
    <List:DomainName xsi:type="xsd:string"></List:DomainName>
    <List:AddressLayoutId xsi:type="xsd:int">0</List:AddressLayoutId>
    <List:DomesticAddressLayoutId xsi:type="xsd:int">0</List:DomesticAddressLayoutId>
    <List:ForeignAddressLayoutId xsi:type="xsd:int">0</List:ForeignAddressLayoutId>
    <List:Rank xsi:type="xsd:short">0</List:Rank>
    <List:Tooltip xsi:type="xsd:string"></List:Tooltip>
    <List:Deleted xsi:type="xsd:boolean">false</List:Deleted>
   </List:Response>
  </List:CreateDefaultCountryResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```
