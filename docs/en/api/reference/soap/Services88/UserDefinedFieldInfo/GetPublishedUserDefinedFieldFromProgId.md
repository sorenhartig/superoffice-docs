---
title: Services88.UserDefinedFieldInfoAgent.GetPublishedUserDefinedFieldFromProgId SOAP
generated: 1
uid: Services88-UserDefinedFieldInfo-GetPublishedUserDefinedFieldFromProgId
---

# Services88 UserDefinedFieldInfo GetPublishedUserDefinedFieldFromProgId

SOAP request and response examples **Remote/Services88/UserDefinedFieldInfo.svc**
Implemented by the <see cref="M:SuperOffice.Services88.IUserDefinedFieldInfoAgent.GetPublishedUserDefinedFieldFromProgId">SuperOffice.Services88.IUserDefinedFieldInfoAgent.GetPublishedUserDefinedFieldFromProgId</see> method.

## GetPublishedUserDefinedFieldFromProgId

Return information about the given user defined field identified by the owner and the prog-id. The prog-id is used as the key in the entity carriers.

* **progId:** The prog.id is a hidden name that uniquely identifies the field.
* **ownerType:** The user-defined field owner-entity id.

**Returns:** Returns the user-defined field info carrier, or null if no matching field is found.

[WSDL file for Services88/UserDefinedFieldInfo](../Services88-UserDefinedFieldInfo.md)

Obtain a ticket from the [Services88/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## GetPublishedUserDefinedFieldFromProgId Request

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices882="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices881="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:UserDefinedFieldInfo="http://www.superoffice.net/ws/crm/NetServer/Services88">
  <UserDefinedFieldInfo:ApplicationToken>1234567-1234-9876</UserDefinedFieldInfo:ApplicationToken>
  <UserDefinedFieldInfo:Credentials>
    <UserDefinedFieldInfo:Ticket>7T:1234abcxyzExample==</UserDefinedFieldInfo:Ticket>
  </UserDefinedFieldInfo:Credentials>
 <SOAP-ENV:Body>
   <UserDefinedFieldInfo:GetPublishedUserDefinedFieldFromProgId>
    <UserDefinedFieldInfo:ProgId xsi:type="xsd:string"></UserDefinedFieldInfo:ProgId>
    <UserDefinedFieldInfo:OwnerType xsi:type="UserDefinedFieldInfo:UDefType">Invalid</UserDefinedFieldInfo:OwnerType>
   </UserDefinedFieldInfo:GetPublishedUserDefinedFieldFromProgId>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

## GetPublishedUserDefinedFieldFromProgId Response

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices882="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices881="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:UserDefinedFieldInfo="http://www.superoffice.net/ws/crm/NetServer/Services88">
 <SOAP-ENV:Body>
  <UserDefinedFieldInfo:GetPublishedUserDefinedFieldFromProgIdResponse>
   <UserDefinedFieldInfo:Response xsi:type="UserDefinedFieldInfo:UserDefinedFieldInfo">
    <UserDefinedFieldInfo:UDefFieldId xsi:type="xsd:int">0</UserDefinedFieldInfo:UDefFieldId>
    <UserDefinedFieldInfo:ColumnId xsi:type="xsd:int">0</UserDefinedFieldInfo:ColumnId>
    <UserDefinedFieldInfo:FieldDefault xsi:type="xsd:string"></UserDefinedFieldInfo:FieldDefault>
    <UserDefinedFieldInfo:FieldHeight xsi:type="xsd:short">0</UserDefinedFieldInfo:FieldHeight>
    <UserDefinedFieldInfo:FieldLabel xsi:type="xsd:string"></UserDefinedFieldInfo:FieldLabel>
    <UserDefinedFieldInfo:FieldLeft xsi:type="xsd:short">0</UserDefinedFieldInfo:FieldLeft>
    <UserDefinedFieldInfo:FieldTop xsi:type="xsd:short">0</UserDefinedFieldInfo:FieldTop>
    <UserDefinedFieldInfo:FieldType xsi:type="UserDefinedFieldInfo:UDefFieldType">Number</UserDefinedFieldInfo:FieldType>
    <UserDefinedFieldInfo:FieldWidth xsi:type="xsd:short">0</UserDefinedFieldInfo:FieldWidth>
    <UserDefinedFieldInfo:FormatMask xsi:type="xsd:string"></UserDefinedFieldInfo:FormatMask>
    <UserDefinedFieldInfo:HideLabel xsi:type="xsd:boolean">false</UserDefinedFieldInfo:HideLabel>
    <UserDefinedFieldInfo:IsIndexed xsi:type="xsd:boolean">false</UserDefinedFieldInfo:IsIndexed>
    <UserDefinedFieldInfo:LabelHeight xsi:type="xsd:short">0</UserDefinedFieldInfo:LabelHeight>
    <UserDefinedFieldInfo:LabelLeft xsi:type="xsd:short">0</UserDefinedFieldInfo:LabelLeft>
    <UserDefinedFieldInfo:LabelTop xsi:type="xsd:short">0</UserDefinedFieldInfo:LabelTop>
    <UserDefinedFieldInfo:LabelWidth xsi:type="xsd:short">0</UserDefinedFieldInfo:LabelWidth>
    <UserDefinedFieldInfo:LastVersionId xsi:type="xsd:int">0</UserDefinedFieldInfo:LastVersionId>
    <UserDefinedFieldInfo:ListTableId xsi:type="xsd:short">0</UserDefinedFieldInfo:ListTableId>
    <UserDefinedFieldInfo:IsMandatory xsi:type="xsd:boolean">false</UserDefinedFieldInfo:IsMandatory>
    <UserDefinedFieldInfo:Type xsi:type="UserDefinedFieldInfo:UDefType">Invalid</UserDefinedFieldInfo:Type>
    <UserDefinedFieldInfo:Page1LineNo xsi:type="xsd:short">0</UserDefinedFieldInfo:Page1LineNo>
    <UserDefinedFieldInfo:ProgId xsi:type="xsd:string"></UserDefinedFieldInfo:ProgId>
    <UserDefinedFieldInfo:IsReadOnly xsi:type="xsd:boolean">false</UserDefinedFieldInfo:IsReadOnly>
    <UserDefinedFieldInfo:ShortLabel xsi:type="xsd:string"></UserDefinedFieldInfo:ShortLabel>
    <UserDefinedFieldInfo:TabOrder xsi:type="xsd:short">0</UserDefinedFieldInfo:TabOrder>
    <UserDefinedFieldInfo:TextLength xsi:type="xsd:short">0</UserDefinedFieldInfo:TextLength>
    <UserDefinedFieldInfo:Tooltip xsi:type="xsd:string"></UserDefinedFieldInfo:Tooltip>
    <UserDefinedFieldInfo:UdefIdentity xsi:type="xsd:int">0</UserDefinedFieldInfo:UdefIdentity>
    <UserDefinedFieldInfo:UDListDefinitionId xsi:type="xsd:int">0</UserDefinedFieldInfo:UDListDefinitionId>
    <UserDefinedFieldInfo:Justification xsi:type="UserDefinedFieldInfo:UdefJustification">Default</UserDefinedFieldInfo:Justification>
    <UserDefinedFieldInfo:Version xsi:type="xsd:short">0</UserDefinedFieldInfo:Version>
    <UserDefinedFieldInfo:TemplateVariableName xsi:type="xsd:string"></UserDefinedFieldInfo:TemplateVariableName>
    <UserDefinedFieldInfo:HasBeenPublished xsi:type="xsd:boolean">false</UserDefinedFieldInfo:HasBeenPublished>
    <UserDefinedFieldInfo:MdoListName xsi:type="xsd:string"></UserDefinedFieldInfo:MdoListName>
   </UserDefinedFieldInfo:Response>
  </UserDefinedFieldInfo:GetPublishedUserDefinedFieldFromProgIdResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```
