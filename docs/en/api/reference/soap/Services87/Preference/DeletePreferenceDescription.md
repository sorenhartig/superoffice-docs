---
title: Services87.PreferenceAgent.DeletePreferenceDescription SOAP
generated: 1
uid: Services87-Preference-DeletePreferenceDescription
---

# Services87 Preference DeletePreferenceDescription

SOAP request and response examples **Remote/Services87/Preference.svc**
Implemented by the <see cref="M:SuperOffice.Services87.IPreferenceAgent.DeletePreferenceDescription">SuperOffice.Services87.IPreferenceAgent.DeletePreferenceDescription</see> method.

## DeletePreferenceDescription

Deletes the PreferenceDescription

* **preferenceDescriptionId:** The identity of the PreferenceDescription

[WSDL file for Services87/Preference](../Services87-Preference.md)

Obtain a ticket from the [Services87/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## DeletePreferenceDescription Request

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices872="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices871="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Preference="http://www.superoffice.net/ws/crm/NetServer/Services87">
  <Preference:ApplicationToken>1234567-1234-9876</Preference:ApplicationToken>
  <Preference:Credentials>
    <Preference:Ticket>7T:1234abcxyzExample==</Preference:Ticket>
  </Preference:Credentials>
 <SOAP-ENV:Body>
   <Preference:DeletePreferenceDescription>
    <Preference:PreferenceDescriptionId xsi:type="xsd:int">0</Preference:PreferenceDescriptionId>
   </Preference:DeletePreferenceDescription>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

## DeletePreferenceDescription Response

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices872="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices871="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Preference="http://www.superoffice.net/ws/crm/NetServer/Services87">
 <SOAP-ENV:Body>
  <Preference:DeletePreferenceDescriptionResponse>
  </Preference:DeletePreferenceDescriptionResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```
