---
title: Services87.ListAgent.ChangeCurrency SOAP
generated: 1
uid: Services87-List-ChangeCurrency
---

# Services87 List ChangeCurrency

SOAP request and response examples **Remote/Services87/List.svc**
Implemented by the <see cref="M:SuperOffice.Services87.IListAgent.ChangeCurrency">SuperOffice.Services87.IListAgent.ChangeCurrency</see> method.

## ChangeCurrency

Recalculates the amount to the new currency.

* **amount:** The amount in the old currency
* **fromCurrency:** The old currency name
* **toCurrency:** The new currency name

**Returns:** Amount in new currency

[WSDL file for Services87/List](../Services87-List.md)

Obtain a ticket from the [Services87/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## ChangeCurrency Request

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
   <List:ChangeCurrency>
    <List:Amount xsi:type="xsd:double">0.0</List:Amount>
    <List:FromCurrency xsi:type="xsd:string"></List:FromCurrency>
    <List:ToCurrency xsi:type="xsd:string"></List:ToCurrency>
   </List:ChangeCurrency>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

## ChangeCurrency Response

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
  <List:ChangeCurrencyResponse>
   <List:Response xsi:type="xsd:double">0.0</List:Response>
  </List:ChangeCurrencyResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```
