---
title: Services84.SelectionAgent.SaveSelectionEntity SOAP
generated: 1
uid: Services84-Selection-SaveSelectionEntity
---

# Services84 Selection SaveSelectionEntity

SOAP request and response examples **Remote/Services84/Selection.svc**
Implemented by the <see cref="M:SuperOffice.Services84.ISelectionAgent.SaveSelectionEntity">SuperOffice.Services84.ISelectionAgent.SaveSelectionEntity</see> method.

## SaveSelectionEntity

Updates the existing SelectionEntity or creates a new SelectionEntity if the id parameter is 0.

* **selectionEntity:** The SelectionEntity that is saved.

**Returns:** New or updated SelectionEntity

[WSDL file for Services84/Selection](../Services84-Selection.md)

Obtain a ticket from the [Services84/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## SaveSelectionEntity Request

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices842="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices841="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Selection="http://www.superoffice.net/ws/crm/NetServer/Services84">
  <Selection:ApplicationToken>1234567-1234-9876</Selection:ApplicationToken>
  <Selection:Credentials>
    <Selection:Ticket>7T:1234abcxyzExample==</Selection:Ticket>
  </Selection:Credentials>
 <SOAP-ENV:Body>
   <Selection:SaveSelectionEntity>
    <Selection:SelectionEntity xsi:type="Selection:SelectionEntity">
     <Selection:Description xsi:type="xsd:string"></Selection:Description>
     <Selection:Postit xsi:type="xsd:string"></Selection:Postit>
     <Selection:Associate xsi:type="Selection:Associate">
      <Selection:AssociateId xsi:type="xsd:int">0</Selection:AssociateId>
      <Selection:Name xsi:type="xsd:string"></Selection:Name>
      <Selection:PersonId xsi:type="xsd:int">0</Selection:PersonId>
      <Selection:Rank xsi:type="xsd:short">0</Selection:Rank>
      <Selection:Tooltip xsi:type="xsd:string"></Selection:Tooltip>
      <Selection:Type xsi:type="Selection:UserType">Unknown</Selection:Type>
      <Selection:GroupIdx xsi:type="xsd:int">0</Selection:GroupIdx>
      <Selection:FullName xsi:type="xsd:string"></Selection:FullName>
      <Selection:FormalName xsi:type="xsd:string"></Selection:FormalName>
      <Selection:Deleted xsi:type="xsd:boolean">false</Selection:Deleted>
      <Selection:EjUserId xsi:type="xsd:int">0</Selection:EjUserId>
     </Selection:Associate>
     <Selection:CreatedBy xsi:type="Selection:Associate">
      <Selection:AssociateId xsi:type="xsd:int">0</Selection:AssociateId>
      <Selection:Name xsi:type="xsd:string"></Selection:Name>
      <Selection:PersonId xsi:type="xsd:int">0</Selection:PersonId>
      <Selection:Rank xsi:type="xsd:short">0</Selection:Rank>
      <Selection:Tooltip xsi:type="xsd:string"></Selection:Tooltip>
      <Selection:Type xsi:type="Selection:UserType">Unknown</Selection:Type>
      <Selection:GroupIdx xsi:type="xsd:int">0</Selection:GroupIdx>
      <Selection:FullName xsi:type="xsd:string"></Selection:FullName>
      <Selection:FormalName xsi:type="xsd:string"></Selection:FormalName>
      <Selection:Deleted xsi:type="xsd:boolean">false</Selection:Deleted>
      <Selection:EjUserId xsi:type="xsd:int">0</Selection:EjUserId>
     </Selection:CreatedBy>
     <Selection:UpdatedBy xsi:type="Selection:Associate">
      <Selection:AssociateId xsi:type="xsd:int">0</Selection:AssociateId>
      <Selection:Name xsi:type="xsd:string"></Selection:Name>
      <Selection:PersonId xsi:type="xsd:int">0</Selection:PersonId>
      <Selection:Rank xsi:type="xsd:short">0</Selection:Rank>
      <Selection:Tooltip xsi:type="xsd:string"></Selection:Tooltip>
      <Selection:Type xsi:type="Selection:UserType">Unknown</Selection:Type>
      <Selection:GroupIdx xsi:type="xsd:int">0</Selection:GroupIdx>
      <Selection:FullName xsi:type="xsd:string"></Selection:FullName>
      <Selection:FormalName xsi:type="xsd:string"></Selection:FormalName>
      <Selection:Deleted xsi:type="xsd:boolean">false</Selection:Deleted>
      <Selection:EjUserId xsi:type="xsd:int">0</Selection:EjUserId>
     </Selection:UpdatedBy>
     <Selection:SelectionCategory xsi:type="Selection:SelectionCategory">
      <Selection:Id xsi:type="xsd:int">0</Selection:Id>
      <Selection:Value xsi:type="xsd:string"></Selection:Value>
      <Selection:Tooltip xsi:type="xsd:string"></Selection:Tooltip>
     </Selection:SelectionCategory>
     <Selection:GroupIdx xsi:type="xsd:int">0</Selection:GroupIdx>
     <Selection:IncludePerson xsi:type="xsd:int">0</Selection:IncludePerson>
     <Selection:MemberCount xsi:type="xsd:unsignedInt">0</Selection:MemberCount>
     <Selection:Name xsi:type="xsd:string"></Selection:Name>
     <Selection:PostitTextId xsi:type="xsd:int">0</Selection:PostitTextId>
     <Selection:CreatedDate xsi:type="xsd:dateTime">2022-08-26T08:51:46Z</Selection:CreatedDate>
     <Selection:SelectionId xsi:type="xsd:int">0</Selection:SelectionId>
     <Selection:SoundEx xsi:type="xsd:string"></Selection:SoundEx>
     <Selection:Source xsi:type="xsd:short">0</Selection:Source>
     <Selection:TextId xsi:type="xsd:int">0</Selection:TextId>
     <Selection:UpdatedDate xsi:type="xsd:dateTime">2022-08-26T08:51:46Z</Selection:UpdatedDate>
     <Selection:UpdatedCount xsi:type="xsd:short">0</Selection:UpdatedCount>
     <Selection:Visibility xsi:type="xsd:short">0</Selection:Visibility>
     <Selection:SelectionType xsi:type="Selection:SelectionType">Static</Selection:SelectionType>
     <Selection:CompanyUnique xsi:type="xsd:boolean">false</Selection:CompanyUnique>
     <Selection:TargetTableNumber xsi:type="xsd:int">0</Selection:TargetTableNumber>
     <Selection:TargetTableName xsi:type="xsd:string"></Selection:TargetTableName>
     <Selection:Completed xsi:type="xsd:boolean">false</Selection:Completed>
     <Selection:LeftSelectionId xsi:type="xsd:int">0</Selection:LeftSelectionId>
     <Selection:RightSelectionId xsi:type="xsd:int">0</Selection:RightSelectionId>
     <Selection:SelectionUnionType xsi:type="Selection:SelectionUnionType">Unknown</Selection:SelectionUnionType>
     <Selection:VisibleFor xsi:type="Selection:ArrayOfVisibleFor">
      <Selection:VisibleFor xsi:type="Selection:VisibleFor">
       <Selection:VisibleId xsi:type="xsd:int">0</Selection:VisibleId>
       <Selection:Visibility xsi:type="Selection:Visibility">All</Selection:Visibility>
       <Selection:DisplayValue xsi:type="xsd:string"></Selection:DisplayValue>
      </Selection:VisibleFor>
     </Selection:VisibleFor>
    </Selection:SelectionEntity>
   </Selection:SaveSelectionEntity>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

## SaveSelectionEntity Response

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices842="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices841="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Selection="http://www.superoffice.net/ws/crm/NetServer/Services84">
 <SOAP-ENV:Body>
  <Selection:SaveSelectionEntityResponse>
   <Selection:Response xsi:type="Selection:SelectionEntity">
    <Selection:Description xsi:type="xsd:string"></Selection:Description>
    <Selection:Postit xsi:type="xsd:string"></Selection:Postit>
    <Selection:Associate xsi:type="Selection:Associate">
     <Selection:AssociateId xsi:type="xsd:int">0</Selection:AssociateId>
     <Selection:Name xsi:type="xsd:string"></Selection:Name>
     <Selection:PersonId xsi:type="xsd:int">0</Selection:PersonId>
     <Selection:Rank xsi:type="xsd:short">0</Selection:Rank>
     <Selection:Tooltip xsi:type="xsd:string"></Selection:Tooltip>
     <Selection:Type xsi:type="Selection:UserType">Unknown</Selection:Type>
     <Selection:GroupIdx xsi:type="xsd:int">0</Selection:GroupIdx>
     <Selection:FullName xsi:type="xsd:string"></Selection:FullName>
     <Selection:FormalName xsi:type="xsd:string"></Selection:FormalName>
     <Selection:Deleted xsi:type="xsd:boolean">false</Selection:Deleted>
     <Selection:EjUserId xsi:type="xsd:int">0</Selection:EjUserId>
    </Selection:Associate>
    <Selection:CreatedBy xsi:type="Selection:Associate">
     <Selection:AssociateId xsi:type="xsd:int">0</Selection:AssociateId>
     <Selection:Name xsi:type="xsd:string"></Selection:Name>
     <Selection:PersonId xsi:type="xsd:int">0</Selection:PersonId>
     <Selection:Rank xsi:type="xsd:short">0</Selection:Rank>
     <Selection:Tooltip xsi:type="xsd:string"></Selection:Tooltip>
     <Selection:Type xsi:type="Selection:UserType">Unknown</Selection:Type>
     <Selection:GroupIdx xsi:type="xsd:int">0</Selection:GroupIdx>
     <Selection:FullName xsi:type="xsd:string"></Selection:FullName>
     <Selection:FormalName xsi:type="xsd:string"></Selection:FormalName>
     <Selection:Deleted xsi:type="xsd:boolean">false</Selection:Deleted>
     <Selection:EjUserId xsi:type="xsd:int">0</Selection:EjUserId>
    </Selection:CreatedBy>
    <Selection:UpdatedBy xsi:type="Selection:Associate">
     <Selection:AssociateId xsi:type="xsd:int">0</Selection:AssociateId>
     <Selection:Name xsi:type="xsd:string"></Selection:Name>
     <Selection:PersonId xsi:type="xsd:int">0</Selection:PersonId>
     <Selection:Rank xsi:type="xsd:short">0</Selection:Rank>
     <Selection:Tooltip xsi:type="xsd:string"></Selection:Tooltip>
     <Selection:Type xsi:type="Selection:UserType">Unknown</Selection:Type>
     <Selection:GroupIdx xsi:type="xsd:int">0</Selection:GroupIdx>
     <Selection:FullName xsi:type="xsd:string"></Selection:FullName>
     <Selection:FormalName xsi:type="xsd:string"></Selection:FormalName>
     <Selection:Deleted xsi:type="xsd:boolean">false</Selection:Deleted>
     <Selection:EjUserId xsi:type="xsd:int">0</Selection:EjUserId>
    </Selection:UpdatedBy>
    <Selection:SelectionCategory xsi:type="Selection:SelectionCategory">
     <Selection:Id xsi:type="xsd:int">0</Selection:Id>
     <Selection:Value xsi:type="xsd:string"></Selection:Value>
     <Selection:Tooltip xsi:type="xsd:string"></Selection:Tooltip>
    </Selection:SelectionCategory>
    <Selection:GroupIdx xsi:type="xsd:int">0</Selection:GroupIdx>
    <Selection:IncludePerson xsi:type="xsd:int">0</Selection:IncludePerson>
    <Selection:MemberCount xsi:type="xsd:unsignedInt">0</Selection:MemberCount>
    <Selection:Name xsi:type="xsd:string"></Selection:Name>
    <Selection:PostitTextId xsi:type="xsd:int">0</Selection:PostitTextId>
    <Selection:CreatedDate xsi:type="xsd:dateTime">2022-08-26T08:51:46Z</Selection:CreatedDate>
    <Selection:SelectionId xsi:type="xsd:int">0</Selection:SelectionId>
    <Selection:SoundEx xsi:type="xsd:string"></Selection:SoundEx>
    <Selection:Source xsi:type="xsd:short">0</Selection:Source>
    <Selection:TextId xsi:type="xsd:int">0</Selection:TextId>
    <Selection:UpdatedDate xsi:type="xsd:dateTime">2022-08-26T08:51:46Z</Selection:UpdatedDate>
    <Selection:UpdatedCount xsi:type="xsd:short">0</Selection:UpdatedCount>
    <Selection:Visibility xsi:type="xsd:short">0</Selection:Visibility>
    <Selection:SelectionType xsi:type="Selection:SelectionType">Static</Selection:SelectionType>
    <Selection:CompanyUnique xsi:type="xsd:boolean">false</Selection:CompanyUnique>
    <Selection:TargetTableNumber xsi:type="xsd:int">0</Selection:TargetTableNumber>
    <Selection:TargetTableName xsi:type="xsd:string"></Selection:TargetTableName>
    <Selection:Completed xsi:type="xsd:boolean">false</Selection:Completed>
    <Selection:LeftSelectionId xsi:type="xsd:int">0</Selection:LeftSelectionId>
    <Selection:RightSelectionId xsi:type="xsd:int">0</Selection:RightSelectionId>
    <Selection:SelectionUnionType xsi:type="Selection:SelectionUnionType">Unknown</Selection:SelectionUnionType>
    <Selection:VisibleFor xsi:type="Selection:ArrayOfVisibleFor">
     <Selection:VisibleFor xsi:type="Selection:VisibleFor">
      <Selection:VisibleId xsi:type="xsd:int">0</Selection:VisibleId>
      <Selection:Visibility xsi:type="Selection:Visibility">All</Selection:Visibility>
      <Selection:DisplayValue xsi:type="xsd:string"></Selection:DisplayValue>
     </Selection:VisibleFor>
    </Selection:VisibleFor>
   </Selection:Response>
  </Selection:SaveSelectionEntityResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```
