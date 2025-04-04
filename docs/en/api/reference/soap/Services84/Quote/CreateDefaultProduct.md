---
title: Services84.QuoteAgent.CreateDefaultProduct SOAP
generated: 1
uid: Services84-Quote-CreateDefaultProduct
---

# Services84 Quote CreateDefaultProduct

SOAP request and response examples **Remote/Services84/Quote.svc**
Implemented by the <see cref="M:SuperOffice.Services84.IQuoteAgent.CreateDefaultProduct">SuperOffice.Services84.IQuoteAgent.CreateDefaultProduct</see> method.

## CreateDefaultProduct

Loading default values into a new Product.
NetServer calculates default values (e.g. Country) on the entity, which is required when creating/storing a new instance

**Returns:** New Product with default values

[WSDL file for Services84/Quote](../Services84-Quote.md)

Obtain a ticket from the [Services84/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## CreateDefaultProduct Request

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices842="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices841="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Quote="http://www.superoffice.net/ws/crm/NetServer/Services84">
  <Quote:ApplicationToken>1234567-1234-9876</Quote:ApplicationToken>
  <Quote:Credentials>
    <Quote:Ticket>7T:1234abcxyzExample==</Quote:Ticket>
  </Quote:Credentials>
 <SOAP-ENV:Body>
   <Quote:CreateDefaultProduct>
   </Quote:CreateDefaultProduct>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

## CreateDefaultProduct Response

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices842="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices841="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Quote="http://www.superoffice.net/ws/crm/NetServer/Services84">
 <SOAP-ENV:Body>
  <Quote:CreateDefaultProductResponse>
   <Quote:Response xsi:type="Quote:Product">
    <Quote:ProductId xsi:type="xsd:int">0</Quote:ProductId>
    <Quote:ERPProductKey xsi:type="xsd:string"></Quote:ERPProductKey>
    <Quote:ERPPriceListKey xsi:type="xsd:string"></Quote:ERPPriceListKey>
    <Quote:Name xsi:type="xsd:string"></Quote:Name>
    <Quote:Description xsi:type="xsd:string"></Quote:Description>
    <Quote:Code xsi:type="xsd:string"></Quote:Code>
    <Quote:PriceUnit xsi:type="xsd:string"></Quote:PriceUnit>
    <Quote:QuantityUnit xsi:type="xsd:string"></Quote:QuantityUnit>
    <Quote:IsSubscription xsi:type="xsd:boolean">false</Quote:IsSubscription>
    <Quote:SubscriptionUnit xsi:type="xsd:string"></Quote:SubscriptionUnit>
    <Quote:DefaultSubscriptionQuantity xsi:type="xsd:double">0.0</Quote:DefaultSubscriptionQuantity>
    <Quote:ItemNumber xsi:type="xsd:string"></Quote:ItemNumber>
    <Quote:Url xsi:type="xsd:string"></Quote:Url>
    <Quote:ProductCategoryKey xsi:type="xsd:string"></Quote:ProductCategoryKey>
    <Quote:ProductFamilyKey xsi:type="xsd:string"></Quote:ProductFamilyKey>
    <Quote:ProductTypeKey xsi:type="xsd:string"></Quote:ProductTypeKey>
    <Quote:VAT xsi:type="xsd:double">0.0</Quote:VAT>
    <Quote:VATInfo xsi:type="xsd:string"></Quote:VATInfo>
    <Quote:UnitCost xsi:type="xsd:double">0.0</Quote:UnitCost>
    <Quote:UnitMinimumPrice xsi:type="xsd:double">0.0</Quote:UnitMinimumPrice>
    <Quote:UnitListPrice xsi:type="xsd:double">0.0</Quote:UnitListPrice>
    <Quote:InAssortment xsi:type="xsd:boolean">false</Quote:InAssortment>
    <Quote:Supplier xsi:type="xsd:string"></Quote:Supplier>
    <Quote:SupplierCode xsi:type="xsd:string"></Quote:SupplierCode>
    <Quote:Rights xsi:type="xsd:string"></Quote:Rights>
    <Quote:Rule xsi:type="xsd:string"></Quote:Rule>
    <Quote:ExtraInfo xsi:type="Quote:ArrayOfProductExtraDataField">
     <Quote:ProductExtraDataField xsi:type="Quote:ProductExtraDataField">
      <Quote:Name xsi:type="xsd:string"></Quote:Name>
      <Quote:Value xsi:type="xsd:string"></Quote:Value>
      <Quote:Type xsi:type="Quote:ExtraDataFieldType">String</Quote:Type>
     </Quote:ProductExtraDataField>
    </Quote:ExtraInfo>
    <Quote:RawExtraInfo xsi:type="xsd:string"></Quote:RawExtraInfo>
    <Quote:ExtraField1 xsi:type="xsd:string"></Quote:ExtraField1>
    <Quote:ExtraField2 xsi:type="xsd:string"></Quote:ExtraField2>
    <Quote:ExtraField3 xsi:type="xsd:string"></Quote:ExtraField3>
    <Quote:ExtraField4 xsi:type="xsd:string"></Quote:ExtraField4>
    <Quote:ExtraField5 xsi:type="xsd:string"></Quote:ExtraField5>
    <Quote:InStock xsi:type="xsd:double">0.0</Quote:InStock>
   </Quote:Response>
  </Quote:CreateDefaultProductResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```
