---
title: Services88.SelectionAgent.SetDuplicateRulesStatus SOAP
generated: 1
uid: Services88-Selection-SetDuplicateRulesStatus
---

# Services88 Selection SetDuplicateRulesStatus

SOAP request and response examples **Remote/Services88/Selection.svc**
Implemented by the <see cref="M:SuperOffice.Services88.ISelectionAgent.SetDuplicateRulesStatus">SuperOffice.Services88.ISelectionAgent.SetDuplicateRulesStatus</see> method.

## SetDuplicateRulesStatus

Set which duplicate rules should be active or not

* **rules:** Duplicate rules to update active status for

[WSDL file for Services88/Selection](../Services88-Selection.md)

Obtain a ticket from the [Services88/SoPrincipal.svc](../SoPrincipal/index.md)

Application tokens must be specified if calling an Online installation. ApplicationTokens are not checked for on-site installations.

## SetDuplicateRulesStatus Request

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices882="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices881="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Selection="http://www.superoffice.net/ws/crm/NetServer/Services88">
  <Selection:ApplicationToken>1234567-1234-9876</Selection:ApplicationToken>
  <Selection:Credentials>
    <Selection:Ticket>7T:1234abcxyzExample==</Selection:Ticket>
  </Selection:Credentials>
 <SOAP-ENV:Body>
   <Selection:SetDuplicateRulesStatus>
    <Selection:Rules xsi:type="Selection:ArrayOfDuplicateRule">
     <Selection:DuplicateRule xsi:type="Selection:DuplicateRule">
      <Selection:Name xsi:type="xsd:string"></Selection:Name>
      <Selection:DisplayName xsi:type="xsd:string"></Selection:DisplayName>
      <Selection:DisplayTooltip xsi:type="xsd:string"></Selection:DisplayTooltip>
      <Selection:IsActive xsi:type="xsd:boolean">false</Selection:IsActive>
     </Selection:DuplicateRule>
    </Selection:Rules>
   </Selection:SetDuplicateRulesStatus>

 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```

## SetDuplicateRulesStatus Response

```xml
<?xml version="1.0" encoding="UTF-8"?>
<SOAP-ENV:Envelope
 xmlns:SOAP-ENV="http://www.w3.org/2003/05/soap-envelope"
 xmlns:SOAP-ENC="http://www.w3.org/2003/05/soap-encoding"
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:NetServerServices882="http://schemas.microsoft.com/2003/10/Serialization/Arrays"
 xmlns:NetServerServices881="http://schemas.microsoft.com/2003/10/Serialization/"
 xmlns:Selection="http://www.superoffice.net/ws/crm/NetServer/Services88">
 <SOAP-ENV:Body>
  <Selection:SetDuplicateRulesStatusResponse>
  </Selection:SetDuplicateRulesStatusResponse>
 </SOAP-ENV:Body>
</SOAP-ENV:Envelope>

```
