---
title: Services88.AppointmentAgent.GetTaskListItem SOAP
generated: 1
uid: Services88-Appointment-GetTaskListItem
---

# Services88 Appointment GetTaskListItem

SOAP request and response examples **Remote/Services88/Appointment.svc**
Implemented by the <see cref="M:SuperOffice.Services88.IAppointmentAgent.GetTaskListItem">SuperOffice.Services88.IAppointmentAgent.GetTaskListItem</see> method.

## GetTaskListItem

Gets a TaskListItem object.

* **taskListItemId:** The identifier of the TaskListItem object

**Returns:** TaskListItem

[WSDL file for Services88/Appointment](../Services88-Appointment.md)

Obtain a ticket from the [Services88/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## GetTaskListItem Request

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices882="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices881="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Appointment="http://www.superoffice.net/ws/crm/NetServer/Services88">
  <Appointment:ApplicationToken>1234567-1234-9876</Appointment:ApplicationToken>
  <Appointment:Credentials>
    <Appointment:Ticket>7T:1234abcxyzExample==</Appointment:Ticket>
  </Appointment:Credentials>
 <SOAP-ENV:Body>
   <Appointment:GetTaskListItem>
    <Appointment:TaskListItemId xsi:type="xsd:int">0</Appointment:TaskListItemId>
   </Appointment:GetTaskListItem>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

## GetTaskListItem Response

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices882="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices881="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Appointment="http://www.superoffice.net/ws/crm/NetServer/Services88">
 <SOAP-ENV:Body>
  <Appointment:GetTaskListItemResponse>
   <Appointment:Response xsi:type="Appointment:TaskListItem">
    <Appointment:TaskListItemId xsi:type="xsd:int">0</Appointment:TaskListItemId>
    <Appointment:Value xsi:type="xsd:string"></Appointment:Value>
    <Appointment:Direction xsi:type="Appointment:TaskDirection">Unknown</Appointment:Direction>
    <Appointment:Type xsi:type="Appointment:TaskType">Unknown</Appointment:Type>
    <Appointment:Tooltip xsi:type="xsd:string"></Appointment:Tooltip>
    <Appointment:Deleted xsi:type="xsd:boolean">false</Appointment:Deleted>
    <Appointment:IntentId xsi:type="xsd:int">0</Appointment:IntentId>
    <Appointment:Rank xsi:type="xsd:short">0</Appointment:Rank>
    <Appointment:IsDefaultAlldayEvent xsi:type="xsd:boolean">false</Appointment:IsDefaultAlldayEvent>
    <Appointment:IsDefaultFree xsi:type="xsd:boolean">false</Appointment:IsDefaultFree>
    <Appointment:IsDefaultPublished xsi:type="xsd:boolean">false</Appointment:IsDefaultPublished>
    <Appointment:ColorIndex xsi:type="Appointment:ColorIndex">LightBlue</Appointment:ColorIndex>
    <Appointment:DefaultVideomeetingStatus xsi:type="Appointment:VideoMeetingStatus">NoChange</Appointment:DefaultVideomeetingStatus>
   </Appointment:Response>
  </Appointment:GetTaskListItemResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```
