---
title: Services86.AssociateAgent.GetAssociateList SOAP
generated: 1
uid: Services86-Associate-GetAssociateList
---

# Services86 Associate GetAssociateList

SOAP request and response examples **Remote/Services86/Associate.svc**
Implemented by the <see cref="M:SuperOffice.Services86.IAssociateAgent.GetAssociateList">SuperOffice.Services86.IAssociateAgent.GetAssociateList</see> method.

## GetAssociateList

Gets an array of Associate objects.

* **associateIds:** The identifiers of the Associate object

**Returns:** Array of Associate objects

[WSDL file for Services86/Associate](../Services86-Associate.md)

Obtain a ticket from the [Services86/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## GetAssociateList Request

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices862="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices861="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Associate="http://www.superoffice.net/ws/crm/NetServer/Services86">
  <Associate:ApplicationToken>1234567-1234-9876</Associate:ApplicationToken>
  <Associate:Credentials>
    <Associate:Ticket>7T:1234abcxyzExample==</Associate:Ticket>
  </Associate:Credentials>
 <SOAP-ENV:Body>
   <Associate:GetAssociateList>
    <Associate:AssociateIds xsi:type="NetServerServices862:ArrayOfint">
     <NetServerServices862:int xsi:type="xsd:int">0</NetServerServices862:int>
    </Associate:AssociateIds>
   </Associate:GetAssociateList>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

## GetAssociateList Response

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices862="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices861="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Associate="http://www.superoffice.net/ws/crm/NetServer/Services86">
 <SOAP-ENV:Body>
  <Associate:GetAssociateListResponse>
   <Associate:Response xsi:type="Associate:ArrayOfAssociate">
    <Associate:Associate xsi:type="Associate:Associate">
     <Associate:AssociateId xsi:type="xsd:int">0</Associate:AssociateId>
     <Associate:Name xsi:type="xsd:string"></Associate:Name>
     <Associate:PersonId xsi:type="xsd:int">0</Associate:PersonId>
     <Associate:Rank xsi:type="xsd:short">0</Associate:Rank>
     <Associate:Tooltip xsi:type="xsd:string"></Associate:Tooltip>
     <Associate:Type xsi:type="Associate:UserType">Unknown</Associate:Type>
     <Associate:GroupIdx xsi:type="xsd:int">0</Associate:GroupIdx>
     <Associate:FullName xsi:type="xsd:string"></Associate:FullName>
     <Associate:FormalName xsi:type="xsd:string"></Associate:FormalName>
     <Associate:Deleted xsi:type="xsd:boolean">false</Associate:Deleted>
     <Associate:EjUserId xsi:type="xsd:int">0</Associate:EjUserId>
     <Associate:UserName xsi:type="xsd:string"></Associate:UserName>
    </Associate:Associate>
   </Associate:Response>
  </Associate:GetAssociateListResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```
