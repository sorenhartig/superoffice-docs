---
title: Services85.AudienceAgent.SaveAudienceLayoutEntity SOAP
generated: 1
uid: Services85-Audience-SaveAudienceLayoutEntity
---

# Services85 Audience SaveAudienceLayoutEntity

SOAP request and response examples **Remote/Services85/Audience.svc**
Implemented by the <see cref="M:SuperOffice.Services85.IAudienceAgent.SaveAudienceLayoutEntity">SuperOffice.Services85.IAudienceAgent.SaveAudienceLayoutEntity</see> method.

## SaveAudienceLayoutEntity

Updates the existing AudienceLayoutEntity or creates a new AudienceLayoutEntity if the id parameter is 0.

* **audienceLayoutEntity:** The AudienceLayoutEntity that is saved.

**Returns:** New or updated AudienceLayoutEntity

[WSDL file for Services85/Audience](../Services85-Audience.md)

Obtain a ticket from the [Services85/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## SaveAudienceLayoutEntity Request

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices851="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Audience="http://www.superoffice.net/ws/crm/NetServer/Services85">
  <Audience:ApplicationToken>1234567-1234-9876</Audience:ApplicationToken>
  <Audience:Credentials>
    <Audience:Ticket>7T:1234abcxyzExample==</Audience:Ticket>
  </Audience:Credentials>
 <SOAP-ENV:Body>
   <Audience:SaveAudienceLayoutEntity>
    <Audience:AudienceLayoutEntity xsi:type="Audience:AudienceLayoutEntity">
     <Audience:AudienceLayoutId xsi:type="xsd:int">0</Audience:AudienceLayoutId>
     <Audience:InstanceLayout xsi:type="xsd:string"></Audience:InstanceLayout>
     <Audience:InstanceName xsi:type="xsd:string"></Audience:InstanceName>
     <Audience:CreatedDate xsi:type="xsd:dateTime">2022-08-26T08:52:14Z</Audience:CreatedDate>
     <Audience:UpdatedDate xsi:type="xsd:dateTime">2022-08-26T08:52:14Z</Audience:UpdatedDate>
     <Audience:CreatedBy xsi:type="Audience:Associate">
      <Audience:AssociateId xsi:type="xsd:int">0</Audience:AssociateId>
      <Audience:Name xsi:type="xsd:string"></Audience:Name>
      <Audience:PersonId xsi:type="xsd:int">0</Audience:PersonId>
      <Audience:Rank xsi:type="xsd:short">0</Audience:Rank>
      <Audience:Tooltip xsi:type="xsd:string"></Audience:Tooltip>
      <Audience:Type xsi:type="Audience:UserType">Unknown</Audience:Type>
      <Audience:GroupIdx xsi:type="xsd:int">0</Audience:GroupIdx>
      <Audience:FullName xsi:type="xsd:string"></Audience:FullName>
      <Audience:FormalName xsi:type="xsd:string"></Audience:FormalName>
      <Audience:Deleted xsi:type="xsd:boolean">false</Audience:Deleted>
      <Audience:EjUserId xsi:type="xsd:int">0</Audience:EjUserId>
     </Audience:CreatedBy>
     <Audience:UpdatedBy xsi:type="Audience:Associate">
      <Audience:AssociateId xsi:type="xsd:int">0</Audience:AssociateId>
      <Audience:Name xsi:type="xsd:string"></Audience:Name>
      <Audience:PersonId xsi:type="xsd:int">0</Audience:PersonId>
      <Audience:Rank xsi:type="xsd:short">0</Audience:Rank>
      <Audience:Tooltip xsi:type="xsd:string"></Audience:Tooltip>
      <Audience:Type xsi:type="Audience:UserType">Unknown</Audience:Type>
      <Audience:GroupIdx xsi:type="xsd:int">0</Audience:GroupIdx>
      <Audience:FullName xsi:type="xsd:string"></Audience:FullName>
      <Audience:FormalName xsi:type="xsd:string"></Audience:FormalName>
      <Audience:Deleted xsi:type="xsd:boolean">false</Audience:Deleted>
      <Audience:EjUserId xsi:type="xsd:int">0</Audience:EjUserId>
     </Audience:UpdatedBy>
    </Audience:AudienceLayoutEntity>
   </Audience:SaveAudienceLayoutEntity>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

## SaveAudienceLayoutEntity Response

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices851="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Audience="http://www.superoffice.net/ws/crm/NetServer/Services85">
 <SOAP-ENV:Body>
  <Audience:SaveAudienceLayoutEntityResponse>
   <Audience:Response xsi:type="Audience:AudienceLayoutEntity">
    <Audience:AudienceLayoutId xsi:type="xsd:int">0</Audience:AudienceLayoutId>
    <Audience:InstanceLayout xsi:type="xsd:string"></Audience:InstanceLayout>
    <Audience:InstanceName xsi:type="xsd:string"></Audience:InstanceName>
    <Audience:CreatedDate xsi:type="xsd:dateTime">2022-08-26T08:52:14Z</Audience:CreatedDate>
    <Audience:UpdatedDate xsi:type="xsd:dateTime">2022-08-26T08:52:14Z</Audience:UpdatedDate>
    <Audience:CreatedBy xsi:type="Audience:Associate">
     <Audience:AssociateId xsi:type="xsd:int">0</Audience:AssociateId>
     <Audience:Name xsi:type="xsd:string"></Audience:Name>
     <Audience:PersonId xsi:type="xsd:int">0</Audience:PersonId>
     <Audience:Rank xsi:type="xsd:short">0</Audience:Rank>
     <Audience:Tooltip xsi:type="xsd:string"></Audience:Tooltip>
     <Audience:Type xsi:type="Audience:UserType">Unknown</Audience:Type>
     <Audience:GroupIdx xsi:type="xsd:int">0</Audience:GroupIdx>
     <Audience:FullName xsi:type="xsd:string"></Audience:FullName>
     <Audience:FormalName xsi:type="xsd:string"></Audience:FormalName>
     <Audience:Deleted xsi:type="xsd:boolean">false</Audience:Deleted>
     <Audience:EjUserId xsi:type="xsd:int">0</Audience:EjUserId>
    </Audience:CreatedBy>
    <Audience:UpdatedBy xsi:type="Audience:Associate">
     <Audience:AssociateId xsi:type="xsd:int">0</Audience:AssociateId>
     <Audience:Name xsi:type="xsd:string"></Audience:Name>
     <Audience:PersonId xsi:type="xsd:int">0</Audience:PersonId>
     <Audience:Rank xsi:type="xsd:short">0</Audience:Rank>
     <Audience:Tooltip xsi:type="xsd:string"></Audience:Tooltip>
     <Audience:Type xsi:type="Audience:UserType">Unknown</Audience:Type>
     <Audience:GroupIdx xsi:type="xsd:int">0</Audience:GroupIdx>
     <Audience:FullName xsi:type="xsd:string"></Audience:FullName>
     <Audience:FormalName xsi:type="xsd:string"></Audience:FormalName>
     <Audience:Deleted xsi:type="xsd:boolean">false</Audience:Deleted>
     <Audience:EjUserId xsi:type="xsd:int">0</Audience:EjUserId>
    </Audience:UpdatedBy>
   </Audience:Response>
  </Audience:SaveAudienceLayoutEntityResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```
