---
title: Services84.LicenseAgent.GetSatelliteLicenses SOAP
generated: 1
uid: Services84-License-GetSatelliteLicenses
---

# Services84 License GetSatelliteLicenses

SOAP request and response examples **Remote/Services84/License.svc**
Implemented by the <see cref="M:SuperOffice.Services84.ILicenseAgent.GetSatelliteLicenses">SuperOffice.Services84.ILicenseAgent.GetSatelliteLicenses</see> method.

## GetSatelliteLicenses

Obtain information about satellite module licenses

* **satelliteId:** Satellite id to check for satellite module licenses

**Returns:** Satellite module licenses grouped by owners.

[WSDL file for Services84/License](../Services84-License.md)

Obtain a ticket from the [Services84/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## GetSatelliteLicenses Request

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices842="http://schemas.datacontract.org/2004/07/System.Security.Cryptography"
 xmlns:NetServerServices843="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices841="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:License="http://www.superoffice.net/ws/crm/NetServer/Services84">
  <License:ApplicationToken>1234567-1234-9876</License:ApplicationToken>
  <License:Credentials>
    <License:Ticket>7T:1234abcxyzExample==</License:Ticket>
  </License:Credentials>
 <SOAP-ENV:Body>
   <License:GetSatelliteLicenses>
    <License:SatelliteId xsi:type="xsd:int">0</License:SatelliteId>
   </License:GetSatelliteLicenses>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

## GetSatelliteLicenses Response

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices842="http://schemas.datacontract.org/2004/07/System.Security.Cryptography"
 xmlns:NetServerServices843="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices841="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:License="http://www.superoffice.net/ws/crm/NetServer/Services84">
 <SOAP-ENV:Body>
  <License:GetSatelliteLicensesResponse>
   <License:Response xsi:type="License:ArrayOfLicenseOwner">
    <License:LicenseOwner xsi:type="License:LicenseOwner">
     <License:Name xsi:type="xsd:string"></License:Name>
     <License:Description xsi:type="xsd:string"></License:Description>
     <License:RestrictedModuleLicenses xsi:type="License:ArrayOfModuleLicenseLink">
      <License:ModuleLicenseLink xsi:type="License:ModuleLicenseLink">
       <License:Unrestricted xsi:type="xsd:boolean">false</License:Unrestricted>
       <License:Total xsi:type="xsd:int">0</License:Total>
       <License:Tooltip xsi:type="xsd:string"></License:Tooltip>
       <License:CanAssign xsi:type="xsd:boolean">false</License:CanAssign>
       <License:Free xsi:type="xsd:int">0</License:Free>
       <License:InUse xsi:type="xsd:int">0</License:InUse>
       <License:Assigned xsi:type="xsd:boolean">false</License:Assigned>
       <License:ModuleLicenseId xsi:type="xsd:int">0</License:ModuleLicenseId>
       <License:Name xsi:type="xsd:string"></License:Name>
       <License:Description xsi:type="xsd:string"></License:Description>
       <License:PrerequisiteModuleName xsi:type="xsd:string"></License:PrerequisiteModuleName>
       <License:SortOrder xsi:type="xsd:int">0</License:SortOrder>
      </License:ModuleLicenseLink>
     </License:RestrictedModuleLicenses>
     <License:UnrestrictedModuleLicenses xsi:type="License:ArrayOfModuleLicenseLink">
      <License:ModuleLicenseLink xsi:type="License:ModuleLicenseLink">
       <License:Unrestricted xsi:type="xsd:boolean">false</License:Unrestricted>
       <License:Total xsi:type="xsd:int">0</License:Total>
       <License:Tooltip xsi:type="xsd:string"></License:Tooltip>
       <License:CanAssign xsi:type="xsd:boolean">false</License:CanAssign>
       <License:Free xsi:type="xsd:int">0</License:Free>
       <License:InUse xsi:type="xsd:int">0</License:InUse>
       <License:Assigned xsi:type="xsd:boolean">false</License:Assigned>
       <License:ModuleLicenseId xsi:type="xsd:int">0</License:ModuleLicenseId>
       <License:Name xsi:type="xsd:string"></License:Name>
       <License:Description xsi:type="xsd:string"></License:Description>
       <License:PrerequisiteModuleName xsi:type="xsd:string"></License:PrerequisiteModuleName>
       <License:SortOrder xsi:type="xsd:int">0</License:SortOrder>
      </License:ModuleLicenseLink>
     </License:UnrestrictedModuleLicenses>
    </License:LicenseOwner>
   </License:Response>
  </License:GetSatelliteLicensesResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```
