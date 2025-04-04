---
title: Services87.AppointmentAgent.ToggleAppointmentStatus SOAP
generated: 1
uid: Services87-Appointment-ToggleAppointmentStatus
---

# Services87 Appointment ToggleAppointmentStatus

SOAP request and response examples **Remote/Services87/Appointment.svc**
Implemented by the <see cref="M:SuperOffice.Services87.IAppointmentAgent.ToggleAppointmentStatus">SuperOffice.Services87.IAppointmentAgent.ToggleAppointmentStatus</see> method.

## ToggleAppointmentStatus

Sets an appointment's status to Completed if the appointment had a different status, or sets the status to started if already set to completed.

* **appointmentId:** The appointment id.

**Returns:** The new AppointmentStatus

[WSDL file for Services87/Appointment](../Services87-Appointment.md)

Obtain a ticket from the [Services87/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## ToggleAppointmentStatus Request

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
   <Appointment:ToggleAppointmentStatus>
    <Appointment:AppointmentId xsi:type="xsd:int">0</Appointment:AppointmentId>
   </Appointment:ToggleAppointmentStatus>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

## ToggleAppointmentStatus Response

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
  <Appointment:ToggleAppointmentStatusResponse>
   <Appointment:Response xsi:type="Appointment:AppointmentStatus">UnknownOrPostIt</Appointment:Response>
  </Appointment:ToggleAppointmentStatusResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```
