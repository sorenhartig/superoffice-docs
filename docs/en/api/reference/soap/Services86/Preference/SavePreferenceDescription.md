---
title: Services86.PreferenceAgent.SavePreferenceDescription SOAP
generated: 1
uid: Services86-Preference-SavePreferenceDescription
---

# Services86 Preference SavePreferenceDescription

SOAP request and response examples **Remote/Services86/Preference.svc**
Implemented by the <see cref="M:SuperOffice.Services86.IPreferenceAgent.SavePreferenceDescription">SuperOffice.Services86.IPreferenceAgent.SavePreferenceDescription</see> method.

## SavePreferenceDescription

Updates the existing PreferenceDescription or creates a new PreferenceDescription if the id parameter is 0.

* **preferenceDescription:** The PreferenceDescription that is saved.

**Returns:** New or updated PreferenceDescription

[WSDL file for Services86/Preference](../Services86-Preference.md)

Obtain a ticket from the [Services86/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## SavePreferenceDescription Request

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices862="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices861="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Preference="http://www.superoffice.net/ws/crm/NetServer/Services86">
  <Preference:ApplicationToken>1234567-1234-9876</Preference:ApplicationToken>
  <Preference:Credentials>
    <Preference:Ticket>7T:1234abcxyzExample==</Preference:Ticket>
  </Preference:Credentials>
 <SOAP-ENV:Body>
   <Preference:SavePreferenceDescription>
    <Preference:PreferenceDescription xsi:type="Preference:PreferenceDescription">
     <Preference:PrefDescId xsi:type="xsd:int">0</Preference:PrefDescId>
     <Preference:Section xsi:type="xsd:string"></Preference:Section>
     <Preference:Key xsi:type="xsd:string"></Preference:Key>
     <Preference:Name xsi:type="xsd:string"></Preference:Name>
     <Preference:ValueType xsi:type="Preference:PrefDescValueType">Unknown</Preference:ValueType>
     <Preference:MaxLevel xsi:type="Preference:PreferenceLevel">Undefined</Preference:MaxLevel>
     <Preference:SysMaxLevel xsi:type="Preference:PreferenceLevel">Undefined</Preference:SysMaxLevel>
     <Preference:AccessFlags xsi:type="Preference:PrefDescAccessFlags">WizardMode</Preference:AccessFlags>
     <Preference:Description xsi:type="xsd:string"></Preference:Description>
     <Preference:IsBuiltin xsi:type="xsd:boolean">false</Preference:IsBuiltin>
     <Preference:TableName xsi:type="xsd:string"></Preference:TableName>
     <Preference:UserDefinedListId xsi:type="xsd:int">0</Preference:UserDefinedListId>
    </Preference:PreferenceDescription>
   </Preference:SavePreferenceDescription>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

## SavePreferenceDescription Response

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices862="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices861="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Preference="http://www.superoffice.net/ws/crm/NetServer/Services86">
 <SOAP-ENV:Body>
  <Preference:SavePreferenceDescriptionResponse>
   <Preference:Response xsi:type="Preference:PreferenceDescription">
    <Preference:PrefDescId xsi:type="xsd:int">0</Preference:PrefDescId>
    <Preference:Section xsi:type="xsd:string"></Preference:Section>
    <Preference:Key xsi:type="xsd:string"></Preference:Key>
    <Preference:Name xsi:type="xsd:string"></Preference:Name>
    <Preference:ValueType xsi:type="Preference:PrefDescValueType">Unknown</Preference:ValueType>
    <Preference:MaxLevel xsi:type="Preference:PreferenceLevel">Undefined</Preference:MaxLevel>
    <Preference:SysMaxLevel xsi:type="Preference:PreferenceLevel">Undefined</Preference:SysMaxLevel>
    <Preference:AccessFlags xsi:type="Preference:PrefDescAccessFlags">WizardMode</Preference:AccessFlags>
    <Preference:Description xsi:type="xsd:string"></Preference:Description>
    <Preference:IsBuiltin xsi:type="xsd:boolean">false</Preference:IsBuiltin>
    <Preference:TableName xsi:type="xsd:string"></Preference:TableName>
    <Preference:UserDefinedListId xsi:type="xsd:int">0</Preference:UserDefinedListId>
   </Preference:Response>
  </Preference:SavePreferenceDescriptionResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```
