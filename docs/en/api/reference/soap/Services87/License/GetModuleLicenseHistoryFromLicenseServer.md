---
title: Services87.LicenseAgent.GetModuleLicenseHistoryFromLicenseServer SOAP
generated: 1
uid: Services87-License-GetModuleLicenseHistoryFromLicenseServer
---

# Services87 License GetModuleLicenseHistoryFromLicenseServer

SOAP request and response examples **Remote/Services87/License.svc**
Implemented by the <see cref="M:SuperOffice.Services87.ILicenseAgent.GetModuleLicenseHistoryFromLicenseServer">SuperOffice.Services87.ILicenseAgent.GetModuleLicenseHistoryFromLicenseServer</see> method.

## GetModuleLicenseHistoryFromLicenseServer

Get details about a license from the license server.

* **licenseInfo:** Description of the license
* **moduleLicense:** Information about a particular module to get information for.

**Returns:** Information about a particular license module.

[WSDL file for Services87/License](../Services87-License.md)

Obtain a ticket from the [Services87/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## GetModuleLicenseHistoryFromLicenseServer Request

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices872="http://schemas.datacontract.org/2004/07/System.Security.Cryptography"
 xmlns:NetServerServices873="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices871="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:License="http://www.superoffice.net/ws/crm/NetServer/Services87">
  <License:ApplicationToken>1234567-1234-9876</License:ApplicationToken>
  <License:Credentials>
    <License:Ticket>7T:1234abcxyzExample==</License:Ticket>
  </License:Credentials>
 <SOAP-ENV:Body>
   <License:GetModuleLicenseHistoryFromLicenseServer>
    <License:LicenseInfo xsi:type="License:ExtendedLicenseInfo">
     <License:Reason xsi:type="xsd:string"></License:Reason>
     <License:CanBeActivated xsi:type="xsd:boolean">false</License:CanBeActivated>
     <License:New xsi:type="License:LicenseInfo">
      <License:CompanyName xsi:type="xsd:string"></License:CompanyName>
      <License:SerialNr xsi:type="xsd:string"></License:SerialNr>
      <License:OwnerName xsi:type="xsd:string"></License:OwnerName>
      <License:OwnerDescription xsi:type="xsd:string"></License:OwnerDescription>
      <License:NextCheckDate xsi:type="xsd:dateTime">2022-08-26T08:57:15Z</License:NextCheckDate>
      <License:MaintenanceDate xsi:type="xsd:dateTime">2022-08-26T08:57:15Z</License:MaintenanceDate>
      <License:AdminWarningDate xsi:type="xsd:dateTime">2022-08-26T08:57:15Z</License:AdminWarningDate>
      <License:ExpiryDate xsi:type="xsd:dateTime">2022-08-26T08:57:15Z</License:ExpiryDate>
      <License:GraceDate xsi:type="xsd:dateTime">2022-08-26T08:57:15Z</License:GraceDate>
      <License:ExtraFlags xsi:type="xsd:int">0</License:ExtraFlags>
      <License:LicenseUrl xsi:type="xsd:string"></License:LicenseUrl>
      <License:LicenseVersion xsi:type="xsd:string"></License:LicenseVersion>
      <License:DeploymentType xsi:type="xsd:int">0</License:DeploymentType>
      <License:ProductType xsi:type="xsd:string"></License:ProductType>
      <License:ProductDescription xsi:type="xsd:string"></License:ProductDescription>
      <License:ModuleLicenses xsi:type="License:ArrayOfModuleLicense">
       <License:ModuleLicense xsi:type="License:ModuleLicense">
        <License:OwnerName xsi:type="xsd:string"></License:OwnerName>
        <License:ModuleName xsi:type="xsd:string"></License:ModuleName>
        <License:ModuleDescription xsi:type="xsd:string"></License:ModuleDescription>
        <License:ModuleTooltip xsi:type="xsd:string"></License:ModuleTooltip>
        <License:ModuleVersion xsi:type="xsd:string"></License:ModuleVersion>
        <License:LicenseType xsi:type="License:LicenseType">Unknown</License:LicenseType>
        <License:Unrestricted xsi:type="xsd:boolean">false</License:Unrestricted>
        <License:AllowedUserType xsi:type="License:UserType">Unknown</License:AllowedUserType>
        <License:NumberOfLicenses xsi:type="xsd:int">0</License:NumberOfLicenses>
        <License:ExtraFlags xsi:type="xsd:int">0</License:ExtraFlags>
        <License:ExtraInfo xsi:type="xsd:string"></License:ExtraInfo>
        <License:SortOrder xsi:type="xsd:int">0</License:SortOrder>
        <License:IsHidden xsi:type="xsd:boolean">false</License:IsHidden>
        <License:PrerequisiteModuleName xsi:type="xsd:string"></License:PrerequisiteModuleName>
        <License:Signature xsi:type="xsd:string"></License:Signature>
       </License:ModuleLicense>
      </License:ModuleLicenses>
      <License:PublicKey xsi:type="License:SignedPublicKey">
       <License:OwnerName xsi:type="xsd:string"></License:OwnerName>
       <License:SignDate xsi:type="xsd:dateTime">2022-08-26T08:57:15Z</License:SignDate>
       <License:ExpiryDate xsi:type="xsd:dateTime">2022-08-26T08:57:15Z</License:ExpiryDate>
       <License:Key xsi:type="NetServerServices872:DSAParameters">
        <NetServerServices872:Counter xsi:type="xsd:int">0</NetServerServices872:Counter>
        <NetServerServices872:G xsi:type="xsd:base64Binary"></NetServerServices872:G>
        <NetServerServices872:J xsi:type="xsd:base64Binary"></NetServerServices872:J>
        <NetServerServices872:P xsi:type="xsd:base64Binary"></NetServerServices872:P>
        <NetServerServices872:Q xsi:type="xsd:base64Binary"></NetServerServices872:Q>
        <NetServerServices872:Seed xsi:type="xsd:base64Binary"></NetServerServices872:Seed>
        <NetServerServices872:Y xsi:type="xsd:base64Binary"></NetServerServices872:Y>
       </License:Key>
       <License:Signature xsi:type="xsd:string"></License:Signature>
      </License:PublicKey>
      <License:Signature xsi:type="xsd:string"></License:Signature>
     </License:New>
     <License:Current xsi:type="License:LicenseInfo">
      <License:CompanyName xsi:type="xsd:string"></License:CompanyName>
      <License:SerialNr xsi:type="xsd:string"></License:SerialNr>
      <License:OwnerName xsi:type="xsd:string"></License:OwnerName>
      <License:OwnerDescription xsi:type="xsd:string"></License:OwnerDescription>
      <License:NextCheckDate xsi:type="xsd:dateTime">2022-08-26T08:57:15Z</License:NextCheckDate>
      <License:MaintenanceDate xsi:type="xsd:dateTime">2022-08-26T08:57:15Z</License:MaintenanceDate>
      <License:AdminWarningDate xsi:type="xsd:dateTime">2022-08-26T08:57:15Z</License:AdminWarningDate>
      <License:ExpiryDate xsi:type="xsd:dateTime">2022-08-26T08:57:15Z</License:ExpiryDate>
      <License:GraceDate xsi:type="xsd:dateTime">2022-08-26T08:57:15Z</License:GraceDate>
      <License:ExtraFlags xsi:type="xsd:int">0</License:ExtraFlags>
      <License:LicenseUrl xsi:type="xsd:string"></License:LicenseUrl>
      <License:LicenseVersion xsi:type="xsd:string"></License:LicenseVersion>
      <License:DeploymentType xsi:type="xsd:int">0</License:DeploymentType>
      <License:ProductType xsi:type="xsd:string"></License:ProductType>
      <License:ProductDescription xsi:type="xsd:string"></License:ProductDescription>
      <License:ModuleLicenses xsi:type="License:ArrayOfModuleLicense">
       <License:ModuleLicense xsi:type="License:ModuleLicense">
        <License:OwnerName xsi:type="xsd:string"></License:OwnerName>
        <License:ModuleName xsi:type="xsd:string"></License:ModuleName>
        <License:ModuleDescription xsi:type="xsd:string"></License:ModuleDescription>
        <License:ModuleTooltip xsi:type="xsd:string"></License:ModuleTooltip>
        <License:ModuleVersion xsi:type="xsd:string"></License:ModuleVersion>
        <License:LicenseType xsi:type="License:LicenseType">Unknown</License:LicenseType>
        <License:Unrestricted xsi:type="xsd:boolean">false</License:Unrestricted>
        <License:AllowedUserType xsi:type="License:UserType">Unknown</License:AllowedUserType>
        <License:NumberOfLicenses xsi:type="xsd:int">0</License:NumberOfLicenses>
        <License:ExtraFlags xsi:type="xsd:int">0</License:ExtraFlags>
        <License:ExtraInfo xsi:type="xsd:string"></License:ExtraInfo>
        <License:SortOrder xsi:type="xsd:int">0</License:SortOrder>
        <License:IsHidden xsi:type="xsd:boolean">false</License:IsHidden>
        <License:PrerequisiteModuleName xsi:type="xsd:string"></License:PrerequisiteModuleName>
        <License:Signature xsi:type="xsd:string"></License:Signature>
       </License:ModuleLicense>
      </License:ModuleLicenses>
      <License:PublicKey xsi:type="License:SignedPublicKey">
       <License:OwnerName xsi:type="xsd:string"></License:OwnerName>
       <License:SignDate xsi:type="xsd:dateTime">2022-08-26T08:57:15Z</License:SignDate>
       <License:ExpiryDate xsi:type="xsd:dateTime">2022-08-26T08:57:15Z</License:ExpiryDate>
       <License:Key xsi:type="NetServerServices872:DSAParameters">
        <NetServerServices872:Counter xsi:type="xsd:int">0</NetServerServices872:Counter>
        <NetServerServices872:G xsi:type="xsd:base64Binary"></NetServerServices872:G>
        <NetServerServices872:J xsi:type="xsd:base64Binary"></NetServerServices872:J>
        <NetServerServices872:P xsi:type="xsd:base64Binary"></NetServerServices872:P>
        <NetServerServices872:Q xsi:type="xsd:base64Binary"></NetServerServices872:Q>
        <NetServerServices872:Seed xsi:type="xsd:base64Binary"></NetServerServices872:Seed>
        <NetServerServices872:Y xsi:type="xsd:base64Binary"></NetServerServices872:Y>
       </License:Key>
       <License:Signature xsi:type="xsd:string"></License:Signature>
      </License:PublicKey>
      <License:Signature xsi:type="xsd:string"></License:Signature>
     </License:Current>
     <License:ExtendedModuleLicenses xsi:type="License:ArrayOfExtendedModuleLicense">
      <License:ExtendedModuleLicense xsi:type="License:ExtendedModuleLicense">
       <License:New xsi:type="License:ModuleLicense">
        <License:OwnerName xsi:type="xsd:string"></License:OwnerName>
        <License:ModuleName xsi:type="xsd:string"></License:ModuleName>
        <License:ModuleDescription xsi:type="xsd:string"></License:ModuleDescription>
        <License:ModuleTooltip xsi:type="xsd:string"></License:ModuleTooltip>
        <License:ModuleVersion xsi:type="xsd:string"></License:ModuleVersion>
        <License:LicenseType xsi:type="License:LicenseType">Unknown</License:LicenseType>
        <License:Unrestricted xsi:type="xsd:boolean">false</License:Unrestricted>
        <License:AllowedUserType xsi:type="License:UserType">Unknown</License:AllowedUserType>
        <License:NumberOfLicenses xsi:type="xsd:int">0</License:NumberOfLicenses>
        <License:ExtraFlags xsi:type="xsd:int">0</License:ExtraFlags>
        <License:ExtraInfo xsi:type="xsd:string"></License:ExtraInfo>
        <License:SortOrder xsi:type="xsd:int">0</License:SortOrder>
        <License:IsHidden xsi:type="xsd:boolean">false</License:IsHidden>
        <License:PrerequisiteModuleName xsi:type="xsd:string"></License:PrerequisiteModuleName>
        <License:Signature xsi:type="xsd:string"></License:Signature>
       </License:New>
       <License:Current xsi:type="License:ModuleLicense">
        <License:OwnerName xsi:type="xsd:string"></License:OwnerName>
        <License:ModuleName xsi:type="xsd:string"></License:ModuleName>
        <License:ModuleDescription xsi:type="xsd:string"></License:ModuleDescription>
        <License:ModuleTooltip xsi:type="xsd:string"></License:ModuleTooltip>
        <License:ModuleVersion xsi:type="xsd:string"></License:ModuleVersion>
        <License:LicenseType xsi:type="License:LicenseType">Unknown</License:LicenseType>
        <License:Unrestricted xsi:type="xsd:boolean">false</License:Unrestricted>
        <License:AllowedUserType xsi:type="License:UserType">Unknown</License:AllowedUserType>
        <License:NumberOfLicenses xsi:type="xsd:int">0</License:NumberOfLicenses>
        <License:ExtraFlags xsi:type="xsd:int">0</License:ExtraFlags>
        <License:ExtraInfo xsi:type="xsd:string"></License:ExtraInfo>
        <License:SortOrder xsi:type="xsd:int">0</License:SortOrder>
        <License:IsHidden xsi:type="xsd:boolean">false</License:IsHidden>
        <License:PrerequisiteModuleName xsi:type="xsd:string"></License:PrerequisiteModuleName>
        <License:Signature xsi:type="xsd:string"></License:Signature>
       </License:Current>
       <License:NumberOfLicensesInUse xsi:type="xsd:int">0</License:NumberOfLicensesInUse>
       <License:NumberOfLicensesFree xsi:type="xsd:int">0</License:NumberOfLicensesFree>
       <License:NumberOfLicensesAdded xsi:type="xsd:int">0</License:NumberOfLicensesAdded>
       <License:NumberOfLicensesNewTotal xsi:type="xsd:int">0</License:NumberOfLicensesNewTotal>
       <License:NumberOfLicensesNewFree xsi:type="xsd:int">0</License:NumberOfLicensesNewFree>
       <License:NumberOfLicensesTotal xsi:type="xsd:int">0</License:NumberOfLicensesTotal>
      </License:ExtendedModuleLicense>
     </License:ExtendedModuleLicenses>
     <License:AccumulatedNextCheckDate xsi:type="xsd:dateTime">2022-08-26T08:57:15Z</License:AccumulatedNextCheckDate>
    </License:LicenseInfo>
    <License:ModuleLicense xsi:type="License:ExtendedModuleLicense">
     <License:New xsi:type="License:ModuleLicense">
      <License:OwnerName xsi:type="xsd:string"></License:OwnerName>
      <License:ModuleName xsi:type="xsd:string"></License:ModuleName>
      <License:ModuleDescription xsi:type="xsd:string"></License:ModuleDescription>
      <License:ModuleTooltip xsi:type="xsd:string"></License:ModuleTooltip>
      <License:ModuleVersion xsi:type="xsd:string"></License:ModuleVersion>
      <License:LicenseType xsi:type="License:LicenseType">Unknown</License:LicenseType>
      <License:Unrestricted xsi:type="xsd:boolean">false</License:Unrestricted>
      <License:AllowedUserType xsi:type="License:UserType">Unknown</License:AllowedUserType>
      <License:NumberOfLicenses xsi:type="xsd:int">0</License:NumberOfLicenses>
      <License:ExtraFlags xsi:type="xsd:int">0</License:ExtraFlags>
      <License:ExtraInfo xsi:type="xsd:string"></License:ExtraInfo>
      <License:SortOrder xsi:type="xsd:int">0</License:SortOrder>
      <License:IsHidden xsi:type="xsd:boolean">false</License:IsHidden>
      <License:PrerequisiteModuleName xsi:type="xsd:string"></License:PrerequisiteModuleName>
      <License:Signature xsi:type="xsd:string"></License:Signature>
     </License:New>
     <License:Current xsi:type="License:ModuleLicense">
      <License:OwnerName xsi:type="xsd:string"></License:OwnerName>
      <License:ModuleName xsi:type="xsd:string"></License:ModuleName>
      <License:ModuleDescription xsi:type="xsd:string"></License:ModuleDescription>
      <License:ModuleTooltip xsi:type="xsd:string"></License:ModuleTooltip>
      <License:ModuleVersion xsi:type="xsd:string"></License:ModuleVersion>
      <License:LicenseType xsi:type="License:LicenseType">Unknown</License:LicenseType>
      <License:Unrestricted xsi:type="xsd:boolean">false</License:Unrestricted>
      <License:AllowedUserType xsi:type="License:UserType">Unknown</License:AllowedUserType>
      <License:NumberOfLicenses xsi:type="xsd:int">0</License:NumberOfLicenses>
      <License:ExtraFlags xsi:type="xsd:int">0</License:ExtraFlags>
      <License:ExtraInfo xsi:type="xsd:string"></License:ExtraInfo>
      <License:SortOrder xsi:type="xsd:int">0</License:SortOrder>
      <License:IsHidden xsi:type="xsd:boolean">false</License:IsHidden>
      <License:PrerequisiteModuleName xsi:type="xsd:string"></License:PrerequisiteModuleName>
      <License:Signature xsi:type="xsd:string"></License:Signature>
     </License:Current>
     <License:NumberOfLicensesInUse xsi:type="xsd:int">0</License:NumberOfLicensesInUse>
     <License:NumberOfLicensesFree xsi:type="xsd:int">0</License:NumberOfLicensesFree>
     <License:NumberOfLicensesAdded xsi:type="xsd:int">0</License:NumberOfLicensesAdded>
     <License:NumberOfLicensesNewTotal xsi:type="xsd:int">0</License:NumberOfLicensesNewTotal>
     <License:NumberOfLicensesNewFree xsi:type="xsd:int">0</License:NumberOfLicensesNewFree>
     <License:NumberOfLicensesTotal xsi:type="xsd:int">0</License:NumberOfLicensesTotal>
    </License:ModuleLicense>
   </License:GetModuleLicenseHistoryFromLicenseServer>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

## GetModuleLicenseHistoryFromLicenseServer Response

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices872="http://schemas.datacontract.org/2004/07/System.Security.Cryptography"
 xmlns:NetServerServices873="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices871="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:License="http://www.superoffice.net/ws/crm/NetServer/Services87">
 <SOAP-ENV:Body>
  <License:GetModuleLicenseHistoryFromLicenseServerResponse>
   <License:Response xsi:type="xsd:string"></License:Response>
  </License:GetModuleLicenseHistoryFromLicenseServerResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```
