---
title: Services87.AppointmentAgent.Accept SOAP
generated: 1
uid: Services87-Appointment-Accept
---

# Services87 Appointment Accept

SOAP request and response examples **Remote/Services87/Appointment.svc**
Implemented by the <see cref="M:SuperOffice.Services87.IAppointmentAgent.Accept">SuperOffice.Services87.IAppointmentAgent.Accept</see> method.

## Accept

Accepting an appointment invitation.

* **appointmentId:** The appointmentId. Both master and child record ids are accepted.
* **updateMode:** Update mode for a recurring appointment.

**Returns:** Updated AppointmentEntity

[WSDL file for Services87/Appointment](../Services87-Appointment.md)

Obtain a ticket from the [Services87/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## Accept Request

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices872="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices871="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Appointment="http://www.superoffice.net/ws/crm/NetServer/Services87">
  <Appointment:ApplicationToken>1234567-1234-9876</Appointment:ApplicationToken>
  <Appointment:Credentials>
    <Appointment:Ticket>7T:1234abcxyzExample==</Appointment:Ticket>
  </Appointment:Credentials>
 <SOAP-ENV:Body>
   <Appointment:Accept>
    <Appointment:AppointmentId xsi:type="xsd:int">0</Appointment:AppointmentId>
    <Appointment:UpdateMode xsi:type="Appointment:RecurrenceUpdateMode">Unknown</Appointment:UpdateMode>
   </Appointment:Accept>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

## Accept Response

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices872="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices871="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Appointment="http://www.superoffice.net/ws/crm/NetServer/Services87">
 <SOAP-ENV:Body>
  <Appointment:AcceptResponse>
  </Appointment:AcceptResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```
