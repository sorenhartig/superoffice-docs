---
title: Services88.TicketAgent.SplitTicketMessage SOAP
generated: 1
uid: Services88-Ticket-SplitTicketMessage
---

# Services88 Ticket SplitTicketMessage

SOAP request and response examples **Remote/Services88/Ticket.svc**
Implemented by the <see cref="M:SuperOffice.Services88.ITicketAgent.SplitTicketMessage">SuperOffice.Services88.ITicketAgent.SplitTicketMessage</see> method.

## SplitTicketMessage





[WSDL file for Services88/Ticket](../Services88-Ticket.md)

Obtain a ticket from the [Services88/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## SplitTicketMessage Request

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices882="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices881="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Ticket="http://www.superoffice.net/ws/crm/NetServer/Services88">
  <Ticket:ApplicationToken>1234567-1234-9876</Ticket:ApplicationToken>
  <Ticket:Credentials>
    <Ticket:Ticket>7T:1234abcxyzExample==</Ticket:Ticket>
  </Ticket:Credentials>
 <SOAP-ENV:Body>
   <Ticket:SplitTicketMessage>
    <Ticket:SourceTicketMessage xsi:type="Ticket:TicketMessageEntity">
     <Ticket:EjMessageId xsi:type="xsd:int">0</Ticket:EjMessageId>
     <Ticket:Ticket xsi:type="Ticket:Ticket">
      <Ticket:TicketId xsi:type="xsd:int">0</Ticket:TicketId>
      <Ticket:Title xsi:type="xsd:string"></Ticket:Title>
      <Ticket:CreatedAt xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:CreatedAt>
      <Ticket:LastChanged xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:LastChanged>
      <Ticket:ReadByOwner xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:ReadByOwner>
      <Ticket:ReadByCustomer xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:ReadByCustomer>
      <Ticket:FirstReadByUser xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:FirstReadByUser>
      <Ticket:Activate xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:Activate>
      <Ticket:ClosedAt xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:ClosedAt>
      <Ticket:RepliedAt xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:RepliedAt>
      <Ticket:AlertTimeout xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:AlertTimeout>
      <Ticket:Deadline xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:Deadline>
      <Ticket:CreatedBy xsi:type="xsd:int">0</Ticket:CreatedBy>
      <Ticket:CreatedByName xsi:type="xsd:string"></Ticket:CreatedByName>
      <Ticket:Author xsi:type="xsd:string"></Ticket:Author>
      <Ticket:OwnedBy xsi:type="xsd:int">0</Ticket:OwnedBy>
      <Ticket:OwnedByName xsi:type="xsd:string"></Ticket:OwnedByName>
      <Ticket:Category xsi:type="xsd:int">0</Ticket:Category>
      <Ticket:CategoryName xsi:type="xsd:string"></Ticket:CategoryName>
      <Ticket:CategoryFullname xsi:type="xsd:string"></Ticket:CategoryFullname>
      <Ticket:Slevel xsi:type="Ticket:TicketSecurityLevel">Unknown</Ticket:Slevel>
      <Ticket:Priority xsi:type="xsd:int">0</Ticket:Priority>
      <Ticket:PriorityName xsi:type="xsd:string"></Ticket:PriorityName>
      <Ticket:BaseStatus xsi:type="Ticket:TicketBaseStatus">Unknown</Ticket:BaseStatus>
      <Ticket:TicketStatus xsi:type="xsd:int">0</Ticket:TicketStatus>
      <Ticket:TicketStatusDisplayValue xsi:type="xsd:string"></Ticket:TicketStatusDisplayValue>
      <Ticket:Origin xsi:type="Ticket:TicketOrigin">Unknown</Ticket:Origin>
      <Ticket:CustId xsi:type="xsd:int">0</Ticket:CustId>
      <Ticket:PersonFirstname xsi:type="xsd:string"></Ticket:PersonFirstname>
      <Ticket:PersonMiddleName xsi:type="xsd:string"></Ticket:PersonMiddleName>
      <Ticket:PersonLastname xsi:type="xsd:string"></Ticket:PersonLastname>
      <Ticket:PersonFullname xsi:type="xsd:string"></Ticket:PersonFullname>
      <Ticket:AlertLevel xsi:type="xsd:short">0</Ticket:AlertLevel>
      <Ticket:ConnectId xsi:type="xsd:int">0</Ticket:ConnectId>
      <Ticket:ReadStatus xsi:type="Ticket:TicketReadStatus">Unknown</Ticket:ReadStatus>
      <Ticket:TimeToReply xsi:type="xsd:int">0</Ticket:TimeToReply>
      <Ticket:RealTimeToReply xsi:type="xsd:int">0</Ticket:RealTimeToReply>
      <Ticket:TimeToClose xsi:type="xsd:int">0</Ticket:TimeToClose>
      <Ticket:RealTimeToClose xsi:type="xsd:int">0</Ticket:RealTimeToClose>
      <Ticket:TimeSpentInternally xsi:type="xsd:int">0</Ticket:TimeSpentInternally>
      <Ticket:TimeSpentExternally xsi:type="xsd:int">0</Ticket:TimeSpentExternally>
      <Ticket:TimeSpentQueue xsi:type="xsd:int">0</Ticket:TimeSpentQueue>
      <Ticket:RealTimeSpentInternally xsi:type="xsd:int">0</Ticket:RealTimeSpentInternally>
      <Ticket:RealTimeSpentExternally xsi:type="xsd:int">0</Ticket:RealTimeSpentExternally>
      <Ticket:RealTimeSpentQueue xsi:type="xsd:int">0</Ticket:RealTimeSpentQueue>
      <Ticket:HasAttachment xsi:type="xsd:boolean">false</Ticket:HasAttachment>
      <Ticket:NumReplies xsi:type="xsd:int">0</Ticket:NumReplies>
      <Ticket:NumMessages xsi:type="xsd:int">0</Ticket:NumMessages>
      <Ticket:FromAddress xsi:type="xsd:string"></Ticket:FromAddress>
      <Ticket:ContactId xsi:type="xsd:int">0</Ticket:ContactId>
      <Ticket:ContactName xsi:type="xsd:string"></Ticket:ContactName>
      <Ticket:OwnedByAssociateId xsi:type="xsd:int">0</Ticket:OwnedByAssociateId>
      <Ticket:Language xsi:type="xsd:string"></Ticket:Language>
      <Ticket:Sentiment xsi:type="xsd:int">0</Ticket:Sentiment>
      <Ticket:SentimentConfidence xsi:type="xsd:int">0</Ticket:SentimentConfidence>
     </Ticket:Ticket>
     <Ticket:CreatedAt xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:CreatedAt>
     <Ticket:CreatedBy xsi:type="Ticket:Associate">
      <Ticket:AssociateId xsi:type="xsd:int">0</Ticket:AssociateId>
      <Ticket:Name xsi:type="xsd:string"></Ticket:Name>
      <Ticket:PersonId xsi:type="xsd:int">0</Ticket:PersonId>
      <Ticket:Rank xsi:type="xsd:short">0</Ticket:Rank>
      <Ticket:Tooltip xsi:type="xsd:string"></Ticket:Tooltip>
      <Ticket:Type xsi:type="Ticket:UserType">Unknown</Ticket:Type>
      <Ticket:GroupIdx xsi:type="xsd:int">0</Ticket:GroupIdx>
      <Ticket:FullName xsi:type="xsd:string"></Ticket:FullName>
      <Ticket:FormalName xsi:type="xsd:string"></Ticket:FormalName>
      <Ticket:Deleted xsi:type="xsd:boolean">false</Ticket:Deleted>
      <Ticket:EjUserId xsi:type="xsd:int">0</Ticket:EjUserId>
      <Ticket:UserName xsi:type="xsd:string"></Ticket:UserName>
     </Ticket:CreatedBy>
     <Ticket:Author xsi:type="xsd:string"></Ticket:Author>
     <Ticket:Slevel xsi:type="Ticket:TicketSecurityLevel">Unknown</Ticket:Slevel>
     <Ticket:Type xsi:type="Ticket:TicketMessageType">Unknown</Ticket:Type>
     <Ticket:MessageId xsi:type="xsd:string"></Ticket:MessageId>
     <Ticket:TimeSpent xsi:type="xsd:int">0</Ticket:TimeSpent>
     <Ticket:Body xsi:type="xsd:string"></Ticket:Body>
     <Ticket:HtmlBody xsi:type="xsd:string"></Ticket:HtmlBody>
     <Ticket:EmailHeader xsi:type="xsd:string"></Ticket:EmailHeader>
     <Ticket:DebugInfo xsi:type="xsd:string"></Ticket:DebugInfo>
     <Ticket:MailSorter xsi:type="xsd:string"></Ticket:MailSorter>
     <Ticket:MessageCategory xsi:type="Ticket:TicketMessageCategory">Message</Ticket:MessageCategory>
     <Ticket:Person xsi:type="Ticket:Person">
      <Ticket:Position xsi:type="xsd:string"></Ticket:Position>
      <Ticket:PersonId xsi:type="xsd:int">0</Ticket:PersonId>
      <Ticket:Mrmrs xsi:type="xsd:string"></Ticket:Mrmrs>
      <Ticket:Firstname xsi:type="xsd:string"></Ticket:Firstname>
      <Ticket:Lastname xsi:type="xsd:string"></Ticket:Lastname>
      <Ticket:MiddleName xsi:type="xsd:string"></Ticket:MiddleName>
      <Ticket:Title xsi:type="xsd:string"></Ticket:Title>
      <Ticket:Description xsi:type="xsd:string"></Ticket:Description>
      <Ticket:Email xsi:type="xsd:string"></Ticket:Email>
      <Ticket:FullName xsi:type="xsd:string"></Ticket:FullName>
      <Ticket:DirectPhone xsi:type="xsd:string"></Ticket:DirectPhone>
      <Ticket:FormalName xsi:type="xsd:string"></Ticket:FormalName>
      <Ticket:CountryId xsi:type="xsd:int">0</Ticket:CountryId>
      <Ticket:ContactId xsi:type="xsd:int">0</Ticket:ContactId>
      <Ticket:ContactName xsi:type="xsd:string"></Ticket:ContactName>
      <Ticket:Retired xsi:type="xsd:short">0</Ticket:Retired>
      <Ticket:Rank xsi:type="xsd:short">0</Ticket:Rank>
      <Ticket:ActiveInterests xsi:type="xsd:short">0</Ticket:ActiveInterests>
      <Ticket:ContactDepartment xsi:type="xsd:string"></Ticket:ContactDepartment>
      <Ticket:ContactCountryId xsi:type="xsd:int">0</Ticket:ContactCountryId>
      <Ticket:ContactOrgNr xsi:type="xsd:string"></Ticket:ContactOrgNr>
      <Ticket:FaxPhone xsi:type="xsd:string"></Ticket:FaxPhone>
      <Ticket:MobilePhone xsi:type="xsd:string"></Ticket:MobilePhone>
      <Ticket:ContactPhone xsi:type="xsd:string"></Ticket:ContactPhone>
      <Ticket:AssociateName xsi:type="xsd:string"></Ticket:AssociateName>
      <Ticket:AssociateId xsi:type="xsd:int">0</Ticket:AssociateId>
      <Ticket:UsePersonAddress xsi:type="xsd:boolean">false</Ticket:UsePersonAddress>
      <Ticket:ContactFax xsi:type="xsd:string"></Ticket:ContactFax>
      <Ticket:Kanafname xsi:type="xsd:string"></Ticket:Kanafname>
      <Ticket:Kanalname xsi:type="xsd:string"></Ticket:Kanalname>
      <Ticket:Post1 xsi:type="xsd:string"></Ticket:Post1>
      <Ticket:Post2 xsi:type="xsd:string"></Ticket:Post2>
      <Ticket:Post3 xsi:type="xsd:string"></Ticket:Post3>
      <Ticket:EmailName xsi:type="xsd:string"></Ticket:EmailName>
      <Ticket:ContactFullName xsi:type="xsd:string"></Ticket:ContactFullName>
      <Ticket:ActiveErpLinks xsi:type="xsd:int">0</Ticket:ActiveErpLinks>
      <Ticket:TicketPriorityId xsi:type="xsd:int">0</Ticket:TicketPriorityId>
      <Ticket:SupportLanguageId xsi:type="xsd:int">0</Ticket:SupportLanguageId>
      <Ticket:SupportAssociateId xsi:type="xsd:int">0</Ticket:SupportAssociateId>
      <Ticket:CategoryName xsi:type="xsd:string"></Ticket:CategoryName>
     </Ticket:Person>
     <Ticket:SearchTitle xsi:type="xsd:string"></Ticket:SearchTitle>
     <Ticket:MessageHeaders xsi:type="Ticket:ArrayOfTicketMessageHeader">
      <Ticket:TicketMessageHeader xsi:type="Ticket:TicketMessageHeader">
       <Ticket:Id xsi:type="xsd:int">0</Ticket:Id>
       <Ticket:Name xsi:type="xsd:string"></Ticket:Name>
       <Ticket:Value xsi:type="xsd:string"></Ticket:Value>
       <Ticket:StdItem xsi:type="Ticket:MessageHeaderStdItem">None</Ticket:StdItem>
       <Ticket:StdItemCol xsi:type="Ticket:MessageHeaderStdItemCol">None</Ticket:StdItemCol>
      </Ticket:TicketMessageHeader>
     </Ticket:MessageHeaders>
     <Ticket:Important xsi:type="xsd:boolean">false</Ticket:Important>
     <Ticket:Language xsi:type="xsd:string"></Ticket:Language>
     <Ticket:Sentiment xsi:type="xsd:int">0</Ticket:Sentiment>
     <Ticket:SentimentConfidence xsi:type="xsd:int">0</Ticket:SentimentConfidence>
     <Ticket:ExtraFields xsi:type="Ticket:StringDictionary">
      <Ticket:StringKeyValuePair>
       <Ticket:Key xsi:type="xsd:string"></Ticket:Key>
       <Ticket:Value xsi:type="xsd:string"></Ticket:Value>
      </Ticket:StringKeyValuePair>
     </Ticket:ExtraFields>
     <Ticket:CustomFields xsi:type="Ticket:StringDictionary">
      <Ticket:StringKeyValuePair>
       <Ticket:Key xsi:type="xsd:string"></Ticket:Key>
       <Ticket:Value xsi:type="xsd:string"></Ticket:Value>
      </Ticket:StringKeyValuePair>
     </Ticket:CustomFields>
    </Ticket:SourceTicketMessage>
    <Ticket:NewTicketEntity xsi:type="Ticket:TicketEntity">
     <Ticket:TicketId xsi:type="xsd:int">0</Ticket:TicketId>
     <Ticket:Title xsi:type="xsd:string"></Ticket:Title>
     <Ticket:CreatedAt xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:CreatedAt>
     <Ticket:LastChanged xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:LastChanged>
     <Ticket:ReadByOwner xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:ReadByOwner>
     <Ticket:ReadByCustomer xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:ReadByCustomer>
     <Ticket:FirstReadByOwner xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:FirstReadByOwner>
     <Ticket:FirstReadByUser xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:FirstReadByUser>
     <Ticket:Activate xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:Activate>
     <Ticket:ClosedAt xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:ClosedAt>
     <Ticket:RepliedAt xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:RepliedAt>
     <Ticket:AlertTimeout xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:AlertTimeout>
     <Ticket:Deadline xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:Deadline>
     <Ticket:CreatedBy xsi:type="Ticket:Associate">
      <Ticket:AssociateId xsi:type="xsd:int">0</Ticket:AssociateId>
      <Ticket:Name xsi:type="xsd:string"></Ticket:Name>
      <Ticket:PersonId xsi:type="xsd:int">0</Ticket:PersonId>
      <Ticket:Rank xsi:type="xsd:short">0</Ticket:Rank>
      <Ticket:Tooltip xsi:type="xsd:string"></Ticket:Tooltip>
      <Ticket:Type xsi:type="Ticket:UserType">Unknown</Ticket:Type>
      <Ticket:GroupIdx xsi:type="xsd:int">0</Ticket:GroupIdx>
      <Ticket:FullName xsi:type="xsd:string"></Ticket:FullName>
      <Ticket:FormalName xsi:type="xsd:string"></Ticket:FormalName>
      <Ticket:Deleted xsi:type="xsd:boolean">false</Ticket:Deleted>
      <Ticket:EjUserId xsi:type="xsd:int">0</Ticket:EjUserId>
      <Ticket:UserName xsi:type="xsd:string"></Ticket:UserName>
     </Ticket:CreatedBy>
     <Ticket:Author xsi:type="xsd:string"></Ticket:Author>
     <Ticket:OwnedBy xsi:type="Ticket:Associate">
      <Ticket:AssociateId xsi:type="xsd:int">0</Ticket:AssociateId>
      <Ticket:Name xsi:type="xsd:string"></Ticket:Name>
      <Ticket:PersonId xsi:type="xsd:int">0</Ticket:PersonId>
      <Ticket:Rank xsi:type="xsd:short">0</Ticket:Rank>
      <Ticket:Tooltip xsi:type="xsd:string"></Ticket:Tooltip>
      <Ticket:Type xsi:type="Ticket:UserType">Unknown</Ticket:Type>
      <Ticket:GroupIdx xsi:type="xsd:int">0</Ticket:GroupIdx>
      <Ticket:FullName xsi:type="xsd:string"></Ticket:FullName>
      <Ticket:FormalName xsi:type="xsd:string"></Ticket:FormalName>
      <Ticket:Deleted xsi:type="xsd:boolean">false</Ticket:Deleted>
      <Ticket:EjUserId xsi:type="xsd:int">0</Ticket:EjUserId>
      <Ticket:UserName xsi:type="xsd:string"></Ticket:UserName>
     </Ticket:OwnedBy>
     <Ticket:Category xsi:type="Ticket:TicketCategoryEntity">
      <Ticket:TicketCategoryId xsi:type="xsd:int">0</Ticket:TicketCategoryId>
      <Ticket:ParentId xsi:type="xsd:int">0</Ticket:ParentId>
      <Ticket:Name xsi:type="xsd:string"></Ticket:Name>
      <Ticket:Fullname xsi:type="xsd:string"></Ticket:Fullname>
      <Ticket:CategoryMaster xsi:type="xsd:int">0</Ticket:CategoryMaster>
      <Ticket:Flags xsi:type="Ticket:TicketCategoryFlags">Internal</Ticket:Flags>
      <Ticket:DelegateMethod xsi:type="Ticket:TicketCategoryDelegateMethod">Unknown</Ticket:DelegateMethod>
      <Ticket:ExternalName xsi:type="xsd:string"></Ticket:ExternalName>
      <Ticket:ClosingStatus xsi:type="Ticket:TicketCategoryClosingStatus">UserDefined</Ticket:ClosingStatus>
      <Ticket:MsgClosingStatus xsi:type="Ticket:TicketCategoryClosingStatus">UserDefined</Ticket:MsgClosingStatus>
      <Ticket:AssignmentLag xsi:type="xsd:int">0</Ticket:AssignmentLag>
      <Ticket:ReplyTemplate xsi:type="xsd:int">0</Ticket:ReplyTemplate>
      <Ticket:NotificationEmail xsi:type="xsd:string"></Ticket:NotificationEmail>
      <Ticket:DefaultTicketStatus xsi:type="Ticket:TicketStatusEntity">
       <Ticket:TicketStatusId xsi:type="xsd:int">0</Ticket:TicketStatusId>
       <Ticket:Name xsi:type="xsd:string"></Ticket:Name>
       <Ticket:Status xsi:type="Ticket:TicketBaseStatus">Unknown</Ticket:Status>
       <Ticket:TimeCounter xsi:type="Ticket:TicketStatusTimeCounter">None</Ticket:TimeCounter>
       <Ticket:NoEmailReopen xsi:type="xsd:boolean">false</Ticket:NoEmailReopen>
       <Ticket:IsDefault xsi:type="xsd:boolean">false</Ticket:IsDefault>
       <Ticket:UsedInQueue xsi:type="xsd:boolean">false</Ticket:UsedInQueue>
      </Ticket:DefaultTicketStatus>
      <Ticket:DefaultMessageStatus xsi:type="Ticket:TicketStatusEntity">
       <Ticket:TicketStatusId xsi:type="xsd:int">0</Ticket:TicketStatusId>
       <Ticket:Name xsi:type="xsd:string"></Ticket:Name>
       <Ticket:Status xsi:type="Ticket:TicketBaseStatus">Unknown</Ticket:Status>
       <Ticket:TimeCounter xsi:type="Ticket:TicketStatusTimeCounter">None</Ticket:TimeCounter>
       <Ticket:NoEmailReopen xsi:type="xsd:boolean">false</Ticket:NoEmailReopen>
       <Ticket:IsDefault xsi:type="xsd:boolean">false</Ticket:IsDefault>
       <Ticket:UsedInQueue xsi:type="xsd:boolean">false</Ticket:UsedInQueue>
      </Ticket:DefaultMessageStatus>
      <Ticket:EffectiveReplyTemplateId xsi:type="xsd:int">0</Ticket:EffectiveReplyTemplateId>
      <Ticket:ExtraFields xsi:type="Ticket:StringDictionary">
       <Ticket:StringKeyValuePair>
        <Ticket:Key xsi:type="xsd:string"></Ticket:Key>
        <Ticket:Value xsi:type="xsd:string"></Ticket:Value>
       </Ticket:StringKeyValuePair>
      </Ticket:ExtraFields>
      <Ticket:CustomFields xsi:type="Ticket:StringDictionary">
       <Ticket:StringKeyValuePair>
        <Ticket:Key xsi:type="xsd:string"></Ticket:Key>
        <Ticket:Value xsi:type="xsd:string"></Ticket:Value>
       </Ticket:StringKeyValuePair>
      </Ticket:CustomFields>
     </Ticket:Category>
     <Ticket:Slevel xsi:type="Ticket:TicketSecurityLevel">Unknown</Ticket:Slevel>
     <Ticket:Priority xsi:type="Ticket:TicketPriorityEntity">
      <Ticket:TicketPriorityId xsi:type="xsd:int">0</Ticket:TicketPriorityId>
      <Ticket:Name xsi:type="xsd:string"></Ticket:Name>
      <Ticket:Status xsi:type="Ticket:TicketPriorityStatus">Unknown</Ticket:Status>
      <Ticket:Flags xsi:type="Ticket:TicketPriorityFlags">External</Ticket:Flags>
      <Ticket:SortOrder xsi:type="xsd:int">0</Ticket:SortOrder>
      <Ticket:TicketRead xsi:type="Ticket:TicketPriorityEscalateEvent">None</Ticket:TicketRead>
      <Ticket:ChangedOwner xsi:type="Ticket:TicketPriorityEscalateEvent">None</Ticket:ChangedOwner>
      <Ticket:TicketNewinfo xsi:type="Ticket:TicketPriorityEscalateEvent">None</Ticket:TicketNewinfo>
      <Ticket:TicketClosed xsi:type="Ticket:TicketPriorityEscalateEvent">None</Ticket:TicketClosed>
      <Ticket:TicketChangedPriority xsi:type="Ticket:TicketPriorityEscalateEvent">None</Ticket:TicketChangedPriority>
      <Ticket:TicketNew xsi:type="Ticket:TicketPriorityEscalateEvent">None</Ticket:TicketNew>
      <Ticket:Deadline xsi:type="xsd:int">0</Ticket:Deadline>
      <Ticket:MonStart xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:MonStart>
      <Ticket:MonStop xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:MonStop>
      <Ticket:TueStart xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:TueStart>
      <Ticket:TueStop xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:TueStop>
      <Ticket:WedStart xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:WedStart>
      <Ticket:WedStop xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:WedStop>
      <Ticket:ThuStart xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:ThuStart>
      <Ticket:ThuStop xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:ThuStop>
      <Ticket:FriStart xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:FriStart>
      <Ticket:FriStop xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:FriStop>
      <Ticket:SatStart xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:SatStart>
      <Ticket:SatStop xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:SatStop>
      <Ticket:SunStart xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:SunStart>
      <Ticket:SunStop xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:SunStop>
      <Ticket:NonDates xsi:type="NetServerServices882:ArrayOfdateTime">
       <NetServerServices882:dateTime xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</NetServerServices882:dateTime>
      </Ticket:NonDates>
      <Ticket:EscalationLevels xsi:type="Ticket:ArrayOfTicketPriorityEscalationLevelEntity">
       <Ticket:TicketPriorityEscalationLevelEntity xsi:type="Ticket:TicketPriorityEscalationLevelEntity">
        <Ticket:TicketAlertId xsi:type="xsd:int">0</Ticket:TicketAlertId>
        <Ticket:AlertLevel xsi:type="xsd:short">0</Ticket:AlertLevel>
        <Ticket:AlertTimeout xsi:type="xsd:int">0</Ticket:AlertTimeout>
        <Ticket:Action xsi:type="xsd:int">0</Ticket:Action>
        <Ticket:DelegateTo xsi:type="xsd:int">0</Ticket:DelegateTo>
        <Ticket:ScriptId xsi:type="xsd:int">0</Ticket:ScriptId>
        <Ticket:EmailTo xsi:type="xsd:string"></Ticket:EmailTo>
        <Ticket:SmsTo xsi:type="xsd:string"></Ticket:SmsTo>
        <Ticket:ReplyTemplateIdCustomer xsi:type="xsd:int">0</Ticket:ReplyTemplateIdCustomer>
        <Ticket:ReplyTemplateIdUser xsi:type="xsd:int">0</Ticket:ReplyTemplateIdUser>
        <Ticket:ReplyTemplateIdCatmast xsi:type="xsd:int">0</Ticket:ReplyTemplateIdCatmast>
        <Ticket:ReplyTemplateIdEmail xsi:type="xsd:int">0</Ticket:ReplyTemplateIdEmail>
        <Ticket:RtiCustomerSms xsi:type="xsd:int">0</Ticket:RtiCustomerSms>
        <Ticket:ReplyTemplateIdUserSms xsi:type="xsd:int">0</Ticket:ReplyTemplateIdUserSms>
        <Ticket:ReplyTemplateIdCatmastSms xsi:type="xsd:int">0</Ticket:ReplyTemplateIdCatmastSms>
        <Ticket:ReplyTemplateIdSms xsi:type="xsd:int">0</Ticket:ReplyTemplateIdSms>
       </Ticket:TicketPriorityEscalationLevelEntity>
      </Ticket:EscalationLevels>
     </Ticket:Priority>
     <Ticket:BaseStatus xsi:type="Ticket:TicketBaseStatus">Unknown</Ticket:BaseStatus>
     <Ticket:Status xsi:type="Ticket:TicketStatusEntity">
      <Ticket:TicketStatusId xsi:type="xsd:int">0</Ticket:TicketStatusId>
      <Ticket:Name xsi:type="xsd:string"></Ticket:Name>
      <Ticket:Status xsi:type="Ticket:TicketBaseStatus">Unknown</Ticket:Status>
      <Ticket:TimeCounter xsi:type="Ticket:TicketStatusTimeCounter">None</Ticket:TimeCounter>
      <Ticket:NoEmailReopen xsi:type="xsd:boolean">false</Ticket:NoEmailReopen>
      <Ticket:IsDefault xsi:type="xsd:boolean">false</Ticket:IsDefault>
      <Ticket:UsedInQueue xsi:type="xsd:boolean">false</Ticket:UsedInQueue>
     </Ticket:Status>
     <Ticket:Origin xsi:type="Ticket:TicketOrigin">Unknown</Ticket:Origin>
     <Ticket:Person xsi:type="Ticket:Person">
      <Ticket:Position xsi:type="xsd:string"></Ticket:Position>
      <Ticket:PersonId xsi:type="xsd:int">0</Ticket:PersonId>
      <Ticket:Mrmrs xsi:type="xsd:string"></Ticket:Mrmrs>
      <Ticket:Firstname xsi:type="xsd:string"></Ticket:Firstname>
      <Ticket:Lastname xsi:type="xsd:string"></Ticket:Lastname>
      <Ticket:MiddleName xsi:type="xsd:string"></Ticket:MiddleName>
      <Ticket:Title xsi:type="xsd:string"></Ticket:Title>
      <Ticket:Description xsi:type="xsd:string"></Ticket:Description>
      <Ticket:Email xsi:type="xsd:string"></Ticket:Email>
      <Ticket:FullName xsi:type="xsd:string"></Ticket:FullName>
      <Ticket:DirectPhone xsi:type="xsd:string"></Ticket:DirectPhone>
      <Ticket:FormalName xsi:type="xsd:string"></Ticket:FormalName>
      <Ticket:CountryId xsi:type="xsd:int">0</Ticket:CountryId>
      <Ticket:ContactId xsi:type="xsd:int">0</Ticket:ContactId>
      <Ticket:ContactName xsi:type="xsd:string"></Ticket:ContactName>
      <Ticket:Retired xsi:type="xsd:short">0</Ticket:Retired>
      <Ticket:Rank xsi:type="xsd:short">0</Ticket:Rank>
      <Ticket:ActiveInterests xsi:type="xsd:short">0</Ticket:ActiveInterests>
      <Ticket:ContactDepartment xsi:type="xsd:string"></Ticket:ContactDepartment>
      <Ticket:ContactCountryId xsi:type="xsd:int">0</Ticket:ContactCountryId>
      <Ticket:ContactOrgNr xsi:type="xsd:string"></Ticket:ContactOrgNr>
      <Ticket:FaxPhone xsi:type="xsd:string"></Ticket:FaxPhone>
      <Ticket:MobilePhone xsi:type="xsd:string"></Ticket:MobilePhone>
      <Ticket:ContactPhone xsi:type="xsd:string"></Ticket:ContactPhone>
      <Ticket:AssociateName xsi:type="xsd:string"></Ticket:AssociateName>
      <Ticket:AssociateId xsi:type="xsd:int">0</Ticket:AssociateId>
      <Ticket:UsePersonAddress xsi:type="xsd:boolean">false</Ticket:UsePersonAddress>
      <Ticket:ContactFax xsi:type="xsd:string"></Ticket:ContactFax>
      <Ticket:Kanafname xsi:type="xsd:string"></Ticket:Kanafname>
      <Ticket:Kanalname xsi:type="xsd:string"></Ticket:Kanalname>
      <Ticket:Post1 xsi:type="xsd:string"></Ticket:Post1>
      <Ticket:Post2 xsi:type="xsd:string"></Ticket:Post2>
      <Ticket:Post3 xsi:type="xsd:string"></Ticket:Post3>
      <Ticket:EmailName xsi:type="xsd:string"></Ticket:EmailName>
      <Ticket:ContactFullName xsi:type="xsd:string"></Ticket:ContactFullName>
      <Ticket:ActiveErpLinks xsi:type="xsd:int">0</Ticket:ActiveErpLinks>
      <Ticket:TicketPriorityId xsi:type="xsd:int">0</Ticket:TicketPriorityId>
      <Ticket:SupportLanguageId xsi:type="xsd:int">0</Ticket:SupportLanguageId>
      <Ticket:SupportAssociateId xsi:type="xsd:int">0</Ticket:SupportAssociateId>
      <Ticket:CategoryName xsi:type="xsd:string"></Ticket:CategoryName>
     </Ticket:Person>
     <Ticket:SecondaryPersons xsi:type="Ticket:ArrayOfPerson">
      <Ticket:Person xsi:type="Ticket:Person">
       <Ticket:Position xsi:type="xsd:string"></Ticket:Position>
       <Ticket:PersonId xsi:type="xsd:int">0</Ticket:PersonId>
       <Ticket:Mrmrs xsi:type="xsd:string"></Ticket:Mrmrs>
       <Ticket:Firstname xsi:type="xsd:string"></Ticket:Firstname>
       <Ticket:Lastname xsi:type="xsd:string"></Ticket:Lastname>
       <Ticket:MiddleName xsi:type="xsd:string"></Ticket:MiddleName>
       <Ticket:Title xsi:type="xsd:string"></Ticket:Title>
       <Ticket:Description xsi:type="xsd:string"></Ticket:Description>
       <Ticket:Email xsi:type="xsd:string"></Ticket:Email>
       <Ticket:FullName xsi:type="xsd:string"></Ticket:FullName>
       <Ticket:DirectPhone xsi:type="xsd:string"></Ticket:DirectPhone>
       <Ticket:FormalName xsi:type="xsd:string"></Ticket:FormalName>
       <Ticket:CountryId xsi:type="xsd:int">0</Ticket:CountryId>
       <Ticket:ContactId xsi:type="xsd:int">0</Ticket:ContactId>
       <Ticket:ContactName xsi:type="xsd:string"></Ticket:ContactName>
       <Ticket:Retired xsi:type="xsd:short">0</Ticket:Retired>
       <Ticket:Rank xsi:type="xsd:short">0</Ticket:Rank>
       <Ticket:ActiveInterests xsi:type="xsd:short">0</Ticket:ActiveInterests>
       <Ticket:ContactDepartment xsi:type="xsd:string"></Ticket:ContactDepartment>
       <Ticket:ContactCountryId xsi:type="xsd:int">0</Ticket:ContactCountryId>
       <Ticket:ContactOrgNr xsi:type="xsd:string"></Ticket:ContactOrgNr>
       <Ticket:FaxPhone xsi:type="xsd:string"></Ticket:FaxPhone>
       <Ticket:MobilePhone xsi:type="xsd:string"></Ticket:MobilePhone>
       <Ticket:ContactPhone xsi:type="xsd:string"></Ticket:ContactPhone>
       <Ticket:AssociateName xsi:type="xsd:string"></Ticket:AssociateName>
       <Ticket:AssociateId xsi:type="xsd:int">0</Ticket:AssociateId>
       <Ticket:UsePersonAddress xsi:type="xsd:boolean">false</Ticket:UsePersonAddress>
       <Ticket:ContactFax xsi:type="xsd:string"></Ticket:ContactFax>
       <Ticket:Kanafname xsi:type="xsd:string"></Ticket:Kanafname>
       <Ticket:Kanalname xsi:type="xsd:string"></Ticket:Kanalname>
       <Ticket:Post1 xsi:type="xsd:string"></Ticket:Post1>
       <Ticket:Post2 xsi:type="xsd:string"></Ticket:Post2>
       <Ticket:Post3 xsi:type="xsd:string"></Ticket:Post3>
       <Ticket:EmailName xsi:type="xsd:string"></Ticket:EmailName>
       <Ticket:ContactFullName xsi:type="xsd:string"></Ticket:ContactFullName>
       <Ticket:ActiveErpLinks xsi:type="xsd:int">0</Ticket:ActiveErpLinks>
       <Ticket:TicketPriorityId xsi:type="xsd:int">0</Ticket:TicketPriorityId>
       <Ticket:SupportLanguageId xsi:type="xsd:int">0</Ticket:SupportLanguageId>
       <Ticket:SupportAssociateId xsi:type="xsd:int">0</Ticket:SupportAssociateId>
       <Ticket:CategoryName xsi:type="xsd:string"></Ticket:CategoryName>
      </Ticket:Person>
     </Ticket:SecondaryPersons>
     <Ticket:AlertLevel xsi:type="xsd:short">0</Ticket:AlertLevel>
     <Ticket:ConnectId xsi:type="xsd:int">0</Ticket:ConnectId>
     <Ticket:ReadStatus xsi:type="Ticket:TicketReadStatus">Unknown</Ticket:ReadStatus>
     <Ticket:TimeToReply xsi:type="xsd:int">0</Ticket:TimeToReply>
     <Ticket:RealTimeToReply xsi:type="xsd:int">0</Ticket:RealTimeToReply>
     <Ticket:TimeToClose xsi:type="xsd:int">0</Ticket:TimeToClose>
     <Ticket:RealTimeToClose xsi:type="xsd:int">0</Ticket:RealTimeToClose>
     <Ticket:TimeSpentInternally xsi:type="xsd:int">0</Ticket:TimeSpentInternally>
     <Ticket:TimeSpentExternally xsi:type="xsd:int">0</Ticket:TimeSpentExternally>
     <Ticket:TimeSpentQueue xsi:type="xsd:int">0</Ticket:TimeSpentQueue>
     <Ticket:RealTimeSpentInternally xsi:type="xsd:int">0</Ticket:RealTimeSpentInternally>
     <Ticket:RealTimeSpentExternally xsi:type="xsd:int">0</Ticket:RealTimeSpentExternally>
     <Ticket:RealTimeSpentQueue xsi:type="xsd:int">0</Ticket:RealTimeSpentQueue>
     <Ticket:HasAttachment xsi:type="xsd:boolean">false</Ticket:HasAttachment>
     <Ticket:NumReplies xsi:type="xsd:int">0</Ticket:NumReplies>
     <Ticket:NumMessages xsi:type="xsd:int">0</Ticket:NumMessages>
     <Ticket:FromAddress xsi:type="xsd:string"></Ticket:FromAddress>
     <Ticket:Messages xsi:type="Ticket:ArrayOfTicketMessage">
      <Ticket:TicketMessage xsi:type="Ticket:TicketMessage">
       <Ticket:TicketMessageId xsi:type="xsd:int">0</Ticket:TicketMessageId>
       <Ticket:CreatedAt xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:CreatedAt>
       <Ticket:Slevel xsi:type="Ticket:TicketSecurityLevel">Unknown</Ticket:Slevel>
       <Ticket:Important xsi:type="xsd:boolean">false</Ticket:Important>
       <Ticket:Author xsi:type="xsd:string"></Ticket:Author>
       <Ticket:PersonId xsi:type="xsd:int">0</Ticket:PersonId>
       <Ticket:PersonFullName xsi:type="xsd:string"></Ticket:PersonFullName>
       <Ticket:ContactId xsi:type="xsd:int">0</Ticket:ContactId>
       <Ticket:ContactName xsi:type="xsd:string"></Ticket:ContactName>
       <Ticket:ContactDepartment xsi:type="xsd:string"></Ticket:ContactDepartment>
       <Ticket:NumAttachments xsi:type="xsd:int">0</Ticket:NumAttachments>
       <Ticket:EmailHeader xsi:type="xsd:string"></Ticket:EmailHeader>
       <Ticket:MessageHeaders xsi:type="Ticket:ArrayOfTicketMessageHeader">
        <Ticket:TicketMessageHeader xsi:type="Ticket:TicketMessageHeader">
         <Ticket:Id xsi:type="xsd:int">0</Ticket:Id>
         <Ticket:Name xsi:type="xsd:string"></Ticket:Name>
         <Ticket:Value xsi:type="xsd:string"></Ticket:Value>
         <Ticket:StdItem xsi:type="Ticket:MessageHeaderStdItem">None</Ticket:StdItem>
         <Ticket:StdItemCol xsi:type="Ticket:MessageHeaderStdItemCol">None</Ticket:StdItemCol>
        </Ticket:TicketMessageHeader>
       </Ticket:MessageHeaders>
       <Ticket:Language xsi:type="xsd:string"></Ticket:Language>
       <Ticket:Sentiment xsi:type="xsd:int">0</Ticket:Sentiment>
       <Ticket:SentimentConfidence xsi:type="xsd:int">0</Ticket:SentimentConfidence>
       <Ticket:CreatedBy xsi:type="xsd:int">0</Ticket:CreatedBy>
       <Ticket:ChangedAt xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:ChangedAt>
      </Ticket:TicketMessage>
     </Ticket:Messages>
     <Ticket:Tags xsi:type="Ticket:ArrayOfTag">
      <Ticket:Tag xsi:type="Ticket:Tag">
       <Ticket:Id xsi:type="xsd:int">0</Ticket:Id>
       <Ticket:Name xsi:type="xsd:string"></Ticket:Name>
       <Ticket:ToolTip xsi:type="xsd:string"></Ticket:ToolTip>
      </Ticket:Tag>
     </Ticket:Tags>
     <Ticket:Language xsi:type="xsd:string"></Ticket:Language>
     <Ticket:Sentiment xsi:type="xsd:int">0</Ticket:Sentiment>
     <Ticket:SentimentConfidence xsi:type="xsd:int">0</Ticket:SentimentConfidence>
     <Ticket:SuggestedCategoryId xsi:type="xsd:int">0</Ticket:SuggestedCategoryId>
     <Ticket:SuggestedCategoryName xsi:type="xsd:string"></Ticket:SuggestedCategoryName>
     <Ticket:OrigHumanCategoryId xsi:type="xsd:int">0</Ticket:OrigHumanCategoryId>
     <Ticket:IconHint xsi:type="xsd:string"></Ticket:IconHint>
     <Ticket:ExtraFields xsi:type="Ticket:StringDictionary">
      <Ticket:StringKeyValuePair>
       <Ticket:Key xsi:type="xsd:string"></Ticket:Key>
       <Ticket:Value xsi:type="xsd:string"></Ticket:Value>
      </Ticket:StringKeyValuePair>
     </Ticket:ExtraFields>
     <Ticket:CustomFields xsi:type="Ticket:StringDictionary">
      <Ticket:StringKeyValuePair>
       <Ticket:Key xsi:type="xsd:string"></Ticket:Key>
       <Ticket:Value xsi:type="xsd:string"></Ticket:Value>
      </Ticket:StringKeyValuePair>
     </Ticket:CustomFields>
    </Ticket:NewTicketEntity>
    <Ticket:NewTicketMessage xsi:type="Ticket:TicketMessageEntity">
     <Ticket:EjMessageId xsi:type="xsd:int">0</Ticket:EjMessageId>
     <Ticket:Ticket xsi:type="Ticket:Ticket">
      <Ticket:TicketId xsi:type="xsd:int">0</Ticket:TicketId>
      <Ticket:Title xsi:type="xsd:string"></Ticket:Title>
      <Ticket:CreatedAt xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:CreatedAt>
      <Ticket:LastChanged xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:LastChanged>
      <Ticket:ReadByOwner xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:ReadByOwner>
      <Ticket:ReadByCustomer xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:ReadByCustomer>
      <Ticket:FirstReadByUser xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:FirstReadByUser>
      <Ticket:Activate xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:Activate>
      <Ticket:ClosedAt xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:ClosedAt>
      <Ticket:RepliedAt xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:RepliedAt>
      <Ticket:AlertTimeout xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:AlertTimeout>
      <Ticket:Deadline xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:Deadline>
      <Ticket:CreatedBy xsi:type="xsd:int">0</Ticket:CreatedBy>
      <Ticket:CreatedByName xsi:type="xsd:string"></Ticket:CreatedByName>
      <Ticket:Author xsi:type="xsd:string"></Ticket:Author>
      <Ticket:OwnedBy xsi:type="xsd:int">0</Ticket:OwnedBy>
      <Ticket:OwnedByName xsi:type="xsd:string"></Ticket:OwnedByName>
      <Ticket:Category xsi:type="xsd:int">0</Ticket:Category>
      <Ticket:CategoryName xsi:type="xsd:string"></Ticket:CategoryName>
      <Ticket:CategoryFullname xsi:type="xsd:string"></Ticket:CategoryFullname>
      <Ticket:Slevel xsi:type="Ticket:TicketSecurityLevel">Unknown</Ticket:Slevel>
      <Ticket:Priority xsi:type="xsd:int">0</Ticket:Priority>
      <Ticket:PriorityName xsi:type="xsd:string"></Ticket:PriorityName>
      <Ticket:BaseStatus xsi:type="Ticket:TicketBaseStatus">Unknown</Ticket:BaseStatus>
      <Ticket:TicketStatus xsi:type="xsd:int">0</Ticket:TicketStatus>
      <Ticket:TicketStatusDisplayValue xsi:type="xsd:string"></Ticket:TicketStatusDisplayValue>
      <Ticket:Origin xsi:type="Ticket:TicketOrigin">Unknown</Ticket:Origin>
      <Ticket:CustId xsi:type="xsd:int">0</Ticket:CustId>
      <Ticket:PersonFirstname xsi:type="xsd:string"></Ticket:PersonFirstname>
      <Ticket:PersonMiddleName xsi:type="xsd:string"></Ticket:PersonMiddleName>
      <Ticket:PersonLastname xsi:type="xsd:string"></Ticket:PersonLastname>
      <Ticket:PersonFullname xsi:type="xsd:string"></Ticket:PersonFullname>
      <Ticket:AlertLevel xsi:type="xsd:short">0</Ticket:AlertLevel>
      <Ticket:ConnectId xsi:type="xsd:int">0</Ticket:ConnectId>
      <Ticket:ReadStatus xsi:type="Ticket:TicketReadStatus">Unknown</Ticket:ReadStatus>
      <Ticket:TimeToReply xsi:type="xsd:int">0</Ticket:TimeToReply>
      <Ticket:RealTimeToReply xsi:type="xsd:int">0</Ticket:RealTimeToReply>
      <Ticket:TimeToClose xsi:type="xsd:int">0</Ticket:TimeToClose>
      <Ticket:RealTimeToClose xsi:type="xsd:int">0</Ticket:RealTimeToClose>
      <Ticket:TimeSpentInternally xsi:type="xsd:int">0</Ticket:TimeSpentInternally>
      <Ticket:TimeSpentExternally xsi:type="xsd:int">0</Ticket:TimeSpentExternally>
      <Ticket:TimeSpentQueue xsi:type="xsd:int">0</Ticket:TimeSpentQueue>
      <Ticket:RealTimeSpentInternally xsi:type="xsd:int">0</Ticket:RealTimeSpentInternally>
      <Ticket:RealTimeSpentExternally xsi:type="xsd:int">0</Ticket:RealTimeSpentExternally>
      <Ticket:RealTimeSpentQueue xsi:type="xsd:int">0</Ticket:RealTimeSpentQueue>
      <Ticket:HasAttachment xsi:type="xsd:boolean">false</Ticket:HasAttachment>
      <Ticket:NumReplies xsi:type="xsd:int">0</Ticket:NumReplies>
      <Ticket:NumMessages xsi:type="xsd:int">0</Ticket:NumMessages>
      <Ticket:FromAddress xsi:type="xsd:string"></Ticket:FromAddress>
      <Ticket:ContactId xsi:type="xsd:int">0</Ticket:ContactId>
      <Ticket:ContactName xsi:type="xsd:string"></Ticket:ContactName>
      <Ticket:OwnedByAssociateId xsi:type="xsd:int">0</Ticket:OwnedByAssociateId>
      <Ticket:Language xsi:type="xsd:string"></Ticket:Language>
      <Ticket:Sentiment xsi:type="xsd:int">0</Ticket:Sentiment>
      <Ticket:SentimentConfidence xsi:type="xsd:int">0</Ticket:SentimentConfidence>
     </Ticket:Ticket>
     <Ticket:CreatedAt xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:CreatedAt>
     <Ticket:CreatedBy xsi:type="Ticket:Associate">
      <Ticket:AssociateId xsi:type="xsd:int">0</Ticket:AssociateId>
      <Ticket:Name xsi:type="xsd:string"></Ticket:Name>
      <Ticket:PersonId xsi:type="xsd:int">0</Ticket:PersonId>
      <Ticket:Rank xsi:type="xsd:short">0</Ticket:Rank>
      <Ticket:Tooltip xsi:type="xsd:string"></Ticket:Tooltip>
      <Ticket:Type xsi:type="Ticket:UserType">Unknown</Ticket:Type>
      <Ticket:GroupIdx xsi:type="xsd:int">0</Ticket:GroupIdx>
      <Ticket:FullName xsi:type="xsd:string"></Ticket:FullName>
      <Ticket:FormalName xsi:type="xsd:string"></Ticket:FormalName>
      <Ticket:Deleted xsi:type="xsd:boolean">false</Ticket:Deleted>
      <Ticket:EjUserId xsi:type="xsd:int">0</Ticket:EjUserId>
      <Ticket:UserName xsi:type="xsd:string"></Ticket:UserName>
     </Ticket:CreatedBy>
     <Ticket:Author xsi:type="xsd:string"></Ticket:Author>
     <Ticket:Slevel xsi:type="Ticket:TicketSecurityLevel">Unknown</Ticket:Slevel>
     <Ticket:Type xsi:type="Ticket:TicketMessageType">Unknown</Ticket:Type>
     <Ticket:MessageId xsi:type="xsd:string"></Ticket:MessageId>
     <Ticket:TimeSpent xsi:type="xsd:int">0</Ticket:TimeSpent>
     <Ticket:Body xsi:type="xsd:string"></Ticket:Body>
     <Ticket:HtmlBody xsi:type="xsd:string"></Ticket:HtmlBody>
     <Ticket:EmailHeader xsi:type="xsd:string"></Ticket:EmailHeader>
     <Ticket:DebugInfo xsi:type="xsd:string"></Ticket:DebugInfo>
     <Ticket:MailSorter xsi:type="xsd:string"></Ticket:MailSorter>
     <Ticket:MessageCategory xsi:type="Ticket:TicketMessageCategory">Message</Ticket:MessageCategory>
     <Ticket:Person xsi:type="Ticket:Person">
      <Ticket:Position xsi:type="xsd:string"></Ticket:Position>
      <Ticket:PersonId xsi:type="xsd:int">0</Ticket:PersonId>
      <Ticket:Mrmrs xsi:type="xsd:string"></Ticket:Mrmrs>
      <Ticket:Firstname xsi:type="xsd:string"></Ticket:Firstname>
      <Ticket:Lastname xsi:type="xsd:string"></Ticket:Lastname>
      <Ticket:MiddleName xsi:type="xsd:string"></Ticket:MiddleName>
      <Ticket:Title xsi:type="xsd:string"></Ticket:Title>
      <Ticket:Description xsi:type="xsd:string"></Ticket:Description>
      <Ticket:Email xsi:type="xsd:string"></Ticket:Email>
      <Ticket:FullName xsi:type="xsd:string"></Ticket:FullName>
      <Ticket:DirectPhone xsi:type="xsd:string"></Ticket:DirectPhone>
      <Ticket:FormalName xsi:type="xsd:string"></Ticket:FormalName>
      <Ticket:CountryId xsi:type="xsd:int">0</Ticket:CountryId>
      <Ticket:ContactId xsi:type="xsd:int">0</Ticket:ContactId>
      <Ticket:ContactName xsi:type="xsd:string"></Ticket:ContactName>
      <Ticket:Retired xsi:type="xsd:short">0</Ticket:Retired>
      <Ticket:Rank xsi:type="xsd:short">0</Ticket:Rank>
      <Ticket:ActiveInterests xsi:type="xsd:short">0</Ticket:ActiveInterests>
      <Ticket:ContactDepartment xsi:type="xsd:string"></Ticket:ContactDepartment>
      <Ticket:ContactCountryId xsi:type="xsd:int">0</Ticket:ContactCountryId>
      <Ticket:ContactOrgNr xsi:type="xsd:string"></Ticket:ContactOrgNr>
      <Ticket:FaxPhone xsi:type="xsd:string"></Ticket:FaxPhone>
      <Ticket:MobilePhone xsi:type="xsd:string"></Ticket:MobilePhone>
      <Ticket:ContactPhone xsi:type="xsd:string"></Ticket:ContactPhone>
      <Ticket:AssociateName xsi:type="xsd:string"></Ticket:AssociateName>
      <Ticket:AssociateId xsi:type="xsd:int">0</Ticket:AssociateId>
      <Ticket:UsePersonAddress xsi:type="xsd:boolean">false</Ticket:UsePersonAddress>
      <Ticket:ContactFax xsi:type="xsd:string"></Ticket:ContactFax>
      <Ticket:Kanafname xsi:type="xsd:string"></Ticket:Kanafname>
      <Ticket:Kanalname xsi:type="xsd:string"></Ticket:Kanalname>
      <Ticket:Post1 xsi:type="xsd:string"></Ticket:Post1>
      <Ticket:Post2 xsi:type="xsd:string"></Ticket:Post2>
      <Ticket:Post3 xsi:type="xsd:string"></Ticket:Post3>
      <Ticket:EmailName xsi:type="xsd:string"></Ticket:EmailName>
      <Ticket:ContactFullName xsi:type="xsd:string"></Ticket:ContactFullName>
      <Ticket:ActiveErpLinks xsi:type="xsd:int">0</Ticket:ActiveErpLinks>
      <Ticket:TicketPriorityId xsi:type="xsd:int">0</Ticket:TicketPriorityId>
      <Ticket:SupportLanguageId xsi:type="xsd:int">0</Ticket:SupportLanguageId>
      <Ticket:SupportAssociateId xsi:type="xsd:int">0</Ticket:SupportAssociateId>
      <Ticket:CategoryName xsi:type="xsd:string"></Ticket:CategoryName>
     </Ticket:Person>
     <Ticket:SearchTitle xsi:type="xsd:string"></Ticket:SearchTitle>
     <Ticket:MessageHeaders xsi:type="Ticket:ArrayOfTicketMessageHeader">
      <Ticket:TicketMessageHeader xsi:type="Ticket:TicketMessageHeader">
       <Ticket:Id xsi:type="xsd:int">0</Ticket:Id>
       <Ticket:Name xsi:type="xsd:string"></Ticket:Name>
       <Ticket:Value xsi:type="xsd:string"></Ticket:Value>
       <Ticket:StdItem xsi:type="Ticket:MessageHeaderStdItem">None</Ticket:StdItem>
       <Ticket:StdItemCol xsi:type="Ticket:MessageHeaderStdItemCol">None</Ticket:StdItemCol>
      </Ticket:TicketMessageHeader>
     </Ticket:MessageHeaders>
     <Ticket:Important xsi:type="xsd:boolean">false</Ticket:Important>
     <Ticket:Language xsi:type="xsd:string"></Ticket:Language>
     <Ticket:Sentiment xsi:type="xsd:int">0</Ticket:Sentiment>
     <Ticket:SentimentConfidence xsi:type="xsd:int">0</Ticket:SentimentConfidence>
     <Ticket:ExtraFields xsi:type="Ticket:StringDictionary">
      <Ticket:StringKeyValuePair>
       <Ticket:Key xsi:type="xsd:string"></Ticket:Key>
       <Ticket:Value xsi:type="xsd:string"></Ticket:Value>
      </Ticket:StringKeyValuePair>
     </Ticket:ExtraFields>
     <Ticket:CustomFields xsi:type="Ticket:StringDictionary">
      <Ticket:StringKeyValuePair>
       <Ticket:Key xsi:type="xsd:string"></Ticket:Key>
       <Ticket:Value xsi:type="xsd:string"></Ticket:Value>
      </Ticket:StringKeyValuePair>
     </Ticket:CustomFields>
    </Ticket:NewTicketMessage>
    <Ticket:TransferAttachmentsIds xsi:type="NetServerServices882:ArrayOfint">
     <NetServerServices882:int xsi:type="xsd:int">0</NetServerServices882:int>
    </Ticket:TransferAttachmentsIds>
   </Ticket:SplitTicketMessage>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```


## SplitTicketMessage Response

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices882="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices881="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Ticket="http://www.superoffice.net/ws/crm/NetServer/Services88">
 <SOAP-ENV:Body>
  <Ticket:SplitTicketMessageResponse>
   <Ticket:Response xsi:type="Ticket:TicketEntity">
    <Ticket:TicketId xsi:type="xsd:int">0</Ticket:TicketId>
    <Ticket:Title xsi:type="xsd:string"></Ticket:Title>
    <Ticket:CreatedAt xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:CreatedAt>
    <Ticket:LastChanged xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:LastChanged>
    <Ticket:ReadByOwner xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:ReadByOwner>
    <Ticket:ReadByCustomer xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:ReadByCustomer>
    <Ticket:FirstReadByOwner xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:FirstReadByOwner>
    <Ticket:FirstReadByUser xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:FirstReadByUser>
    <Ticket:Activate xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:Activate>
    <Ticket:ClosedAt xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:ClosedAt>
    <Ticket:RepliedAt xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:RepliedAt>
    <Ticket:AlertTimeout xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:AlertTimeout>
    <Ticket:Deadline xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:Deadline>
    <Ticket:CreatedBy xsi:type="Ticket:Associate">
     <Ticket:AssociateId xsi:type="xsd:int">0</Ticket:AssociateId>
     <Ticket:Name xsi:type="xsd:string"></Ticket:Name>
     <Ticket:PersonId xsi:type="xsd:int">0</Ticket:PersonId>
     <Ticket:Rank xsi:type="xsd:short">0</Ticket:Rank>
     <Ticket:Tooltip xsi:type="xsd:string"></Ticket:Tooltip>
     <Ticket:Type xsi:type="Ticket:UserType">Unknown</Ticket:Type>
     <Ticket:GroupIdx xsi:type="xsd:int">0</Ticket:GroupIdx>
     <Ticket:FullName xsi:type="xsd:string"></Ticket:FullName>
     <Ticket:FormalName xsi:type="xsd:string"></Ticket:FormalName>
     <Ticket:Deleted xsi:type="xsd:boolean">false</Ticket:Deleted>
     <Ticket:EjUserId xsi:type="xsd:int">0</Ticket:EjUserId>
     <Ticket:UserName xsi:type="xsd:string"></Ticket:UserName>
    </Ticket:CreatedBy>
    <Ticket:Author xsi:type="xsd:string"></Ticket:Author>
    <Ticket:OwnedBy xsi:type="Ticket:Associate">
     <Ticket:AssociateId xsi:type="xsd:int">0</Ticket:AssociateId>
     <Ticket:Name xsi:type="xsd:string"></Ticket:Name>
     <Ticket:PersonId xsi:type="xsd:int">0</Ticket:PersonId>
     <Ticket:Rank xsi:type="xsd:short">0</Ticket:Rank>
     <Ticket:Tooltip xsi:type="xsd:string"></Ticket:Tooltip>
     <Ticket:Type xsi:type="Ticket:UserType">Unknown</Ticket:Type>
     <Ticket:GroupIdx xsi:type="xsd:int">0</Ticket:GroupIdx>
     <Ticket:FullName xsi:type="xsd:string"></Ticket:FullName>
     <Ticket:FormalName xsi:type="xsd:string"></Ticket:FormalName>
     <Ticket:Deleted xsi:type="xsd:boolean">false</Ticket:Deleted>
     <Ticket:EjUserId xsi:type="xsd:int">0</Ticket:EjUserId>
     <Ticket:UserName xsi:type="xsd:string"></Ticket:UserName>
    </Ticket:OwnedBy>
    <Ticket:Category xsi:type="Ticket:TicketCategoryEntity">
     <Ticket:TicketCategoryId xsi:type="xsd:int">0</Ticket:TicketCategoryId>
     <Ticket:ParentId xsi:type="xsd:int">0</Ticket:ParentId>
     <Ticket:Name xsi:type="xsd:string"></Ticket:Name>
     <Ticket:Fullname xsi:type="xsd:string"></Ticket:Fullname>
     <Ticket:CategoryMaster xsi:type="xsd:int">0</Ticket:CategoryMaster>
     <Ticket:Flags xsi:type="Ticket:TicketCategoryFlags">Internal</Ticket:Flags>
     <Ticket:DelegateMethod xsi:type="Ticket:TicketCategoryDelegateMethod">Unknown</Ticket:DelegateMethod>
     <Ticket:ExternalName xsi:type="xsd:string"></Ticket:ExternalName>
     <Ticket:ClosingStatus xsi:type="Ticket:TicketCategoryClosingStatus">UserDefined</Ticket:ClosingStatus>
     <Ticket:MsgClosingStatus xsi:type="Ticket:TicketCategoryClosingStatus">UserDefined</Ticket:MsgClosingStatus>
     <Ticket:AssignmentLag xsi:type="xsd:int">0</Ticket:AssignmentLag>
     <Ticket:ReplyTemplate xsi:type="xsd:int">0</Ticket:ReplyTemplate>
     <Ticket:NotificationEmail xsi:type="xsd:string"></Ticket:NotificationEmail>
     <Ticket:DefaultTicketStatus xsi:type="Ticket:TicketStatusEntity">
      <Ticket:TicketStatusId xsi:type="xsd:int">0</Ticket:TicketStatusId>
      <Ticket:Name xsi:type="xsd:string"></Ticket:Name>
      <Ticket:Status xsi:type="Ticket:TicketBaseStatus">Unknown</Ticket:Status>
      <Ticket:TimeCounter xsi:type="Ticket:TicketStatusTimeCounter">None</Ticket:TimeCounter>
      <Ticket:NoEmailReopen xsi:type="xsd:boolean">false</Ticket:NoEmailReopen>
      <Ticket:IsDefault xsi:type="xsd:boolean">false</Ticket:IsDefault>
      <Ticket:UsedInQueue xsi:type="xsd:boolean">false</Ticket:UsedInQueue>
     </Ticket:DefaultTicketStatus>
     <Ticket:DefaultMessageStatus xsi:type="Ticket:TicketStatusEntity">
      <Ticket:TicketStatusId xsi:type="xsd:int">0</Ticket:TicketStatusId>
      <Ticket:Name xsi:type="xsd:string"></Ticket:Name>
      <Ticket:Status xsi:type="Ticket:TicketBaseStatus">Unknown</Ticket:Status>
      <Ticket:TimeCounter xsi:type="Ticket:TicketStatusTimeCounter">None</Ticket:TimeCounter>
      <Ticket:NoEmailReopen xsi:type="xsd:boolean">false</Ticket:NoEmailReopen>
      <Ticket:IsDefault xsi:type="xsd:boolean">false</Ticket:IsDefault>
      <Ticket:UsedInQueue xsi:type="xsd:boolean">false</Ticket:UsedInQueue>
     </Ticket:DefaultMessageStatus>
     <Ticket:EffectiveReplyTemplateId xsi:type="xsd:int">0</Ticket:EffectiveReplyTemplateId>
     <Ticket:ExtraFields xsi:type="Ticket:StringDictionary">
      <Ticket:StringKeyValuePair>
       <Ticket:Key xsi:type="xsd:string"></Ticket:Key>
       <Ticket:Value xsi:type="xsd:string"></Ticket:Value>
      </Ticket:StringKeyValuePair>
     </Ticket:ExtraFields>
     <Ticket:CustomFields xsi:type="Ticket:StringDictionary">
      <Ticket:StringKeyValuePair>
       <Ticket:Key xsi:type="xsd:string"></Ticket:Key>
       <Ticket:Value xsi:type="xsd:string"></Ticket:Value>
      </Ticket:StringKeyValuePair>
     </Ticket:CustomFields>
    </Ticket:Category>
    <Ticket:Slevel xsi:type="Ticket:TicketSecurityLevel">Unknown</Ticket:Slevel>
    <Ticket:Priority xsi:type="Ticket:TicketPriorityEntity">
     <Ticket:TicketPriorityId xsi:type="xsd:int">0</Ticket:TicketPriorityId>
     <Ticket:Name xsi:type="xsd:string"></Ticket:Name>
     <Ticket:Status xsi:type="Ticket:TicketPriorityStatus">Unknown</Ticket:Status>
     <Ticket:Flags xsi:type="Ticket:TicketPriorityFlags">External</Ticket:Flags>
     <Ticket:SortOrder xsi:type="xsd:int">0</Ticket:SortOrder>
     <Ticket:TicketRead xsi:type="Ticket:TicketPriorityEscalateEvent">None</Ticket:TicketRead>
     <Ticket:ChangedOwner xsi:type="Ticket:TicketPriorityEscalateEvent">None</Ticket:ChangedOwner>
     <Ticket:TicketNewinfo xsi:type="Ticket:TicketPriorityEscalateEvent">None</Ticket:TicketNewinfo>
     <Ticket:TicketClosed xsi:type="Ticket:TicketPriorityEscalateEvent">None</Ticket:TicketClosed>
     <Ticket:TicketChangedPriority xsi:type="Ticket:TicketPriorityEscalateEvent">None</Ticket:TicketChangedPriority>
     <Ticket:TicketNew xsi:type="Ticket:TicketPriorityEscalateEvent">None</Ticket:TicketNew>
     <Ticket:Deadline xsi:type="xsd:int">0</Ticket:Deadline>
     <Ticket:MonStart xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:MonStart>
     <Ticket:MonStop xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:MonStop>
     <Ticket:TueStart xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:TueStart>
     <Ticket:TueStop xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:TueStop>
     <Ticket:WedStart xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:WedStart>
     <Ticket:WedStop xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:WedStop>
     <Ticket:ThuStart xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:ThuStart>
     <Ticket:ThuStop xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:ThuStop>
     <Ticket:FriStart xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:FriStart>
     <Ticket:FriStop xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:FriStop>
     <Ticket:SatStart xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:SatStart>
     <Ticket:SatStop xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:SatStop>
     <Ticket:SunStart xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:SunStart>
     <Ticket:SunStop xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:SunStop>
     <Ticket:NonDates xsi:type="NetServerServices882:ArrayOfdateTime">
      <NetServerServices882:dateTime xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</NetServerServices882:dateTime>
     </Ticket:NonDates>
     <Ticket:EscalationLevels xsi:type="Ticket:ArrayOfTicketPriorityEscalationLevelEntity">
      <Ticket:TicketPriorityEscalationLevelEntity xsi:type="Ticket:TicketPriorityEscalationLevelEntity">
       <Ticket:TicketAlertId xsi:type="xsd:int">0</Ticket:TicketAlertId>
       <Ticket:AlertLevel xsi:type="xsd:short">0</Ticket:AlertLevel>
       <Ticket:AlertTimeout xsi:type="xsd:int">0</Ticket:AlertTimeout>
       <Ticket:Action xsi:type="xsd:int">0</Ticket:Action>
       <Ticket:DelegateTo xsi:type="xsd:int">0</Ticket:DelegateTo>
       <Ticket:ScriptId xsi:type="xsd:int">0</Ticket:ScriptId>
       <Ticket:EmailTo xsi:type="xsd:string"></Ticket:EmailTo>
       <Ticket:SmsTo xsi:type="xsd:string"></Ticket:SmsTo>
       <Ticket:ReplyTemplateIdCustomer xsi:type="xsd:int">0</Ticket:ReplyTemplateIdCustomer>
       <Ticket:ReplyTemplateIdUser xsi:type="xsd:int">0</Ticket:ReplyTemplateIdUser>
       <Ticket:ReplyTemplateIdCatmast xsi:type="xsd:int">0</Ticket:ReplyTemplateIdCatmast>
       <Ticket:ReplyTemplateIdEmail xsi:type="xsd:int">0</Ticket:ReplyTemplateIdEmail>
       <Ticket:RtiCustomerSms xsi:type="xsd:int">0</Ticket:RtiCustomerSms>
       <Ticket:ReplyTemplateIdUserSms xsi:type="xsd:int">0</Ticket:ReplyTemplateIdUserSms>
       <Ticket:ReplyTemplateIdCatmastSms xsi:type="xsd:int">0</Ticket:ReplyTemplateIdCatmastSms>
       <Ticket:ReplyTemplateIdSms xsi:type="xsd:int">0</Ticket:ReplyTemplateIdSms>
      </Ticket:TicketPriorityEscalationLevelEntity>
     </Ticket:EscalationLevels>
    </Ticket:Priority>
    <Ticket:BaseStatus xsi:type="Ticket:TicketBaseStatus">Unknown</Ticket:BaseStatus>
    <Ticket:Status xsi:type="Ticket:TicketStatusEntity">
     <Ticket:TicketStatusId xsi:type="xsd:int">0</Ticket:TicketStatusId>
     <Ticket:Name xsi:type="xsd:string"></Ticket:Name>
     <Ticket:Status xsi:type="Ticket:TicketBaseStatus">Unknown</Ticket:Status>
     <Ticket:TimeCounter xsi:type="Ticket:TicketStatusTimeCounter">None</Ticket:TimeCounter>
     <Ticket:NoEmailReopen xsi:type="xsd:boolean">false</Ticket:NoEmailReopen>
     <Ticket:IsDefault xsi:type="xsd:boolean">false</Ticket:IsDefault>
     <Ticket:UsedInQueue xsi:type="xsd:boolean">false</Ticket:UsedInQueue>
    </Ticket:Status>
    <Ticket:Origin xsi:type="Ticket:TicketOrigin">Unknown</Ticket:Origin>
    <Ticket:Person xsi:type="Ticket:Person">
     <Ticket:Position xsi:type="xsd:string"></Ticket:Position>
     <Ticket:PersonId xsi:type="xsd:int">0</Ticket:PersonId>
     <Ticket:Mrmrs xsi:type="xsd:string"></Ticket:Mrmrs>
     <Ticket:Firstname xsi:type="xsd:string"></Ticket:Firstname>
     <Ticket:Lastname xsi:type="xsd:string"></Ticket:Lastname>
     <Ticket:MiddleName xsi:type="xsd:string"></Ticket:MiddleName>
     <Ticket:Title xsi:type="xsd:string"></Ticket:Title>
     <Ticket:Description xsi:type="xsd:string"></Ticket:Description>
     <Ticket:Email xsi:type="xsd:string"></Ticket:Email>
     <Ticket:FullName xsi:type="xsd:string"></Ticket:FullName>
     <Ticket:DirectPhone xsi:type="xsd:string"></Ticket:DirectPhone>
     <Ticket:FormalName xsi:type="xsd:string"></Ticket:FormalName>
     <Ticket:CountryId xsi:type="xsd:int">0</Ticket:CountryId>
     <Ticket:ContactId xsi:type="xsd:int">0</Ticket:ContactId>
     <Ticket:ContactName xsi:type="xsd:string"></Ticket:ContactName>
     <Ticket:Retired xsi:type="xsd:short">0</Ticket:Retired>
     <Ticket:Rank xsi:type="xsd:short">0</Ticket:Rank>
     <Ticket:ActiveInterests xsi:type="xsd:short">0</Ticket:ActiveInterests>
     <Ticket:ContactDepartment xsi:type="xsd:string"></Ticket:ContactDepartment>
     <Ticket:ContactCountryId xsi:type="xsd:int">0</Ticket:ContactCountryId>
     <Ticket:ContactOrgNr xsi:type="xsd:string"></Ticket:ContactOrgNr>
     <Ticket:FaxPhone xsi:type="xsd:string"></Ticket:FaxPhone>
     <Ticket:MobilePhone xsi:type="xsd:string"></Ticket:MobilePhone>
     <Ticket:ContactPhone xsi:type="xsd:string"></Ticket:ContactPhone>
     <Ticket:AssociateName xsi:type="xsd:string"></Ticket:AssociateName>
     <Ticket:AssociateId xsi:type="xsd:int">0</Ticket:AssociateId>
     <Ticket:UsePersonAddress xsi:type="xsd:boolean">false</Ticket:UsePersonAddress>
     <Ticket:ContactFax xsi:type="xsd:string"></Ticket:ContactFax>
     <Ticket:Kanafname xsi:type="xsd:string"></Ticket:Kanafname>
     <Ticket:Kanalname xsi:type="xsd:string"></Ticket:Kanalname>
     <Ticket:Post1 xsi:type="xsd:string"></Ticket:Post1>
     <Ticket:Post2 xsi:type="xsd:string"></Ticket:Post2>
     <Ticket:Post3 xsi:type="xsd:string"></Ticket:Post3>
     <Ticket:EmailName xsi:type="xsd:string"></Ticket:EmailName>
     <Ticket:ContactFullName xsi:type="xsd:string"></Ticket:ContactFullName>
     <Ticket:ActiveErpLinks xsi:type="xsd:int">0</Ticket:ActiveErpLinks>
     <Ticket:TicketPriorityId xsi:type="xsd:int">0</Ticket:TicketPriorityId>
     <Ticket:SupportLanguageId xsi:type="xsd:int">0</Ticket:SupportLanguageId>
     <Ticket:SupportAssociateId xsi:type="xsd:int">0</Ticket:SupportAssociateId>
     <Ticket:CategoryName xsi:type="xsd:string"></Ticket:CategoryName>
    </Ticket:Person>
    <Ticket:SecondaryPersons xsi:type="Ticket:ArrayOfPerson">
     <Ticket:Person xsi:type="Ticket:Person">
      <Ticket:Position xsi:type="xsd:string"></Ticket:Position>
      <Ticket:PersonId xsi:type="xsd:int">0</Ticket:PersonId>
      <Ticket:Mrmrs xsi:type="xsd:string"></Ticket:Mrmrs>
      <Ticket:Firstname xsi:type="xsd:string"></Ticket:Firstname>
      <Ticket:Lastname xsi:type="xsd:string"></Ticket:Lastname>
      <Ticket:MiddleName xsi:type="xsd:string"></Ticket:MiddleName>
      <Ticket:Title xsi:type="xsd:string"></Ticket:Title>
      <Ticket:Description xsi:type="xsd:string"></Ticket:Description>
      <Ticket:Email xsi:type="xsd:string"></Ticket:Email>
      <Ticket:FullName xsi:type="xsd:string"></Ticket:FullName>
      <Ticket:DirectPhone xsi:type="xsd:string"></Ticket:DirectPhone>
      <Ticket:FormalName xsi:type="xsd:string"></Ticket:FormalName>
      <Ticket:CountryId xsi:type="xsd:int">0</Ticket:CountryId>
      <Ticket:ContactId xsi:type="xsd:int">0</Ticket:ContactId>
      <Ticket:ContactName xsi:type="xsd:string"></Ticket:ContactName>
      <Ticket:Retired xsi:type="xsd:short">0</Ticket:Retired>
      <Ticket:Rank xsi:type="xsd:short">0</Ticket:Rank>
      <Ticket:ActiveInterests xsi:type="xsd:short">0</Ticket:ActiveInterests>
      <Ticket:ContactDepartment xsi:type="xsd:string"></Ticket:ContactDepartment>
      <Ticket:ContactCountryId xsi:type="xsd:int">0</Ticket:ContactCountryId>
      <Ticket:ContactOrgNr xsi:type="xsd:string"></Ticket:ContactOrgNr>
      <Ticket:FaxPhone xsi:type="xsd:string"></Ticket:FaxPhone>
      <Ticket:MobilePhone xsi:type="xsd:string"></Ticket:MobilePhone>
      <Ticket:ContactPhone xsi:type="xsd:string"></Ticket:ContactPhone>
      <Ticket:AssociateName xsi:type="xsd:string"></Ticket:AssociateName>
      <Ticket:AssociateId xsi:type="xsd:int">0</Ticket:AssociateId>
      <Ticket:UsePersonAddress xsi:type="xsd:boolean">false</Ticket:UsePersonAddress>
      <Ticket:ContactFax xsi:type="xsd:string"></Ticket:ContactFax>
      <Ticket:Kanafname xsi:type="xsd:string"></Ticket:Kanafname>
      <Ticket:Kanalname xsi:type="xsd:string"></Ticket:Kanalname>
      <Ticket:Post1 xsi:type="xsd:string"></Ticket:Post1>
      <Ticket:Post2 xsi:type="xsd:string"></Ticket:Post2>
      <Ticket:Post3 xsi:type="xsd:string"></Ticket:Post3>
      <Ticket:EmailName xsi:type="xsd:string"></Ticket:EmailName>
      <Ticket:ContactFullName xsi:type="xsd:string"></Ticket:ContactFullName>
      <Ticket:ActiveErpLinks xsi:type="xsd:int">0</Ticket:ActiveErpLinks>
      <Ticket:TicketPriorityId xsi:type="xsd:int">0</Ticket:TicketPriorityId>
      <Ticket:SupportLanguageId xsi:type="xsd:int">0</Ticket:SupportLanguageId>
      <Ticket:SupportAssociateId xsi:type="xsd:int">0</Ticket:SupportAssociateId>
      <Ticket:CategoryName xsi:type="xsd:string"></Ticket:CategoryName>
     </Ticket:Person>
    </Ticket:SecondaryPersons>
    <Ticket:AlertLevel xsi:type="xsd:short">0</Ticket:AlertLevel>
    <Ticket:ConnectId xsi:type="xsd:int">0</Ticket:ConnectId>
    <Ticket:ReadStatus xsi:type="Ticket:TicketReadStatus">Unknown</Ticket:ReadStatus>
    <Ticket:TimeToReply xsi:type="xsd:int">0</Ticket:TimeToReply>
    <Ticket:RealTimeToReply xsi:type="xsd:int">0</Ticket:RealTimeToReply>
    <Ticket:TimeToClose xsi:type="xsd:int">0</Ticket:TimeToClose>
    <Ticket:RealTimeToClose xsi:type="xsd:int">0</Ticket:RealTimeToClose>
    <Ticket:TimeSpentInternally xsi:type="xsd:int">0</Ticket:TimeSpentInternally>
    <Ticket:TimeSpentExternally xsi:type="xsd:int">0</Ticket:TimeSpentExternally>
    <Ticket:TimeSpentQueue xsi:type="xsd:int">0</Ticket:TimeSpentQueue>
    <Ticket:RealTimeSpentInternally xsi:type="xsd:int">0</Ticket:RealTimeSpentInternally>
    <Ticket:RealTimeSpentExternally xsi:type="xsd:int">0</Ticket:RealTimeSpentExternally>
    <Ticket:RealTimeSpentQueue xsi:type="xsd:int">0</Ticket:RealTimeSpentQueue>
    <Ticket:HasAttachment xsi:type="xsd:boolean">false</Ticket:HasAttachment>
    <Ticket:NumReplies xsi:type="xsd:int">0</Ticket:NumReplies>
    <Ticket:NumMessages xsi:type="xsd:int">0</Ticket:NumMessages>
    <Ticket:FromAddress xsi:type="xsd:string"></Ticket:FromAddress>
    <Ticket:Messages xsi:type="Ticket:ArrayOfTicketMessage">
     <Ticket:TicketMessage xsi:type="Ticket:TicketMessage">
      <Ticket:TicketMessageId xsi:type="xsd:int">0</Ticket:TicketMessageId>
      <Ticket:CreatedAt xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:CreatedAt>
      <Ticket:Slevel xsi:type="Ticket:TicketSecurityLevel">Unknown</Ticket:Slevel>
      <Ticket:Important xsi:type="xsd:boolean">false</Ticket:Important>
      <Ticket:Author xsi:type="xsd:string"></Ticket:Author>
      <Ticket:PersonId xsi:type="xsd:int">0</Ticket:PersonId>
      <Ticket:PersonFullName xsi:type="xsd:string"></Ticket:PersonFullName>
      <Ticket:ContactId xsi:type="xsd:int">0</Ticket:ContactId>
      <Ticket:ContactName xsi:type="xsd:string"></Ticket:ContactName>
      <Ticket:ContactDepartment xsi:type="xsd:string"></Ticket:ContactDepartment>
      <Ticket:NumAttachments xsi:type="xsd:int">0</Ticket:NumAttachments>
      <Ticket:EmailHeader xsi:type="xsd:string"></Ticket:EmailHeader>
      <Ticket:MessageHeaders xsi:type="Ticket:ArrayOfTicketMessageHeader">
       <Ticket:TicketMessageHeader xsi:type="Ticket:TicketMessageHeader">
        <Ticket:Id xsi:type="xsd:int">0</Ticket:Id>
        <Ticket:Name xsi:type="xsd:string"></Ticket:Name>
        <Ticket:Value xsi:type="xsd:string"></Ticket:Value>
        <Ticket:StdItem xsi:type="Ticket:MessageHeaderStdItem">None</Ticket:StdItem>
        <Ticket:StdItemCol xsi:type="Ticket:MessageHeaderStdItemCol">None</Ticket:StdItemCol>
       </Ticket:TicketMessageHeader>
      </Ticket:MessageHeaders>
      <Ticket:Language xsi:type="xsd:string"></Ticket:Language>
      <Ticket:Sentiment xsi:type="xsd:int">0</Ticket:Sentiment>
      <Ticket:SentimentConfidence xsi:type="xsd:int">0</Ticket:SentimentConfidence>
      <Ticket:CreatedBy xsi:type="xsd:int">0</Ticket:CreatedBy>
      <Ticket:ChangedAt xsi:type="xsd:dateTime">2022-11-29T01:49:14Z</Ticket:ChangedAt>
     </Ticket:TicketMessage>
    </Ticket:Messages>
    <Ticket:Tags xsi:type="Ticket:ArrayOfTag">
     <Ticket:Tag xsi:type="Ticket:Tag">
      <Ticket:Id xsi:type="xsd:int">0</Ticket:Id>
      <Ticket:Name xsi:type="xsd:string"></Ticket:Name>
      <Ticket:ToolTip xsi:type="xsd:string"></Ticket:ToolTip>
     </Ticket:Tag>
    </Ticket:Tags>
    <Ticket:Language xsi:type="xsd:string"></Ticket:Language>
    <Ticket:Sentiment xsi:type="xsd:int">0</Ticket:Sentiment>
    <Ticket:SentimentConfidence xsi:type="xsd:int">0</Ticket:SentimentConfidence>
    <Ticket:SuggestedCategoryId xsi:type="xsd:int">0</Ticket:SuggestedCategoryId>
    <Ticket:SuggestedCategoryName xsi:type="xsd:string"></Ticket:SuggestedCategoryName>
    <Ticket:OrigHumanCategoryId xsi:type="xsd:int">0</Ticket:OrigHumanCategoryId>
    <Ticket:IconHint xsi:type="xsd:string"></Ticket:IconHint>
    <Ticket:ExtraFields xsi:type="Ticket:StringDictionary">
     <Ticket:StringKeyValuePair>
      <Ticket:Key xsi:type="xsd:string"></Ticket:Key>
      <Ticket:Value xsi:type="xsd:string"></Ticket:Value>
     </Ticket:StringKeyValuePair>
    </Ticket:ExtraFields>
    <Ticket:CustomFields xsi:type="Ticket:StringDictionary">
     <Ticket:StringKeyValuePair>
      <Ticket:Key xsi:type="xsd:string"></Ticket:Key>
      <Ticket:Value xsi:type="xsd:string"></Ticket:Value>
     </Ticket:StringKeyValuePair>
    </Ticket:CustomFields>
   </Ticket:Response>
  </Ticket:SplitTicketMessageResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

