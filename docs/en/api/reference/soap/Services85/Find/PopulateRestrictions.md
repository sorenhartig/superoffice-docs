---
title: Services85.FindAgent.PopulateRestrictions SOAP
generated: 1
uid: Services85-Find-PopulateRestrictions
---

# Services85 Find PopulateRestrictions

SOAP request and response examples **Remote/Services85/Find.svc**
Implemented by the <see cref="M:SuperOffice.Services85.IFindAgent.PopulateRestrictions">SuperOffice.Services85.IFindAgent.PopulateRestrictions</see> method.

## PopulateRestrictions

Take an incoming set of minimally populated restrictions (name + operator is required), and populate all the other parts of the ArchiveRestrictionInfo structure. This includes column information, display values (including list value lookup), and calculated/default values where the value hints specify read-only (R).

* **providerName:** Provider name to use for populating column information
* **restrictions:** Restrictions to populate. The Name and Operator fields have to have valid content, and Values should be set as appropriate. Other fields can be left blank or null. If a ColumnInfo is already set, it will not be overwritten.

**Returns:** Fully populated restrictions in the same order as the incoming restrictions.

[WSDL file for Services85/Find](../Services85-Find.md)

Obtain a ticket from the [Services85/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## PopulateRestrictions Request

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices852="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices851="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Find="http://www.superoffice.net/ws/crm/NetServer/Services85">
  <Find:ApplicationToken>1234567-1234-9876</Find:ApplicationToken>
  <Find:Credentials>
    <Find:Ticket>7T:1234abcxyzExample==</Find:Ticket>
  </Find:Credentials>
 <SOAP-ENV:Body>
   <Find:PopulateRestrictions>
    <Find:ProviderName xsi:type="xsd:string"></Find:ProviderName>
    <Find:Restrictions xsi:type="Find:ArrayOfArchiveRestrictionInfo">
     <Find:ArchiveRestrictionInfo xsi:type="Find:ArchiveRestrictionInfo">
      <Find:Name xsi:type="xsd:string"></Find:Name>
      <Find:Operator xsi:type="xsd:string"></Find:Operator>
      <Find:Values xsi:type="NetServerServices852:ArrayOfstring">
       <NetServerServices852:string xsi:type="xsd:string"></NetServerServices852:string>
      </Find:Values>
      <Find:DisplayValues xsi:type="NetServerServices852:ArrayOfstring">
       <NetServerServices852:string xsi:type="xsd:string"></NetServerServices852:string>
      </Find:DisplayValues>
      <Find:ColumnInfo xsi:type="Find:ArchiveColumnInfo">
       <Find:DisplayName xsi:type="xsd:string"></Find:DisplayName>
       <Find:DisplayTooltip xsi:type="xsd:string"></Find:DisplayTooltip>
       <Find:DisplayType xsi:type="xsd:string"></Find:DisplayType>
       <Find:CanOrderBy xsi:type="xsd:boolean">false</Find:CanOrderBy>
       <Find:Name xsi:type="xsd:string"></Find:Name>
       <Find:CanRestrictBy xsi:type="xsd:boolean">false</Find:CanRestrictBy>
       <Find:RestrictionType xsi:type="xsd:string"></Find:RestrictionType>
       <Find:RestrictionListName xsi:type="xsd:string"></Find:RestrictionListName>
       <Find:IsVisible xsi:type="xsd:boolean">false</Find:IsVisible>
       <Find:Width xsi:type="xsd:string"></Find:Width>
       <Find:IconHint xsi:type="xsd:string"></Find:IconHint>
       <Find:HeadingIconHint xsi:type="xsd:string"></Find:HeadingIconHint>
      </Find:ColumnInfo>
      <Find:IsActive xsi:type="xsd:boolean">false</Find:IsActive>
      <Find:SubRestrictions xsi:type="Find:ArrayOfArchiveRestrictionInfo">
       <Find:ArchiveRestrictionInfo xsi:type="Find:ArchiveRestrictionInfo">
        <Find:Name xsi:type="xsd:string"></Find:Name>
        <Find:Operator xsi:type="xsd:string"></Find:Operator>
        <Find:Values xsi:type="NetServerServices852:ArrayOfstring">
         <NetServerServices852:string xsi:type="xsd:string"></NetServerServices852:string>
        </Find:Values>
        <Find:DisplayValues xsi:type="NetServerServices852:ArrayOfstring">
         <NetServerServices852:string xsi:type="xsd:string"></NetServerServices852:string>
        </Find:DisplayValues>
        <Find:ColumnInfo xsi:type="Find:ArchiveColumnInfo">
         <Find:DisplayName xsi:type="xsd:string"></Find:DisplayName>
         <Find:DisplayTooltip xsi:type="xsd:string"></Find:DisplayTooltip>
         <Find:DisplayType xsi:type="xsd:string"></Find:DisplayType>
         <Find:CanOrderBy xsi:type="xsd:boolean">false</Find:CanOrderBy>
         <Find:Name xsi:type="xsd:string"></Find:Name>
         <Find:CanRestrictBy xsi:type="xsd:boolean">false</Find:CanRestrictBy>
         <Find:RestrictionType xsi:type="xsd:string"></Find:RestrictionType>
         <Find:RestrictionListName xsi:type="xsd:string"></Find:RestrictionListName>
         <Find:IsVisible xsi:type="xsd:boolean">false</Find:IsVisible>
         <Find:Width xsi:type="xsd:string"></Find:Width>
         <Find:IconHint xsi:type="xsd:string"></Find:IconHint>
         <Find:HeadingIconHint xsi:type="xsd:string"></Find:HeadingIconHint>
        </Find:ColumnInfo>
        <Find:IsActive xsi:type="xsd:boolean">false</Find:IsActive>
        <Find:SubRestrictions xsi:type="Find:ArrayOfArchiveRestrictionInfo">
         <Find:ArchiveRestrictionInfo xsi:type="Find:ArchiveRestrictionInfo">
          <Find:Name xsi:type="xsd:string"></Find:Name>
          <Find:Operator xsi:type="xsd:string"></Find:Operator>
          <Find:Values xsi:nil="true"></Find:Values>
          <Find:DisplayValues xsi:nil="true"></Find:DisplayValues>
          <Find:ColumnInfo xsi:nil="true"></Find:ColumnInfo>
          <Find:IsActive xsi:nil="true"></Find:IsActive>
          <Find:SubRestrictions xsi:nil="true"></Find:SubRestrictions>
          <Find:InterParenthesis xsi:nil="true"></Find:InterParenthesis>
          <Find:InterOperator xsi:nil="true"></Find:InterOperator>
          <Find:UniqueHash xsi:nil="true"></Find:UniqueHash>
         </Find:ArchiveRestrictionInfo>
        </Find:SubRestrictions>
        <Find:InterParenthesis xsi:type="xsd:int">0</Find:InterParenthesis>
        <Find:InterOperator xsi:type="Find:InterRestrictionOperator">None</Find:InterOperator>
        <Find:UniqueHash xsi:type="xsd:int">0</Find:UniqueHash>
       </Find:ArchiveRestrictionInfo>
      </Find:SubRestrictions>
      <Find:InterParenthesis xsi:type="xsd:int">0</Find:InterParenthesis>
      <Find:InterOperator xsi:type="Find:InterRestrictionOperator">None</Find:InterOperator>
      <Find:UniqueHash xsi:type="xsd:int">0</Find:UniqueHash>
     </Find:ArchiveRestrictionInfo>
    </Find:Restrictions>
   </Find:PopulateRestrictions>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

## PopulateRestrictions Response

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices852="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices851="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Find="http://www.superoffice.net/ws/crm/NetServer/Services85">
 <SOAP-ENV:Body>
  <Find:PopulateRestrictionsResponse>
   <Find:Response xsi:type="Find:ArrayOfArchiveRestrictionInfo">
    <Find:ArchiveRestrictionInfo xsi:type="Find:ArchiveRestrictionInfo">
     <Find:Name xsi:type="xsd:string"></Find:Name>
     <Find:Operator xsi:type="xsd:string"></Find:Operator>
     <Find:Values xsi:type="NetServerServices852:ArrayOfstring">
      <NetServerServices852:string xsi:type="xsd:string"></NetServerServices852:string>
     </Find:Values>
     <Find:DisplayValues xsi:type="NetServerServices852:ArrayOfstring">
      <NetServerServices852:string xsi:type="xsd:string"></NetServerServices852:string>
     </Find:DisplayValues>
     <Find:ColumnInfo xsi:type="Find:ArchiveColumnInfo">
      <Find:DisplayName xsi:type="xsd:string"></Find:DisplayName>
      <Find:DisplayTooltip xsi:type="xsd:string"></Find:DisplayTooltip>
      <Find:DisplayType xsi:type="xsd:string"></Find:DisplayType>
      <Find:CanOrderBy xsi:type="xsd:boolean">false</Find:CanOrderBy>
      <Find:Name xsi:type="xsd:string"></Find:Name>
      <Find:CanRestrictBy xsi:type="xsd:boolean">false</Find:CanRestrictBy>
      <Find:RestrictionType xsi:type="xsd:string"></Find:RestrictionType>
      <Find:RestrictionListName xsi:type="xsd:string"></Find:RestrictionListName>
      <Find:IsVisible xsi:type="xsd:boolean">false</Find:IsVisible>
      <Find:Width xsi:type="xsd:string"></Find:Width>
      <Find:IconHint xsi:type="xsd:string"></Find:IconHint>
      <Find:HeadingIconHint xsi:type="xsd:string"></Find:HeadingIconHint>
     </Find:ColumnInfo>
     <Find:IsActive xsi:type="xsd:boolean">false</Find:IsActive>
     <Find:SubRestrictions xsi:type="Find:ArrayOfArchiveRestrictionInfo">
      <Find:ArchiveRestrictionInfo xsi:type="Find:ArchiveRestrictionInfo">
       <Find:Name xsi:type="xsd:string"></Find:Name>
       <Find:Operator xsi:type="xsd:string"></Find:Operator>
       <Find:Values xsi:type="NetServerServices852:ArrayOfstring">
        <NetServerServices852:string xsi:type="xsd:string"></NetServerServices852:string>
       </Find:Values>
       <Find:DisplayValues xsi:type="NetServerServices852:ArrayOfstring">
        <NetServerServices852:string xsi:type="xsd:string"></NetServerServices852:string>
       </Find:DisplayValues>
       <Find:ColumnInfo xsi:type="Find:ArchiveColumnInfo">
        <Find:DisplayName xsi:type="xsd:string"></Find:DisplayName>
        <Find:DisplayTooltip xsi:type="xsd:string"></Find:DisplayTooltip>
        <Find:DisplayType xsi:type="xsd:string"></Find:DisplayType>
        <Find:CanOrderBy xsi:type="xsd:boolean">false</Find:CanOrderBy>
        <Find:Name xsi:type="xsd:string"></Find:Name>
        <Find:CanRestrictBy xsi:type="xsd:boolean">false</Find:CanRestrictBy>
        <Find:RestrictionType xsi:type="xsd:string"></Find:RestrictionType>
        <Find:RestrictionListName xsi:type="xsd:string"></Find:RestrictionListName>
        <Find:IsVisible xsi:type="xsd:boolean">false</Find:IsVisible>
        <Find:Width xsi:type="xsd:string"></Find:Width>
        <Find:IconHint xsi:type="xsd:string"></Find:IconHint>
        <Find:HeadingIconHint xsi:type="xsd:string"></Find:HeadingIconHint>
       </Find:ColumnInfo>
       <Find:IsActive xsi:type="xsd:boolean">false</Find:IsActive>
       <Find:SubRestrictions xsi:type="Find:ArrayOfArchiveRestrictionInfo">
        <Find:ArchiveRestrictionInfo xsi:type="Find:ArchiveRestrictionInfo">
         <Find:Name xsi:type="xsd:string"></Find:Name>
         <Find:Operator xsi:type="xsd:string"></Find:Operator>
         <Find:Values xsi:type="NetServerServices852:ArrayOfstring">
          <NetServerServices852:string xsi:nil="true"></NetServerServices852:string>
         </Find:Values>
         <Find:DisplayValues xsi:type="NetServerServices852:ArrayOfstring">
          <NetServerServices852:string xsi:nil="true"></NetServerServices852:string>
         </Find:DisplayValues>
         <Find:ColumnInfo xsi:type="Find:ArchiveColumnInfo">
          <Find:DisplayName xsi:type="xsd:string"></Find:DisplayName>
          <Find:DisplayTooltip xsi:type="xsd:string"></Find:DisplayTooltip>
          <Find:DisplayType xsi:type="xsd:string"></Find:DisplayType>
          <Find:CanOrderBy xsi:nil="true"></Find:CanOrderBy>
          <Find:Name xsi:type="xsd:string"></Find:Name>
          <Find:CanRestrictBy xsi:nil="true"></Find:CanRestrictBy>
          <Find:RestrictionType xsi:type="xsd:string"></Find:RestrictionType>
          <Find:RestrictionListName xsi:type="xsd:string"></Find:RestrictionListName>
          <Find:IsVisible xsi:nil="true"></Find:IsVisible>
          <Find:Width xsi:type="xsd:string"></Find:Width>
          <Find:IconHint xsi:type="xsd:string"></Find:IconHint>
          <Find:HeadingIconHint xsi:type="xsd:string"></Find:HeadingIconHint>
         </Find:ColumnInfo>
         <Find:IsActive xsi:type="xsd:boolean">false</Find:IsActive>
         <Find:SubRestrictions xsi:type="Find:ArrayOfArchiveRestrictionInfo">
          <Find:ArchiveRestrictionInfo xsi:nil="true"></Find:ArchiveRestrictionInfo>
         </Find:SubRestrictions>
         <Find:InterParenthesis xsi:type="xsd:int">0</Find:InterParenthesis>
         <Find:InterOperator xsi:type="Find:InterRestrictionOperator">None</Find:InterOperator>
         <Find:UniqueHash xsi:type="xsd:int">0</Find:UniqueHash>
        </Find:ArchiveRestrictionInfo>
       </Find:SubRestrictions>
       <Find:InterParenthesis xsi:type="xsd:int">0</Find:InterParenthesis>
       <Find:InterOperator xsi:type="Find:InterRestrictionOperator">None</Find:InterOperator>
       <Find:UniqueHash xsi:type="xsd:int">0</Find:UniqueHash>
      </Find:ArchiveRestrictionInfo>
     </Find:SubRestrictions>
     <Find:InterParenthesis xsi:type="xsd:int">0</Find:InterParenthesis>
     <Find:InterOperator xsi:type="Find:InterRestrictionOperator">None</Find:InterOperator>
     <Find:UniqueHash xsi:type="xsd:int">0</Find:UniqueHash>
    </Find:ArchiveRestrictionInfo>
   </Find:Response>
  </Find:PopulateRestrictionsResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```
