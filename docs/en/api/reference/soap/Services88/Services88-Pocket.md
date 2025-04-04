---
generated: 1
uid: wsdl-Services88-Pocket
title: Services88.PocketAgent WSDL
---

# Services88.PocketAgent WSDL

```xml
<?xml version="1.0" encoding="utf-8"?>
<wsdl:definitions name="WcfPocketService" targetNamespace="http://www.superoffice.net/ws/crm/NetServer/Services88" xmlns:wsdl="http://schemas.xmlsoap.org/wsdl/" xmlns:wsam="http://www.w3.org/2007/05/addressing/metadata" xmlns:wsx="http://schemas.xmlsoap.org/ws/2004/09/mex" xmlns:wsap="http://schemas.xmlsoap.org/ws/2004/08/addressing/policy" xmlns:msc="http://schemas.microsoft.com/ws/2005/12/wsdl/contract" xmlns:wsp="http://schemas.xmlsoap.org/ws/2004/09/policy" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/wsdl/soap/" xmlns:wsu="http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-wssecurity-utility-1.0.xsd" xmlns:soap12="http://schemas.xmlsoap.org/wsdl/soap12/" xmlns:soapenc="http://schemas.xmlsoap.org/soap/encoding/" xmlns:tns="http://www.superoffice.net/ws/crm/NetServer/Services88" xmlns:wsa10="http://www.w3.org/2005/08/addressing" xmlns:wsaw="http://www.w3.org/2006/05/addressing/wsdl" xmlns:wsa="http://schemas.xmlsoap.org/ws/2004/08/addressing">
  <wsdl:types>
    <xs:schema elementFormDefault="qualified" targetNamespace="http://www.superoffice.net/ws/crm/NetServer/Services88" xmlns:xs="http://www.w3.org/2001/XMLSchema" xmlns:ser="http://schemas.microsoft.com/2003/10/Serialization/">
      <xs:import namespace="http://schemas.microsoft.com/2003/10/Serialization/Arrays" />
      <xs:import namespace="http://schemas.microsoft.com/2003/10/Serialization/" />
      <xs:element name="GetMyCallerIDs">
        <xs:complexType>
          <xs:sequence>
            <xs:element minOccurs="0" name="LastHash" nillable="true" type="xs:string" />
            <xs:element minOccurs="0" name="MinDate" type="xs:dateTime" />
            <xs:element minOccurs="0" name="MaxDate" type="xs:dateTime" />
          </xs:sequence>
        </xs:complexType>
      </xs:element>
      <xs:element name="ApplicationToken" nillable="true" type="xs:string" />
      <xs:complexType name="SoCredentials">
        <xs:sequence>
          <xs:element minOccurs="0" name="Ticket" nillable="true" type="xs:string" />
        </xs:sequence>
      </xs:complexType>
      <xs:element name="SoCredentials" nillable="true" type="q1:SoCredentials" xmlns:q1="http://www.superoffice.net/ws/crm/NetServer/Services88" />
      <xs:element name="Credentials" nillable="true" type="q2:SoCredentials" xmlns:q2="http://www.superoffice.net/ws/crm/NetServer/Services88" />
      <xs:complexType name="SoTimeZone">
        <xs:sequence>
          <xs:element minOccurs="0" name="SoTimeZoneId" type="xs:int" />
          <xs:element minOccurs="0" name="SoTimeZoneLocationCode" nillable="true" type="xs:string" />
        </xs:sequence>
      </xs:complexType>
      <xs:element name="SoTimeZone" nillable="true" type="q3:SoTimeZone" xmlns:q3="http://www.superoffice.net/ws/crm/NetServer/Services88" />
      <xs:element name="TimeZone" nillable="true" type="q4:SoTimeZone" xmlns:q4="http://www.superoffice.net/ws/crm/NetServer/Services88" />
      <xs:element name="GetMyCallerIDsResponse">
        <xs:complexType>
          <xs:sequence>
            <xs:element minOccurs="0" name="Response" nillable="true" type="q5:CallerIDCollection" xmlns:q5="http://www.superoffice.net/ws/crm/NetServer/Services88" />
          </xs:sequence>
        </xs:complexType>
      </xs:element>
      <xs:complexType name="CallerIDCollection">
        <xs:sequence>
          <xs:element minOccurs="0" name="CallerIDHash" nillable="true" type="xs:string" />
          <xs:element minOccurs="0" name="CallerIDs" nillable="true" type="q6:ArrayOfCallerID" xmlns:q6="http://www.superoffice.net/ws/crm/NetServer/Services88" />
        </xs:sequence>
      </xs:complexType>
      <xs:element name="CallerIDCollection" nillable="true" type="q7:CallerIDCollection" xmlns:q7="http://www.superoffice.net/ws/crm/NetServer/Services88" />
      <xs:complexType name="ArrayOfCallerID">
        <xs:sequence>
          <xs:element minOccurs="0" maxOccurs="unbounded" name="CallerID" nillable="true" type="q8:CallerID" xmlns:q8="http://www.superoffice.net/ws/crm/NetServer/Services88" />
        </xs:sequence>
      </xs:complexType>
      <xs:element name="ArrayOfCallerID" nillable="true" type="q9:ArrayOfCallerID" xmlns:q9="http://www.superoffice.net/ws/crm/NetServer/Services88" />
      <xs:complexType name="CallerID">
        <xs:sequence>
          <xs:element minOccurs="0" name="PhoneNumber" type="xs:long" />
          <xs:element minOccurs="0" name="DialInPrefix" type="xs:short" />
          <xs:element minOccurs="0" name="PersonId" type="xs:int" />
          <xs:element minOccurs="0" name="PersonName" nillable="true" type="xs:string" />
          <xs:element minOccurs="0" name="Mrmrs" nillable="true" type="xs:string" />
          <xs:element minOccurs="0" name="ContactId" type="xs:int" />
          <xs:element minOccurs="0" name="ContactName" nillable="true" type="xs:string" />
        </xs:sequence>
      </xs:complexType>
      <xs:element name="CallerID" nillable="true" type="q10:CallerID" xmlns:q10="http://www.superoffice.net/ws/crm/NetServer/Services88" />
      <xs:complexType name="SoExceptionInfo">
        <xs:sequence>
          <xs:element minOccurs="0" name="Message" nillable="true" type="xs:string" />
          <xs:element minOccurs="0" name="StackTrace" nillable="true" type="xs:string" />
          <xs:element minOccurs="0" name="FriendlyText" nillable="true" type="xs:string" />
          <xs:element minOccurs="0" name="ExceptionType" nillable="true" type="xs:string" />
          <xs:element minOccurs="0" name="Source" nillable="true" type="xs:string" />
          <xs:element minOccurs="0" name="InnerException" nillable="true" type="q11:SoExceptionInfo" xmlns:q11="http://www.superoffice.net/ws/crm/NetServer/Services88" />
          <xs:element minOccurs="0" name="Parameters" nillable="true" type="q12:SoExceptionInfoParameters" xmlns:q12="http://www.superoffice.net/ws/crm/NetServer/Services88" />
        </xs:sequence>
      </xs:complexType>
      <xs:element name="SoExceptionInfo" nillable="true" type="q13:SoExceptionInfo" xmlns:q13="http://www.superoffice.net/ws/crm/NetServer/Services88" />
      <xs:complexType name="SoExceptionInfoParameters">
        <xs:annotation>
          <xs:appinfo>
            <IsDictionary xmlns="http://schemas.microsoft.com/2003/10/Serialization/">true</IsDictionary>
          </xs:appinfo>
        </xs:annotation>
        <xs:sequence>
          <xs:element minOccurs="0" maxOccurs="unbounded" name="SoExceptionInfoParametersKeyValuePair">
            <xs:complexType>
              <xs:sequence>
                <xs:element name="Key" nillable="true" type="xs:string" />
                <xs:element name="Value" nillable="true" type="xs:string" />
              </xs:sequence>
            </xs:complexType>
          </xs:element>
        </xs:sequence>
      </xs:complexType>
      <xs:element name="SoExceptionInfoParameters" nillable="true" type="q14:SoExceptionInfoParameters" xmlns:q14="http://www.superoffice.net/ws/crm/NetServer/Services88" />
      <xs:element name="ExceptionInfo" nillable="true" type="q15:SoExceptionInfo" xmlns:q15="http://www.superoffice.net/ws/crm/NetServer/Services88" />
      <xs:complexType name="SoExtraInfo">
        <xs:annotation>
          <xs:appinfo>
            <IsDictionary xmlns="http://schemas.microsoft.com/2003/10/Serialization/">true</IsDictionary>
          </xs:appinfo>
        </xs:annotation>
        <xs:sequence>
          <xs:element minOccurs="0" maxOccurs="unbounded" name="ExtraInfoNameValuePair">
            <xs:complexType>
              <xs:sequence>
                <xs:element name="Key" nillable="true" type="xs:string" />
                <xs:element name="Value" nillable="true" type="xs:string" />
              </xs:sequence>
            </xs:complexType>
          </xs:element>
        </xs:sequence>
      </xs:complexType>
      <xs:element name="SoExtraInfo" nillable="true" type="q16:SoExtraInfo" xmlns:q16="http://www.superoffice.net/ws/crm/NetServer/Services88" />
      <xs:element name="ExtraInfo" nillable="true" type="q17:SoExtraInfo" xmlns:q17="http://www.superoffice.net/ws/crm/NetServer/Services88" />
      <xs:element name="Succeeded" type="xs:boolean" />
      <xs:element name="GetCallerIDsFromSelection">
        <xs:complexType>
          <xs:sequence>
            <xs:element minOccurs="0" name="SelectionId" type="xs:int" />
            <xs:element minOccurs="0" name="LastHash" nillable="true" type="xs:string" />
          </xs:sequence>
        </xs:complexType>
      </xs:element>
      <xs:element name="GetCallerIDsFromSelectionResponse">
        <xs:complexType>
          <xs:sequence>
            <xs:element minOccurs="0" name="Response" nillable="true" type="q18:CallerIDCollection" xmlns:q18="http://www.superoffice.net/ws/crm/NetServer/Services88" />
          </xs:sequence>
        </xs:complexType>
      </xs:element>
      <xs:element name="GetPocketStartupData">
        <xs:complexType>
          <xs:sequence>
            <xs:element minOccurs="0" name="Tables" nillable="true" type="q19:ArrayOfstring" xmlns:q19="http://schemas.microsoft.com/2003/10/Serialization/Arrays" />
            <xs:element minOccurs="0" name="CurrentClientTime" type="xs:dateTime" />
          </xs:sequence>
        </xs:complexType>
      </xs:element>
      <xs:element name="GetPocketStartupDataResponse">
        <xs:complexType>
          <xs:sequence>
            <xs:element minOccurs="0" name="Response" nillable="true" type="q20:PocketStartupData" xmlns:q20="http://www.superoffice.net/ws/crm/NetServer/Services88" />
          </xs:sequence>
        </xs:complexType>
      </xs:element>
      <xs:complexType name="PocketStartupData">
        <xs:complexContent mixed="false">
          <xs:extension base="q21:Carrier" xmlns:q21="http://www.superoffice.net/ws/crm/NetServer/Services88">
            <xs:sequence>
              <xs:element minOccurs="0" name="TableRights" nillable="true" type="q21:ArrayOfETableRight" />
              <xs:element minOccurs="0" name="PhoneLocaleTimeZoneData" nillable="true" type="q21:TimeZoneData" />
              <xs:element minOccurs="0" name="BaseLocaleTimeZoneData" nillable="true" type="q21:TimeZoneData" />
              <xs:element minOccurs="0" name="OverdueSalesCount" type="xs:int" />
              <xs:element minOccurs="0" name="NotificationsCount" type="xs:int" />
              <xs:element minOccurs="0" name="SystemWebPanels" nillable="true" type="q21:ArrayOfWebPanelEntity" />
              <xs:element minOccurs="0" name="PocketPreferences" nillable="true" type="q21:ArrayOfPreference" />
              <xs:element minOccurs="0" name="IsPushNotificationEnabled" type="xs:boolean" />
              <xs:element minOccurs="0" name="CustomData" nillable="true" type="xs:string" />
            </xs:sequence>
          </xs:extension>
        </xs:complexContent>
      </xs:complexType>
      <xs:element name="PocketStartupData" nillable="true" type="q22:PocketStartupData" xmlns:q22="http://www.superoffice.net/ws/crm/NetServer/Services88" />
      <xs:complexType name="Carrier">
        <xs:sequence>
          <xs:element minOccurs="0" name="TableRight" nillable="true" type="q23:TableRight" xmlns:q23="http://www.superoffice.net/ws/crm/NetServer/Services88" />
          <xs:element minOccurs="0" name="FieldProperties" nillable="true" type="q24:FieldPropertyDictionary" xmlns:q24="http://www.superoffice.net/ws/crm/NetServer/Services88" />
        </xs:sequence>
      </xs:complexType>
      <xs:element name="Carrier" nillable="true" type="q25:Carrier" xmlns:q25="http://www.superoffice.net/ws/crm/NetServer/Services88" />
      <xs:complexType name="TableRight">
        <xs:sequence>
          <xs:element minOccurs="0" name="Mask" type="q26:ETableRight" xmlns:q26="http://www.superoffice.net/ws/crm/NetServer/Services88" />
          <xs:element minOccurs="0" name="Reason" nillable="true" type="xs:string" />
        </xs:sequence>
      </xs:complexType>
      <xs:element name="TableRight" nillable="true" type="q27:TableRight" xmlns:q27="http://www.superoffice.net/ws/crm/NetServer/Services88" />
      <xs:simpleType name="ETableRight">
        <xs:list>
          <xs:simpleType>
            <xs:restriction base="xs:string">
              <xs:enumeration value="Select" />
              <xs:enumeration value="Update" />
              <xs:enumeration value="Insert" />
              <xs:enumeration value="Delete" />
              <xs:enumeration value="Filtering" />
              <xs:enumeration value="RestrictedUpdate" />
              <xs:enumeration value="Unused1" />
              <xs:enumeration value="Uninitialized" />
              <xs:enumeration value="R">
                <xs:annotation>
                  <xs:appinfo>
                    <EnumerationValue xmlns="http://schemas.microsoft.com/2003/10/Serialization/">1</EnumerationValue>
                  </xs:appinfo>
                </xs:annotation>
              </xs:enumeration>
              <xs:enumeration value="F">
                <xs:annotation>
                  <xs:appinfo>
                    <EnumerationValue xmlns="http://schemas.microsoft.com/2003/10/Serialization/">16</EnumerationValue>
                  </xs:appinfo>
                </xs:annotation>
              </xs:enumeration>
            </xs:restriction>
          </xs:simpleType>
        </xs:list>
      </xs:simpleType>
      <xs:element name="ETableRight" nillable="true" type="q28:ETableRight" xmlns:q28="http://www.superoffice.net/ws/crm/NetServer/Services88" />
      <xs:complexType name="FieldPropertyDictionary">
        <xs:annotation>
          <xs:appinfo>
            <IsDictionary xmlns="http://schemas.microsoft.com/2003/10/Serialization/">true</IsDictionary>
          </xs:appinfo>
        </xs:annotation>
        <xs:sequence>
          <xs:element minOccurs="0" maxOccurs="unbounded" name="FieldPropertyDictionaryKeyValuePair">
            <xs:complexType>
              <xs:sequence>
                <xs:element name="Key" nillable="true" type="xs:string" />
                <xs:element name="Value" nillable="true" type="q29:FieldProperty" xmlns:q29="http://www.superoffice.net/ws/crm/NetServer/Services88" />
              </xs:sequence>
            </xs:complexType>
          </xs:element>
        </xs:sequence>
      </xs:complexType>
      <xs:element name="FieldPropertyDictionary" nillable="true" type="q30:FieldPropertyDictionary" xmlns:q30="http://www.superoffice.net/ws/crm/NetServer/Services88" />
      <xs:complexType name="FieldProperty">
        <xs:sequence>
          <xs:element minOccurs="0" name="FieldRight" nillable="true" type="q31:FieldRight" xmlns:q31="http://www.superoffice.net/ws/crm/NetServer/Services88" />
          <xs:element minOccurs="0" name="FieldType" nillable="true" type="xs:string" />
          <xs:element minOccurs="0" name="FieldLength" type="xs:int" />
        </xs:sequence>
      </xs:complexType>
      <xs:element name="FieldProperty" nillable="true" type="q32:FieldProperty" xmlns:q32="http://www.superoffice.net/ws/crm/NetServer/Services88" />
      <xs:complexType name="FieldRight">
        <xs:sequence>
          <xs:element minOccurs="0" name="Mask" type="q33:EFieldRight" xmlns:q33="http://www.superoffice.net/ws/crm/NetServer/Services88" />
          <xs:element minOccurs="0" name="Reason" nillable="true" type="xs:string" />
        </xs:sequence>
      </xs:complexType>
      <xs:element name="FieldRight" nillable="true" type="q34:FieldRight" xmlns:q34="http://www.superoffice.net/ws/crm/NetServer/Services88" />
      <xs:simpleType name="EFieldRight">
        <xs:list>
          <xs:simpleType>
            <xs:restriction base="xs:string">
              <xs:enumeration value="Read" />
              <xs:enumeration value="Write" />
              <xs:enumeration value="Unused1" />
              <xs:enumeration value="Unused2" />
              <xs:enumeration value="Unused3" />
              <xs:enumeration value="Unused4" />
              <xs:enumeration value="UIHintMandatory" />
              <xs:enumeration value="UIHintReadOnly" />
              <xs:enumeration value="UndefinedValue256" />
              <xs:enumeration value="Nullable">
                <xs:annotation>
                  <xs:appinfo>
                    <EnumerationValue xmlns="http://schemas.microsoft.com/2003/10/Serialization/">32</EnumerationValue>
                  </xs:appinfo>
                </xs:annotation>
              </xs:enumeration>
            </xs:restriction>
          </xs:simpleType>
        </xs:list>
      </xs:simpleType>
      <xs:element name="EFieldRight" nillable="true" type="q35:EFieldRight" xmlns:q35="http://www.superoffice.net/ws/crm/NetServer/Services88" />
      <xs:complexType name="ArrayOfETableRight">
        <xs:sequence>
          <xs:element minOccurs="0" maxOccurs="unbounded" name="ETableRight" type="q36:ETableRight" xmlns:q36="http://www.superoffice.net/ws/crm/NetServer/Services88" />
        </xs:sequence>
      </xs:complexType>
      <xs:element name="ArrayOfETableRight" nillable="true" type="q37:ArrayOfETableRight" xmlns:q37="http://www.superoffice.net/ws/crm/NetServer/Services88" />
      <xs:complexType name="TimeZoneData">
        <xs:sequence>
          <xs:element minOccurs="0" name="TZLocationID" type="xs:int" />
          <xs:element minOccurs="0" name="Name" nillable="true" type="xs:string" />
          <xs:element minOccurs="0" name="TZLocationCode" nillable="true" type="xs:string" />
          <xs:element minOccurs="0" name="TZLocationCities" nillable="true" type="xs:string" />
          <xs:element minOccurs="0" name="IsoNumber" type="xs:int" />
          <xs:element minOccurs="0" name="TimeZoneSTDRules" nillable="true" type="q38:TimeZoneRuleDictionary" xmlns:q38="http://www.superoffice.net/ws/crm/NetServer/Services88" />
          <xs:element minOccurs="0" name="TimeZoneDSTRules" nillable="true" type="q39:TimeZoneRuleDictionary" xmlns:q39="http://www.superoffice.net/ws/crm/NetServer/Services88" />
        </xs:sequence>
      </xs:complexType>
      <xs:element name="TimeZoneData" nillable="true" type="q40:TimeZoneData" xmlns:q40="http://www.superoffice.net/ws/crm/NetServer/Services88" />
      <xs:complexType name="TimeZoneRuleDictionary">
        <xs:annotation>
          <xs:appinfo>
            <IsDictionary xmlns="http://schemas.microsoft.com/2003/10/Serialization/">true</IsDictionary>
          </xs:appinfo>
        </xs:annotation>
        <xs:sequence>
          <xs:element minOccurs="0" maxOccurs="unbounded" name="TimeZoneRuleKeyValuePair">
            <xs:complexType>
              <xs:sequence>
                <xs:element name="Key" type="xs:dateTime" />
                <xs:element name="Value" nillable="true" type="q41:TimeZoneRule" xmlns:q41="http://www.superoffice.net/ws/crm/NetServer/Services88" />
              </xs:sequence>
            </xs:complexType>
          </xs:element>
        </xs:sequence>
      </xs:complexType>
      <xs:element name="TimeZoneRuleDictionary" nillable="true" type="q42:TimeZoneRuleDictionary" xmlns:q42="http://www.superoffice.net/ws/crm/NetServer/Services88" />
      <xs:complexType name="TimeZoneRule">
        <xs:sequence>
          <xs:element minOccurs="0" name="TZOffset" type="xs:int" />
          <xs:element minOccurs="0" name="StartRulePattern" nillable="true" type="xs:string" />
          <xs:element minOccurs="0" name="EndRulePattern" nillable="true" type="xs:string" />
          <xs:element minOccurs="0" name="StartDay" type="xs:int" />
          <xs:element minOccurs="0" name="StartMonth" type="xs:int" />
          <xs:element minOccurs="0" name="EndDay" type="xs:int" />
          <xs:element minOccurs="0" name="EndMonth" type="xs:int" />
        </xs:sequence>
      </xs:complexType>
      <xs:element name="TimeZoneRule" nillable="true" type="q43:TimeZoneRule" xmlns:q43="http://www.superoffice.net/ws/crm/NetServer/Services88" />
      <xs:complexType name="ArrayOfWebPanelEntity">
        <xs:sequence>
          <xs:element minOccurs="0" maxOccurs="unbounded" name="WebPanelEntity" nillable="true" type="q44:WebPanelEntity" xmlns:q44="http://www.superoffice.net/ws/crm/NetServer/Services88" />
        </xs:sequence>
      </xs:complexType>
      <xs:element name="ArrayOfWebPanelEntity" nillable="true" type="q45:ArrayOfWebPanelEntity" xmlns:q45="http://www.superoffice.net/ws/crm/NetServer/Services88" />
      <xs:complexType name="WebPanelEntity">
        <xs:complexContent mixed="false">
          <xs:extension base="q46:Carrier" xmlns:q46="http://www.superoffice.net/ws/crm/NetServer/Services88">
            <xs:sequence>
              <xs:element minOccurs="0" name="WebPanelId" type="xs:int" />
              <xs:element minOccurs="0" name="Name" nillable="true" type="xs:string" />
              <xs:element minOccurs="0" name="Tooltip" nillable="true" type="xs:string" />
              <xs:element minOccurs="0" name="Deleted" type="xs:boolean" />
              <xs:element minOccurs="0" name="Rank" type="xs:int" />
              <xs:element minOccurs="0" name="UrlEncoding" type="q46:UrlEncoding" />
              <xs:element minOccurs="0" name="VisibleIn" type="q46:Navigation" />
              <xs:element minOccurs="0" name="OnCentral" type="xs:boolean" />
              <xs:element minOccurs="0" name="OnSatellite" type="xs:boolean" />
              <xs:element minOccurs="0" name="OnTravel" type="xs:boolean" />
              <xs:element minOccurs="0" name="OnSalesMarketingWeb" type="xs:boolean" />
              <xs:element minOccurs="0" name="OnSalesMarketingPocket" type="xs:boolean" />
              <xs:element minOccurs="0" name="ShowInMenuBar" type="xs:boolean" />
              <xs:element minOccurs="0" name="ShowInToolBar" type="xs:boolean" />
              <xs:element minOccurs="0" name="ShowInAddressBar" type="xs:boolean" />
              <xs:element minOccurs="0" name="ShowInStatusBar" type="xs:boolean" />
              <xs:element minOccurs="0" name="WindowName" nillable="true" type="xs:string" />
              <xs:element minOccurs="0" name="Url" nillable="true" type="xs:string" />
              <xs:element minOccurs="0" name="ProgId" nillable="true" type="xs:string" />
              <xs:element minOccurs="0" name="Icon" type="xs:short" />
              <xs:element minOccurs="0" name="AlwaysReloadOnShow" type="xs:boolean" />
            </xs:sequence>
          </xs:extension>
        </xs:complexContent>
      </xs:complexType>
      <xs:element name="WebPanelEntity" nillable="true" type="q47:WebPanelEntity" xmlns:q47="http://www.superoffice.net/ws/crm/NetServer/Services88" />
      <xs:simpleType name="UrlEncoding">
        <xs:restriction base="xs:string">
          <xs:enumeration value="Unknown" />
          <xs:enumeration value="None" />
          <xs:enumeration value="ANSI" />
          <xs:enumeration value="Unicode" />
        </xs:restriction>
      </xs:simpleType>
      <xs:element name="UrlEncoding" nillable="true" type="q48:UrlEncoding" xmlns:q48="http://www.superoffice.net/ws/crm/NetServer/Services88" />
      <xs:simpleType name="Navigation">
        <xs:annotation>
          <xs:appinfo>
            <ActualType Name="short" Namespace="http://www.w3.org/2001/XMLSchema" xmlns="http://schemas.microsoft.com/2003/10/Serialization/" />
          </xs:appinfo>
        </xs:annotation>
        <xs:restriction base="xs:string">
          <xs:enumeration value="Invisible" />
          <xs:enumeration value="ToolboxMenu" />
          <xs:enumeration value="NavigatorButton" />
          <xs:enumeration value="ViewMenu" />
          <xs:enumeration value="SelectionTaskCard" />
          <xs:enumeration value="ContactCard" />
          <xs:enumeration value="ContactArchive" />
          <xs:enumeration value="ProjectCard" />
          <xs:enumeration value="ProjectArchive" />
          <xs:enumeration value="SaleCard" />
          <xs:enumeration value="PersonCard" />
          <xs:enumeration value="ActivityDialog" />
          <xs:enumeration value="DocumentDialog" />
          <xs:enumeration value="BrowserPanel" />
          <xs:enumeration value="ContSelectionTask" />
          <xs:enumeration value="AppntSelectionTask" />
          <xs:enumeration value="SaleSelectionTask" />
          <xs:enumeration value="DocSelectionTask" />
          <xs:enumeration value="ProjSelectionTask" />
          <xs:enumeration value="CompanyMinicard" />
          <xs:enumeration value="ProjectMinicard" />
          <xs:enumeration value="DiaryMinicard" />
          <xs:enumeration value="SelectionMinicard" />
          <xs:enumeration value="ButtonPanelTask" />
          <xs:enumeration value="AppointmentDialogTask" />
          <xs:enumeration value="SaleDialogTask" />
          <xs:enumeration value="DocumentDialogTask" />
          <xs:enumeration value="PersonDialogTask" />
          <xs:enumeration value="SaleMinicard" />
          <xs:enumeration value="SaleArchive" />
          <xs:enumeration value="AppntSelectionShadowTask" />
          <xs:enumeration value="SaleSelectionShadowTask" />
          <xs:enumeration value="DocSelectionShadowTask" />
          <xs:enumeration value="ProjSelectionShadowTask" />
          <xs:enumeration value="DiaryArchive" />
          <xs:enumeration value="SelectionContactArchive" />
          <xs:enumeration value="SelectionProjectArchive" />
          <xs:enumeration value="SelectionSaleArchive" />
          <xs:enumeration value="SelectionAppointmentArchive" />
          <xs:enumeration value="SelectionDocumentArchive" />
          <xs:enumeration value="ContSelectionCustomTask" />
          <xs:enumeration value="AppntSelectionCustomTask" />
          <xs:enumeration value="SaleSelectionCustomTask" />
          <xs:enumeration value="DocSelectionCustomTask" />
          <xs:enumeration value="ProjSelectionCustomTask" />
          <xs:enumeration value="CustomArchiveMiniCard" />
          <xs:enumeration value="SelectionCard" />
          <xs:enumeration value="ReportMinicard" />
          <xs:enumeration value="QuoteDialog" />
          <xs:enumeration value="QuoteDialogTask" />
          <xs:enumeration value="QuoteDialogArchive" />
          <xs:enumeration value="QuoteLineDialogTask" />
          <xs:enumeration value="QuoteLineDialog" />
          <xs:enumeration value="QuoteLineSelectionMainTask" />
          <xs:enumeration value="QuoteLineSelectionShadowTask" />
          <xs:enumeration value="SelectionQuoteLineArchive" />
          <xs:enumeration value="QuoteLineSelectionCustomTask" />
          <xs:enumeration value="FindSystem" />
          <xs:enumeration value="MailingSelectionTask" />
          <xs:enumeration value="ContactSelectionMailingsTask" />
          <xs:enumeration value="AppointmentSelectionMailingsTask" />
          <xs:enumeration value="SaleSelectionMailingsTask" />
          <xs:enumeration value="DocumentSelectionMailingsTask" />
          <xs:enumeration value="ProjectSelectionMailingsTask" />
          <xs:enumeration value="QuoteLineSelectionMailingsTask" />
          <xs:enumeration value="TopPanelNewMenu" />
          <xs:enumeration value="Dashboard" />
          <xs:enumeration value="PersonArchive" />
          <xs:enumeration value="PersonMinicard" />
          <xs:enumeration value="CompanyCardTask" />
          <xs:enumeration value="ProjectCardTask" />
        </xs:restriction>
      </xs:simpleType>
      <xs:element name="Navigation" nillable="true" type="q49:Navigation" xmlns:q49="http://www.superoffice.net/ws/crm/NetServer/Services88" />
      <xs:complexType name="ArrayOfPreference">
        <xs:sequence>
          <xs:element minOccurs="0" maxOccurs="unbounded" name="Preference" nillable="true" type="q50:Preference" xmlns:q50="http://www.superoffice.net/ws/crm/NetServer/Services88" />
        </xs:sequence>
      </xs:complexType>
      <xs:element name="ArrayOfPreference" nillable="true" type="q51:ArrayOfPreference" xmlns:q51="http://www.superoffice.net/ws/crm/NetServer/Services88" />
      <xs:complexType name="Preference">
        <xs:complexContent mixed="false">
          <xs:extension base="q52:Carrier" xmlns:q52="http://www.superoffice.net/ws/crm/NetServer/Services88">
            <xs:sequence>
              <xs:element minOccurs="0" name="Level" type="q52:PreferenceLevel" />
              <xs:element minOccurs="0" name="RawValue" nillable="true" type="xs:string" />
              <xs:element minOccurs="0" name="Specification" nillable="true" type="q52:PreferenceSpec" />
              <xs:element minOccurs="0" name="DisplayValue" nillable="true" type="xs:string" />
              <xs:element minOccurs="0" name="DisplayTooltip" nillable="true" type="xs:string" />
              <xs:element minOccurs="0" name="DisplayType" type="q52:PrefDescValueType" />
              <xs:element minOccurs="0" name="TabOrder" nillable="true" type="q52:TabOrder" />
              <xs:element minOccurs="0" name="TargetId" type="xs:int" />
              <xs:element minOccurs="0" name="PrefDescId" type="xs:int" />
              <xs:element minOccurs="0" name="TableName" nillable="true" type="xs:string" />
              <xs:element minOccurs="0" name="UserPreferenceId" type="xs:int" />
            </xs:sequence>
          </xs:extension>
        </xs:complexContent>
      </xs:complexType>
      <xs:element name="Preference" nillable="true" type="q53:Preference" xmlns:q53="http://www.superoffice.net/ws/crm/NetServer/Services88" />
      <xs:simpleType name="PreferenceLevel">
        <xs:annotation>
          <xs:appinfo>
            <ActualType Name="short" Namespace="http://www.w3.org/2001/XMLSchema" xmlns="http://schemas.microsoft.com/2003/10/Serialization/" />
          </xs:appinfo>
        </xs:annotation>
        <xs:restriction base="xs:string">
          <xs:enumeration value="Undefined" />
          <xs:enumeration value="HardDefault" />
          <xs:enumeration value="SystemWide" />
          <xs:enumeration value="Database" />
          <xs:enumeration value="Group" />
          <xs:enumeration value="Individual" />
          <xs:enumeration value="PC" />
        </xs:restriction>
      </xs:simpleType>
      <xs:element name="PreferenceLevel" nillable="true" type="q54:PreferenceLevel" xmlns:q54="http://www.superoffice.net/ws/crm/NetServer/Services88" />
      <xs:complexType name="PreferenceSpec">
        <xs:complexContent mixed="false">
          <xs:extension base="q55:Carrier" xmlns:q55="http://www.superoffice.net/ws/crm/NetServer/Services88">
            <xs:sequence>
              <xs:element minOccurs="0" name="Section" nillable="true" type="xs:string" />
              <xs:element minOccurs="0" name="Key" nillable="true" type="xs:string" />
            </xs:sequence>
          </xs:extension>
        </xs:complexContent>
      </xs:complexType>
      <xs:element name="PreferenceSpec" nillable="true" type="q56:PreferenceSpec" xmlns:q56="http://www.superoffice.net/ws/crm/NetServer/Services88" />
      <xs:simpleType name="PrefDescValueType">
        <xs:annotation>
          <xs:appinfo>
            <ActualType Name="short" Namespace="http://www.w3.org/2001/XMLSchema" xmlns="http://schemas.microsoft.com/2003/10/Serialization/" />
          </xs:appinfo>
        </xs:annotation>
        <xs:restriction base="xs:string">
          <xs:enumeration value="Unknown" />
          <xs:enumeration value="Number" />
          <xs:enumeration value="Text" />
          <xs:enumeration value="Bool" />
          <xs:enumeration value="ListOfValues" />
          <xs:enumeration value="ListTableRef" />
          <xs:enumeration value="TimeList" />
          <xs:enumeration value="ContactID" />
          <xs:enumeration value="PersonID" />
          <xs:enumeration value="ProjectID" />
          <xs:enumeration value="SelectionID" />
          <xs:enumeration value="PosSize" />
          <xs:enumeration value="TimeZone" />
          <xs:enumeration value="Time" />
          <xs:enumeration value="Password" />
          <xs:enumeration value="MultiLineText" />
        </xs:restriction>
      </xs:simpleType>
      <xs:element name="PrefDescValueType" nillable="true" type="q57:PrefDescValueType" xmlns:q57="http://www.superoffice.net/ws/crm/NetServer/Services88" />
      <xs:complexType name="TabOrder">
        <xs:complexContent mixed="false">
          <xs:extension base="q58:Carrier" xmlns:q58="http://www.superoffice.net/ws/crm/NetServer/Services88">
            <xs:sequence>
              <xs:element minOccurs="0" name="TabOrderId" type="xs:int" />
              <xs:element minOccurs="0" name="TabName" nillable="true" type="xs:string" />
              <xs:element minOccurs="0" name="Order" nillable="true" type="xs:string" />
              <xs:element minOccurs="0" name="AssociateId" type="xs:int" />
            </xs:sequence>
          </xs:extension>
        </xs:complexContent>
      </xs:complexType>
      <xs:element name="TabOrder" nillable="true" type="q59:TabOrder" xmlns:q59="http://www.superoffice.net/ws/crm/NetServer/Services88" />
      <xs:element name="RegisterDeviceForPushNotification">
        <xs:complexType>
          <xs:sequence>
            <xs:element minOccurs="0" name="DeviceInfo" nillable="true" type="q60:PocketDeviceInfo" xmlns:q60="http://www.superoffice.net/ws/crm/NetServer/Services88" />
          </xs:sequence>
        </xs:complexType>
      </xs:element>
      <xs:complexType name="PocketDeviceInfo">
        <xs:sequence>
          <xs:element minOccurs="0" name="DeviceName" nillable="true" type="xs:string" />
          <xs:element minOccurs="0" name="DeviceIdentifier" nillable="true" type="xs:string" />
          <xs:element minOccurs="0" name="PocketVersion" nillable="true" type="xs:string" />
          <xs:element minOccurs="0" name="Language" nillable="true" type="xs:string" />
          <xs:element minOccurs="0" name="PNSHandle" nillable="true" type="xs:string" />
          <xs:element minOccurs="0" name="Platform" type="q61:NotificationPlatform" xmlns:q61="http://www.superoffice.net/ws/crm/NetServer/Services88" />
          <xs:element minOccurs="0" name="OSVersion" nillable="true" type="xs:string" />
          <xs:element minOccurs="0" name="TimeZoneId" type="xs:int" />
        </xs:sequence>
      </xs:complexType>
      <xs:element name="PocketDeviceInfo" nillable="true" type="q62:PocketDeviceInfo" xmlns:q62="http://www.superoffice.net/ws/crm/NetServer/Services88" />
      <xs:simpleType name="NotificationPlatform">
        <xs:annotation>
          <xs:appinfo>
            <ActualType Name="short" Namespace="http://www.w3.org/2001/XMLSchema" xmlns="http://schemas.microsoft.com/2003/10/Serialization/" />
          </xs:appinfo>
        </xs:annotation>
        <xs:restriction base="xs:string">
          <xs:enumeration value="Apple" />
          <xs:enumeration value="Google" />
          <xs:enumeration value="Microsoft" />
          <xs:enumeration value="AppleDeveloper" />
          <xs:enumeration value="AppleAdHoc" />
          <xs:enumeration value="GoogleDeveloper" />
        </xs:restriction>
      </xs:simpleType>
      <xs:element name="NotificationPlatform" nillable="true" type="q63:NotificationPlatform" xmlns:q63="http://www.superoffice.net/ws/crm/NetServer/Services88" />
      <xs:element name="RegisterDeviceForPushNotificationResponse">
        <xs:complexType>
          <xs:sequence />
        </xs:complexType>
      </xs:element>
      <xs:element name="GetRegisteredDevices">
        <xs:complexType>
          <xs:sequence>
            <xs:element minOccurs="0" name="AssociateId" type="xs:int" />
          </xs:sequence>
        </xs:complexType>
      </xs:element>
      <xs:element name="GetRegisteredDevicesResponse">
        <xs:complexType>
          <xs:sequence>
            <xs:element minOccurs="0" name="Response" nillable="true" type="q64:ArrayOfPocketDeviceInfo" xmlns:q64="http://www.superoffice.net/ws/crm/NetServer/Services88" />
          </xs:sequence>
        </xs:complexType>
      </xs:element>
      <xs:complexType name="ArrayOfPocketDeviceInfo">
        <xs:sequence>
          <xs:element minOccurs="0" maxOccurs="unbounded" name="PocketDeviceInfo" nillable="true" type="q65:PocketDeviceInfo" xmlns:q65="http://www.superoffice.net/ws/crm/NetServer/Services88" />
        </xs:sequence>
      </xs:complexType>
      <xs:element name="ArrayOfPocketDeviceInfo" nillable="true" type="q66:ArrayOfPocketDeviceInfo" xmlns:q66="http://www.superoffice.net/ws/crm/NetServer/Services88" />
      <xs:element name="SetPushNotificationTagsForDevice">
        <xs:complexType>
          <xs:sequence>
            <xs:element minOccurs="0" name="DeviceIdentifier" nillable="true" type="xs:string" />
            <xs:element minOccurs="0" name="Tags" nillable="true" type="xs:string" />
          </xs:sequence>
        </xs:complexType>
      </xs:element>
      <xs:element name="SetPushNotificationTagsForDeviceResponse">
        <xs:complexType>
          <xs:sequence />
        </xs:complexType>
      </xs:element>
      <xs:element name="SetPushNotificationTagsForUser">
        <xs:complexType>
          <xs:sequence>
            <xs:element minOccurs="0" name="AssociateId" type="xs:int" />
            <xs:element minOccurs="0" name="Tags" nillable="true" type="xs:string" />
          </xs:sequence>
        </xs:complexType>
      </xs:element>
      <xs:element name="SetPushNotificationTagsForUserResponse">
        <xs:complexType>
          <xs:sequence />
        </xs:complexType>
      </xs:element>
      <xs:element name="GetPushNotificationTagsForDevice">
        <xs:complexType>
          <xs:sequence>
            <xs:element minOccurs="0" name="DeviceIdentifier" nillable="true" type="xs:string" />
          </xs:sequence>
        </xs:complexType>
      </xs:element>
      <xs:element name="GetPushNotificationTagsForDeviceResponse">
        <xs:complexType>
          <xs:sequence>
            <xs:element minOccurs="0" name="Response" nillable="true" type="xs:string" />
          </xs:sequence>
        </xs:complexType>
      </xs:element>
      <xs:element name="SendPushNotification">
        <xs:complexType>
          <xs:sequence>
            <xs:element minOccurs="0" name="AssociateIds" nillable="true" type="q67:ArrayOfint" xmlns:q67="http://schemas.microsoft.com/2003/10/Serialization/Arrays" />
            <xs:element minOccurs="0" name="Message" nillable="true" type="q68:PocketNotificationMessage" xmlns:q68="http://www.superoffice.net/ws/crm/NetServer/Services88" />
          </xs:sequence>
        </xs:complexType>
      </xs:element>
      <xs:complexType name="PocketNotificationMessage">
        <xs:sequence>
          <xs:element minOccurs="0" name="Title" nillable="true" type="xs:string" />
          <xs:element minOccurs="0" name="Message" nillable="true" type="xs:string" />
          <xs:element minOccurs="0" name="Url" nillable="true" type="xs:string" />
          <xs:element minOccurs="0" name="Silent" type="xs:boolean" />
          <xs:element minOccurs="0" name="Type" type="q69:NotificationMessageType" xmlns:q69="http://www.superoffice.net/ws/crm/NetServer/Services88" />
          <xs:element minOccurs="0" name="TimeToLive" type="xs:int" />
          <xs:element minOccurs="0" name="RecordId" type="xs:int" />
          <xs:element minOccurs="0" name="Date" type="xs:dateTime" />
          <xs:element minOccurs="0" name="Duration" type="ser:duration" />
          <xs:element minOccurs="0" name="ExtraValues" nillable="true" type="q70:StringDictionary" xmlns:q70="http://www.superoffice.net/ws/crm/NetServer/Services88" />
        </xs:sequence>
      </xs:complexType>
      <xs:element name="PocketNotificationMessage" nillable="true" type="q71:PocketNotificationMessage" xmlns:q71="http://www.superoffice.net/ws/crm/NetServer/Services88" />
      <xs:simpleType name="NotificationMessageType">
        <xs:restriction base="xs:string">
          <xs:enumeration value="Message" />
          <xs:enumeration value="ImportantMessage" />
          <xs:enumeration value="RemoteAction" />
          <xs:enumeration value="YesNoQuestion" />
          <xs:enumeration value="ShowWebPage" />
        </xs:restriction>
      </xs:simpleType>
      <xs:element name="NotificationMessageType" nillable="true" type="q72:NotificationMessageType" xmlns:q72="http://www.superoffice.net/ws/crm/NetServer/Services88" />
      <xs:complexType name="StringDictionary">
        <xs:annotation>
          <xs:appinfo>
            <IsDictionary xmlns="http://schemas.microsoft.com/2003/10/Serialization/">true</IsDictionary>
          </xs:appinfo>
        </xs:annotation>
        <xs:sequence>
          <xs:element minOccurs="0" maxOccurs="unbounded" name="StringKeyValuePair">
            <xs:complexType>
              <xs:sequence>
                <xs:element name="Key" nillable="true" type="xs:string" />
                <xs:element name="Value" nillable="true" type="xs:string" />
              </xs:sequence>
            </xs:complexType>
          </xs:element>
        </xs:sequence>
      </xs:complexType>
      <xs:element name="StringDictionary" nillable="true" type="q73:StringDictionary" xmlns:q73="http://www.superoffice.net/ws/crm/NetServer/Services88" />
      <xs:element name="SendPushNotificationResponse">
        <xs:complexType>
          <xs:sequence />
        </xs:complexType>
      </xs:element>
      <xs:element name="RunAppointmentAlarmBroker">
        <xs:complexType>
          <xs:sequence />
        </xs:complexType>
      </xs:element>
      <xs:element name="RunAppointmentAlarmBrokerResponse">
        <xs:complexType>
          <xs:sequence />
        </xs:complexType>
      </xs:element>
      <xs:element name="NotifyUsers">
        <xs:complexType>
          <xs:sequence>
            <xs:element minOccurs="0" name="NotificationEventType" type="q74:NotificationEventType" xmlns:q74="http://www.superoffice.net/ws/crm/NetServer/Services88" />
            <xs:element minOccurs="0" name="Id" type="xs:int" />
          </xs:sequence>
        </xs:complexType>
      </xs:element>
      <xs:simpleType name="NotificationEventType">
        <xs:restriction base="xs:string">
          <xs:enumeration value="Unknown" />
          <xs:enumeration value="NewTicket" />
          <xs:enumeration value="AppointmentInvitation" />
          <xs:enumeration value="AppointmentMoved" />
          <xs:enumeration value="AppointmentCancelled" />
          <xs:enumeration value="NewTicketMessage" />
          <xs:enumeration value="TicketActivated" />
          <xs:enumeration value="TicketEscalated" />
          <xs:enumeration value="QuoteApprovalRequest" />
          <xs:enumeration value="QuoteApprovalApproved" />
          <xs:enumeration value="QuoteApprovalDenied" />
        </xs:restriction>
      </xs:simpleType>
      <xs:element name="NotificationEventType" nillable="true" type="q75:NotificationEventType" xmlns:q75="http://www.superoffice.net/ws/crm/NetServer/Services88" />
      <xs:element name="NotifyUsersResponse">
        <xs:complexType>
          <xs:sequence />
        </xs:complexType>
      </xs:element>
      <xs:element name="NotificationHandled">
        <xs:complexType>
          <xs:sequence>
            <xs:element minOccurs="0" name="NotificationEventType" type="q76:NotificationEventType" xmlns:q76="http://www.superoffice.net/ws/crm/NetServer/Services88" />
            <xs:element minOccurs="0" name="Id" type="xs:int" />
          </xs:sequence>
        </xs:complexType>
      </xs:element>
      <xs:element name="NotificationHandledResponse">
        <xs:complexType>
          <xs:sequence />
        </xs:complexType>
      </xs:element>
      <xs:element name="NotificationsHandled">
        <xs:complexType>
          <xs:sequence>
            <xs:element minOccurs="0" name="NotificationEvents" nillable="true" type="q77:ArrayOfNotificationEvent" xmlns:q77="http://www.superoffice.net/ws/crm/NetServer/Services88" />
          </xs:sequence>
        </xs:complexType>
      </xs:element>
      <xs:complexType name="ArrayOfNotificationEvent">
        <xs:sequence>
          <xs:element minOccurs="0" maxOccurs="unbounded" name="NotificationEvent" nillable="true" type="q78:NotificationEvent" xmlns:q78="http://www.superoffice.net/ws/crm/NetServer/Services88" />
        </xs:sequence>
      </xs:complexType>
      <xs:element name="ArrayOfNotificationEvent" nillable="true" type="q79:ArrayOfNotificationEvent" xmlns:q79="http://www.superoffice.net/ws/crm/NetServer/Services88" />
      <xs:complexType name="NotificationEvent">
        <xs:sequence>
          <xs:element minOccurs="0" name="Type" type="q80:NotificationEventType" xmlns:q80="http://www.superoffice.net/ws/crm/NetServer/Services88" />
          <xs:element minOccurs="0" name="Id" type="xs:int" />
        </xs:sequence>
      </xs:complexType>
      <xs:element name="NotificationEvent" nillable="true" type="q81:NotificationEvent" xmlns:q81="http://www.superoffice.net/ws/crm/NetServer/Services88" />
      <xs:element name="NotificationsHandledResponse">
        <xs:complexType>
          <xs:sequence />
        </xs:complexType>
      </xs:element>
    </xs:schema>
    <xs:schema attributeFormDefault="qualified" elementFormDefault="qualified" targetNamespace="http://schemas.microsoft.com/2003/10/Serialization/" xmlns:xs="http://www.w3.org/2001/XMLSchema" xmlns:tns="http://schemas.microsoft.com/2003/10/Serialization/">
      <xs:element name="anyType" nillable="true" type="xs:anyType" />
      <xs:element name="anyURI" nillable="true" type="xs:anyURI" />
      <xs:element name="base64Binary" nillable="true" type="xs:base64Binary" />
      <xs:element name="boolean" nillable="true" type="xs:boolean" />
      <xs:element name="byte" nillable="true" type="xs:byte" />
      <xs:element name="dateTime" nillable="true" type="xs:dateTime" />
      <xs:element name="decimal" nillable="true" type="xs:decimal" />
      <xs:element name="double" nillable="true" type="xs:double" />
      <xs:element name="float" nillable="true" type="xs:float" />
      <xs:element name="int" nillable="true" type="xs:int" />
      <xs:element name="long" nillable="true" type="xs:long" />
      <xs:element name="QName" nillable="true" type="xs:QName" />
      <xs:element name="short" nillable="true" type="xs:short" />
      <xs:element name="string" nillable="true" type="xs:string" />
      <xs:element name="unsignedByte" nillable="true" type="xs:unsignedByte" />
      <xs:element name="unsignedInt" nillable="true" type="xs:unsignedInt" />
      <xs:element name="unsignedLong" nillable="true" type="xs:unsignedLong" />
      <xs:element name="unsignedShort" nillable="true" type="xs:unsignedShort" />
      <xs:element name="char" nillable="true" type="tns:char" />
      <xs:simpleType name="char">
        <xs:restriction base="xs:int" />
      </xs:simpleType>
      <xs:element name="duration" nillable="true" type="tns:duration" />
      <xs:simpleType name="duration">
        <xs:restriction base="xs:duration">
          <xs:pattern value="\-?P(\d*D)?(T(\d*H)?(\d*M)?(\d*(\.\d*)?S)?)?" />
          <xs:minInclusive value="-P10675199DT2H48M5.4775808S" />
          <xs:maxInclusive value="P10675199DT2H48M5.4775807S" />
        </xs:restriction>
      </xs:simpleType>
      <xs:element name="guid" nillable="true" type="tns:guid" />
      <xs:simpleType name="guid">
        <xs:restriction base="xs:string">
          <xs:pattern value="[\da-fA-F]{8}-[\da-fA-F]{4}-[\da-fA-F]{4}-[\da-fA-F]{4}-[\da-fA-F]{12}" />
        </xs:restriction>
      </xs:simpleType>
      <xs:attribute name="FactoryType" type="xs:QName" />
      <xs:attribute name="Id" type="xs:ID" />
      <xs:attribute name="Ref" type="xs:IDREF" />
    </xs:schema>
    <xs:schema elementFormDefault="qualified" targetNamespace="http://schemas.microsoft.com/2003/10/Serialization/Arrays" xmlns:xs="http://www.w3.org/2001/XMLSchema" xmlns:tns="http://schemas.microsoft.com/2003/10/Serialization/Arrays">
      <xs:complexType name="ArrayOfstring">
        <xs:sequence>
          <xs:element minOccurs="0" maxOccurs="unbounded" name="string" nillable="true" type="xs:string" />
        </xs:sequence>
      </xs:complexType>
      <xs:element name="ArrayOfstring" nillable="true" type="tns:ArrayOfstring" />
      <xs:complexType name="ArrayOfint">
        <xs:sequence>
          <xs:element minOccurs="0" maxOccurs="unbounded" name="int" type="xs:int" />
        </xs:sequence>
      </xs:complexType>
      <xs:element name="ArrayOfint" nillable="true" type="tns:ArrayOfint" />
    </xs:schema>
  </wsdl:types>
  <wsdl:message name="GetMyCallerIDsRequest">
    <wsdl:part name="parameters" element="tns:GetMyCallerIDs" />
  </wsdl:message>
  <wsdl:message name="GetMyCallerIDsRequest_Headers">
    <wsdl:part name="ApplicationToken" element="tns:ApplicationToken" />
    <wsdl:part name="Credentials" element="tns:Credentials" />
    <wsdl:part name="TimeZone" element="tns:TimeZone" />
  </wsdl:message>
  <wsdl:message name="GetMyCallerIDsResponse">
    <wsdl:part name="parameters" element="tns:GetMyCallerIDsResponse" />
  </wsdl:message>
  <wsdl:message name="GetMyCallerIDsResponse_Headers">
    <wsdl:part name="ExceptionInfo" element="tns:ExceptionInfo" />
    <wsdl:part name="ExtraInfo" element="tns:ExtraInfo" />
    <wsdl:part name="Succeeded" element="tns:Succeeded" />
    <wsdl:part name="TimeZone" element="tns:TimeZone" />
  </wsdl:message>
  <wsdl:message name="GetCallerIDsFromSelectionRequest">
    <wsdl:part name="parameters" element="tns:GetCallerIDsFromSelection" />
  </wsdl:message>
  <wsdl:message name="GetCallerIDsFromSelectionRequest_Headers">
    <wsdl:part name="ApplicationToken" element="tns:ApplicationToken" />
    <wsdl:part name="Credentials" element="tns:Credentials" />
    <wsdl:part name="TimeZone" element="tns:TimeZone" />
  </wsdl:message>
  <wsdl:message name="GetCallerIDsFromSelectionResponse">
    <wsdl:part name="parameters" element="tns:GetCallerIDsFromSelectionResponse" />
  </wsdl:message>
  <wsdl:message name="GetCallerIDsFromSelectionResponse_Headers">
    <wsdl:part name="ExceptionInfo" element="tns:ExceptionInfo" />
    <wsdl:part name="ExtraInfo" element="tns:ExtraInfo" />
    <wsdl:part name="Succeeded" element="tns:Succeeded" />
    <wsdl:part name="TimeZone" element="tns:TimeZone" />
  </wsdl:message>
  <wsdl:message name="GetPocketStartupDataRequest">
    <wsdl:part name="parameters" element="tns:GetPocketStartupData" />
  </wsdl:message>
  <wsdl:message name="GetPocketStartupDataRequest_Headers">
    <wsdl:part name="ApplicationToken" element="tns:ApplicationToken" />
    <wsdl:part name="Credentials" element="tns:Credentials" />
    <wsdl:part name="TimeZone" element="tns:TimeZone" />
  </wsdl:message>
  <wsdl:message name="GetPocketStartupDataResponse">
    <wsdl:part name="parameters" element="tns:GetPocketStartupDataResponse" />
  </wsdl:message>
  <wsdl:message name="GetPocketStartupDataResponse_Headers">
    <wsdl:part name="ExceptionInfo" element="tns:ExceptionInfo" />
    <wsdl:part name="ExtraInfo" element="tns:ExtraInfo" />
    <wsdl:part name="Succeeded" element="tns:Succeeded" />
    <wsdl:part name="TimeZone" element="tns:TimeZone" />
  </wsdl:message>
  <wsdl:message name="RegisterDeviceForPushNotificationRequest">
    <wsdl:part name="parameters" element="tns:RegisterDeviceForPushNotification" />
  </wsdl:message>
  <wsdl:message name="RegisterDeviceForPushNotificationRequest_Headers">
    <wsdl:part name="ApplicationToken" element="tns:ApplicationToken" />
    <wsdl:part name="Credentials" element="tns:Credentials" />
    <wsdl:part name="TimeZone" element="tns:TimeZone" />
  </wsdl:message>
  <wsdl:message name="RegisterDeviceForPushNotificationResponse">
    <wsdl:part name="parameters" element="tns:RegisterDeviceForPushNotificationResponse" />
  </wsdl:message>
  <wsdl:message name="RegisterDeviceForPushNotificationResponse_Headers">
    <wsdl:part name="ExceptionInfo" element="tns:ExceptionInfo" />
    <wsdl:part name="ExtraInfo" element="tns:ExtraInfo" />
    <wsdl:part name="Succeeded" element="tns:Succeeded" />
    <wsdl:part name="TimeZone" element="tns:TimeZone" />
  </wsdl:message>
  <wsdl:message name="GetRegisteredDevicesRequest">
    <wsdl:part name="parameters" element="tns:GetRegisteredDevices" />
  </wsdl:message>
  <wsdl:message name="GetRegisteredDevicesRequest_Headers">
    <wsdl:part name="ApplicationToken" element="tns:ApplicationToken" />
    <wsdl:part name="Credentials" element="tns:Credentials" />
    <wsdl:part name="TimeZone" element="tns:TimeZone" />
  </wsdl:message>
  <wsdl:message name="GetRegisteredDevicesResponse">
    <wsdl:part name="parameters" element="tns:GetRegisteredDevicesResponse" />
  </wsdl:message>
  <wsdl:message name="GetRegisteredDevicesResponse_Headers">
    <wsdl:part name="ExceptionInfo" element="tns:ExceptionInfo" />
    <wsdl:part name="ExtraInfo" element="tns:ExtraInfo" />
    <wsdl:part name="Succeeded" element="tns:Succeeded" />
    <wsdl:part name="TimeZone" element="tns:TimeZone" />
  </wsdl:message>
  <wsdl:message name="SetPushNotificationTagsForDeviceRequest">
    <wsdl:part name="parameters" element="tns:SetPushNotificationTagsForDevice" />
  </wsdl:message>
  <wsdl:message name="SetPushNotificationTagsForDeviceRequest_Headers">
    <wsdl:part name="ApplicationToken" element="tns:ApplicationToken" />
    <wsdl:part name="Credentials" element="tns:Credentials" />
    <wsdl:part name="TimeZone" element="tns:TimeZone" />
  </wsdl:message>
  <wsdl:message name="SetPushNotificationTagsForDeviceResponse">
    <wsdl:part name="parameters" element="tns:SetPushNotificationTagsForDeviceResponse" />
  </wsdl:message>
  <wsdl:message name="SetPushNotificationTagsForDeviceResponse_Headers">
    <wsdl:part name="ExceptionInfo" element="tns:ExceptionInfo" />
    <wsdl:part name="ExtraInfo" element="tns:ExtraInfo" />
    <wsdl:part name="Succeeded" element="tns:Succeeded" />
    <wsdl:part name="TimeZone" element="tns:TimeZone" />
  </wsdl:message>
  <wsdl:message name="SetPushNotificationTagsForUserRequest">
    <wsdl:part name="parameters" element="tns:SetPushNotificationTagsForUser" />
  </wsdl:message>
  <wsdl:message name="SetPushNotificationTagsForUserRequest_Headers">
    <wsdl:part name="ApplicationToken" element="tns:ApplicationToken" />
    <wsdl:part name="Credentials" element="tns:Credentials" />
    <wsdl:part name="TimeZone" element="tns:TimeZone" />
  </wsdl:message>
  <wsdl:message name="SetPushNotificationTagsForUserResponse">
    <wsdl:part name="parameters" element="tns:SetPushNotificationTagsForUserResponse" />
  </wsdl:message>
  <wsdl:message name="SetPushNotificationTagsForUserResponse_Headers">
    <wsdl:part name="ExceptionInfo" element="tns:ExceptionInfo" />
    <wsdl:part name="ExtraInfo" element="tns:ExtraInfo" />
    <wsdl:part name="Succeeded" element="tns:Succeeded" />
    <wsdl:part name="TimeZone" element="tns:TimeZone" />
  </wsdl:message>
  <wsdl:message name="GetPushNotificationTagsForDeviceRequest">
    <wsdl:part name="parameters" element="tns:GetPushNotificationTagsForDevice" />
  </wsdl:message>
  <wsdl:message name="GetPushNotificationTagsForDeviceRequest_Headers">
    <wsdl:part name="ApplicationToken" element="tns:ApplicationToken" />
    <wsdl:part name="Credentials" element="tns:Credentials" />
    <wsdl:part name="TimeZone" element="tns:TimeZone" />
  </wsdl:message>
  <wsdl:message name="GetPushNotificationTagsForDeviceResponse">
    <wsdl:part name="parameters" element="tns:GetPushNotificationTagsForDeviceResponse" />
  </wsdl:message>
  <wsdl:message name="GetPushNotificationTagsForDeviceResponse_Headers">
    <wsdl:part name="ExceptionInfo" element="tns:ExceptionInfo" />
    <wsdl:part name="ExtraInfo" element="tns:ExtraInfo" />
    <wsdl:part name="Succeeded" element="tns:Succeeded" />
    <wsdl:part name="TimeZone" element="tns:TimeZone" />
  </wsdl:message>
  <wsdl:message name="SendPushNotificationRequest">
    <wsdl:part name="parameters" element="tns:SendPushNotification" />
  </wsdl:message>
  <wsdl:message name="SendPushNotificationRequest_Headers">
    <wsdl:part name="ApplicationToken" element="tns:ApplicationToken" />
    <wsdl:part name="Credentials" element="tns:Credentials" />
    <wsdl:part name="TimeZone" element="tns:TimeZone" />
  </wsdl:message>
  <wsdl:message name="SendPushNotificationResponse">
    <wsdl:part name="parameters" element="tns:SendPushNotificationResponse" />
  </wsdl:message>
  <wsdl:message name="SendPushNotificationResponse_Headers">
    <wsdl:part name="ExceptionInfo" element="tns:ExceptionInfo" />
    <wsdl:part name="ExtraInfo" element="tns:ExtraInfo" />
    <wsdl:part name="Succeeded" element="tns:Succeeded" />
    <wsdl:part name="TimeZone" element="tns:TimeZone" />
  </wsdl:message>
  <wsdl:message name="RunAppointmentAlarmBrokerRequest">
    <wsdl:part name="parameters" element="tns:RunAppointmentAlarmBroker" />
  </wsdl:message>
  <wsdl:message name="RunAppointmentAlarmBrokerRequest_Headers">
    <wsdl:part name="ApplicationToken" element="tns:ApplicationToken" />
    <wsdl:part name="Credentials" element="tns:Credentials" />
    <wsdl:part name="TimeZone" element="tns:TimeZone" />
  </wsdl:message>
  <wsdl:message name="RunAppointmentAlarmBrokerResponse">
    <wsdl:part name="parameters" element="tns:RunAppointmentAlarmBrokerResponse" />
  </wsdl:message>
  <wsdl:message name="RunAppointmentAlarmBrokerResponse_Headers">
    <wsdl:part name="ExceptionInfo" element="tns:ExceptionInfo" />
    <wsdl:part name="ExtraInfo" element="tns:ExtraInfo" />
    <wsdl:part name="Succeeded" element="tns:Succeeded" />
    <wsdl:part name="TimeZone" element="tns:TimeZone" />
  </wsdl:message>
  <wsdl:message name="NotifyUsersRequest">
    <wsdl:part name="parameters" element="tns:NotifyUsers" />
  </wsdl:message>
  <wsdl:message name="NotifyUsersRequest_Headers">
    <wsdl:part name="ApplicationToken" element="tns:ApplicationToken" />
    <wsdl:part name="Credentials" element="tns:Credentials" />
    <wsdl:part name="TimeZone" element="tns:TimeZone" />
  </wsdl:message>
  <wsdl:message name="NotifyUsersResponse">
    <wsdl:part name="parameters" element="tns:NotifyUsersResponse" />
  </wsdl:message>
  <wsdl:message name="NotifyUsersResponse_Headers">
    <wsdl:part name="ExceptionInfo" element="tns:ExceptionInfo" />
    <wsdl:part name="ExtraInfo" element="tns:ExtraInfo" />
    <wsdl:part name="Succeeded" element="tns:Succeeded" />
    <wsdl:part name="TimeZone" element="tns:TimeZone" />
  </wsdl:message>
  <wsdl:message name="NotificationHandledRequest">
    <wsdl:part name="parameters" element="tns:NotificationHandled" />
  </wsdl:message>
  <wsdl:message name="NotificationHandledRequest_Headers">
    <wsdl:part name="ApplicationToken" element="tns:ApplicationToken" />
    <wsdl:part name="Credentials" element="tns:Credentials" />
    <wsdl:part name="TimeZone" element="tns:TimeZone" />
  </wsdl:message>
  <wsdl:message name="NotificationHandledResponse">
    <wsdl:part name="parameters" element="tns:NotificationHandledResponse" />
  </wsdl:message>
  <wsdl:message name="NotificationHandledResponse_Headers">
    <wsdl:part name="ExceptionInfo" element="tns:ExceptionInfo" />
    <wsdl:part name="ExtraInfo" element="tns:ExtraInfo" />
    <wsdl:part name="Succeeded" element="tns:Succeeded" />
    <wsdl:part name="TimeZone" element="tns:TimeZone" />
  </wsdl:message>
  <wsdl:message name="NotificationsHandledRequest">
    <wsdl:part name="parameters" element="tns:NotificationsHandled" />
  </wsdl:message>
  <wsdl:message name="NotificationsHandledRequest_Headers">
    <wsdl:part name="ApplicationToken" element="tns:ApplicationToken" />
    <wsdl:part name="Credentials" element="tns:Credentials" />
    <wsdl:part name="TimeZone" element="tns:TimeZone" />
  </wsdl:message>
  <wsdl:message name="NotificationsHandledResponse">
    <wsdl:part name="parameters" element="tns:NotificationsHandledResponse" />
  </wsdl:message>
  <wsdl:message name="NotificationsHandledResponse_Headers">
    <wsdl:part name="ExceptionInfo" element="tns:ExceptionInfo" />
    <wsdl:part name="ExtraInfo" element="tns:ExtraInfo" />
    <wsdl:part name="Succeeded" element="tns:Succeeded" />
    <wsdl:part name="TimeZone" element="tns:TimeZone" />
  </wsdl:message>
  <wsdl:portType name="Pocket">
    <wsdl:documentation>
      <summary>Declaration of Wcf web services for Pocket</summary>
    </wsdl:documentation>
    <wsdl:operation name="GetMyCallerIDs">
      <wsdl:documentation>
        <summary>Get caller ids that the current principal might be interested in (phone numbers of related persons in sales and appointments created/owned/touched by ourselves or colleagues in our primary group</summary>
      </wsdl:documentation>
      <wsdl:input wsaw:Action="http://www.superoffice.net/ws/crm/NetServer/Services88/Pocket/GetMyCallerIDs" name="GetMyCallerIDsRequest" message="tns:GetMyCallerIDsRequest" />
      <wsdl:output wsaw:Action="http://www.superoffice.net/ws/crm/NetServer/Services88/Pocket/GetMyCallerIDsResponse" name="GetMyCallerIDsResponse" message="tns:GetMyCallerIDsResponse" />
    </wsdl:operation>
    <wsdl:operation name="GetCallerIDsFromSelection">
      <wsdl:documentation>
        <summary>Get caller ids from a selection. Queries the shadow selection of persons and companies, so selections of any kind can be used</summary>
      </wsdl:documentation>
      <wsdl:input wsaw:Action="http://www.superoffice.net/ws/crm/NetServer/Services88/Pocket/GetCallerIDsFromSelection" name="GetCallerIDsFromSelectionRequest" message="tns:GetCallerIDsFromSelectionRequest" />
      <wsdl:output wsaw:Action="http://www.superoffice.net/ws/crm/NetServer/Services88/Pocket/GetCallerIDsFromSelectionResponse" name="GetCallerIDsFromSelectionResponse" message="tns:GetCallerIDsFromSelectionResponse" />
    </wsdl:operation>
    <wsdl:operation name="GetPocketStartupData">
      <wsdl:documentation>
        <summary>
        </summary>
      </wsdl:documentation>
      <wsdl:input wsaw:Action="http://www.superoffice.net/ws/crm/NetServer/Services88/Pocket/GetPocketStartupData" name="GetPocketStartupDataRequest" message="tns:GetPocketStartupDataRequest" />
      <wsdl:output wsaw:Action="http://www.superoffice.net/ws/crm/NetServer/Services88/Pocket/GetPocketStartupDataResponse" name="GetPocketStartupDataResponse" message="tns:GetPocketStartupDataResponse" />
    </wsdl:operation>
    <wsdl:operation name="RegisterDeviceForPushNotification">
      <wsdl:documentation>
        <summary>Register a device that should receive push notifications when notable events occour</summary>
      </wsdl:documentation>
      <wsdl:input wsaw:Action="http://www.superoffice.net/ws/crm/NetServer/Services88/Pocket/RegisterDeviceForPushNotification" name="RegisterDeviceForPushNotificationRequest" message="tns:RegisterDeviceForPushNotificationRequest" />
      <wsdl:output wsaw:Action="http://www.superoffice.net/ws/crm/NetServer/Services88/Pocket/RegisterDeviceForPushNotificationResponse" name="RegisterDeviceForPushNotificationResponse" message="tns:RegisterDeviceForPushNotificationResponse" />
    </wsdl:operation>
    <wsdl:operation name="GetRegisteredDevices">
      <wsdl:documentation>
        <summary>Retrieve all registered devices for an associate</summary>
      </wsdl:documentation>
      <wsdl:input wsaw:Action="http://www.superoffice.net/ws/crm/NetServer/Services88/Pocket/GetRegisteredDevices" name="GetRegisteredDevicesRequest" message="tns:GetRegisteredDevicesRequest" />
      <wsdl:output wsaw:Action="http://www.superoffice.net/ws/crm/NetServer/Services88/Pocket/GetRegisteredDevicesResponse" name="GetRegisteredDevicesResponse" message="tns:GetRegisteredDevicesResponse" />
    </wsdl:operation>
    <wsdl:operation name="SetPushNotificationTagsForDevice">
      <wsdl:documentation>
        <summary>Specify what kind of notification events a device should receive push notifications for</summary>
      </wsdl:documentation>
      <wsdl:input wsaw:Action="http://www.superoffice.net/ws/crm/NetServer/Services88/Pocket/SetPushNotificationTagsForDevice" name="SetPushNotificationTagsForDeviceRequest" message="tns:SetPushNotificationTagsForDeviceRequest" />
      <wsdl:output wsaw:Action="http://www.superoffice.net/ws/crm/NetServer/Services88/Pocket/SetPushNotificationTagsForDeviceResponse" name="SetPushNotificationTagsForDeviceResponse" message="tns:SetPushNotificationTagsForDeviceResponse" />
    </wsdl:operation>
    <wsdl:operation name="SetPushNotificationTagsForUser">
      <wsdl:documentation>
        <summary>Specify what kind of notification events a user should receive push notifications for.  This will update all registerred devices for this user.</summary>
      </wsdl:documentation>
      <wsdl:input wsaw:Action="http://www.superoffice.net/ws/crm/NetServer/Services88/Pocket/SetPushNotificationTagsForUser" name="SetPushNotificationTagsForUserRequest" message="tns:SetPushNotificationTagsForUserRequest" />
      <wsdl:output wsaw:Action="http://www.superoffice.net/ws/crm/NetServer/Services88/Pocket/SetPushNotificationTagsForUserResponse" name="SetPushNotificationTagsForUserResponse" message="tns:SetPushNotificationTagsForUserResponse" />
    </wsdl:operation>
    <wsdl:operation name="GetPushNotificationTagsForDevice">
      <wsdl:documentation>
        <summary>Retrieve current tag value for a device</summary>
      </wsdl:documentation>
      <wsdl:input wsaw:Action="http://www.superoffice.net/ws/crm/NetServer/Services88/Pocket/GetPushNotificationTagsForDevice" name="GetPushNotificationTagsForDeviceRequest" message="tns:GetPushNotificationTagsForDeviceRequest" />
      <wsdl:output wsaw:Action="http://www.superoffice.net/ws/crm/NetServer/Services88/Pocket/GetPushNotificationTagsForDeviceResponse" name="GetPushNotificationTagsForDeviceResponse" message="tns:GetPushNotificationTagsForDeviceResponse" />
    </wsdl:operation>
    <wsdl:operation name="SendPushNotification">
      <wsdl:documentation>
        <summary>Send a push notification to one or more associates</summary>
      </wsdl:documentation>
      <wsdl:input wsaw:Action="http://www.superoffice.net/ws/crm/NetServer/Services88/Pocket/SendPushNotification" name="SendPushNotificationRequest" message="tns:SendPushNotificationRequest" />
      <wsdl:output wsaw:Action="http://www.superoffice.net/ws/crm/NetServer/Services88/Pocket/SendPushNotificationResponse" name="SendPushNotificationResponse" message="tns:SendPushNotificationResponse" />
    </wsdl:operation>
    <wsdl:operation name="RunAppointmentAlarmBroker">
      <wsdl:documentation>
        <summary>Execute the AppointmentAlarmBroker once</summary>
      </wsdl:documentation>
      <wsdl:input wsaw:Action="http://www.superoffice.net/ws/crm/NetServer/Services88/Pocket/RunAppointmentAlarmBroker" name="RunAppointmentAlarmBrokerRequest" message="tns:RunAppointmentAlarmBrokerRequest" />
      <wsdl:output wsaw:Action="http://www.superoffice.net/ws/crm/NetServer/Services88/Pocket/RunAppointmentAlarmBrokerResponse" name="RunAppointmentAlarmBrokerResponse" message="tns:RunAppointmentAlarmBrokerResponse" />
    </wsdl:operation>
    <wsdl:operation name="NotifyUsers">
      <wsdl:documentation>
        <summary>Notify users about a new or changed entity</summary>
      </wsdl:documentation>
      <wsdl:input wsaw:Action="http://www.superoffice.net/ws/crm/NetServer/Services88/Pocket/NotifyUsers" name="NotifyUsersRequest" message="tns:NotifyUsersRequest" />
      <wsdl:output wsaw:Action="http://www.superoffice.net/ws/crm/NetServer/Services88/Pocket/NotifyUsersResponse" name="NotifyUsersResponse" message="tns:NotifyUsersResponse" />
    </wsdl:operation>
    <wsdl:operation name="NotificationHandled">
      <wsdl:documentation>
        <summary>Mark a notification as handled, so it can be cleaned up on other clients that have received the notification</summary>
      </wsdl:documentation>
      <wsdl:input wsaw:Action="http://www.superoffice.net/ws/crm/NetServer/Services88/Pocket/NotificationHandled" name="NotificationHandledRequest" message="tns:NotificationHandledRequest" />
      <wsdl:output wsaw:Action="http://www.superoffice.net/ws/crm/NetServer/Services88/Pocket/NotificationHandledResponse" name="NotificationHandledResponse" message="tns:NotificationHandledResponse" />
    </wsdl:operation>
    <wsdl:operation name="NotificationsHandled">
      <wsdl:documentation>
        <summary>Mark a set of notifications as handled, so they can be cleaned up on other clients that have received the notification</summary>
      </wsdl:documentation>
      <wsdl:input wsaw:Action="http://www.superoffice.net/ws/crm/NetServer/Services88/Pocket/NotificationsHandled" name="NotificationsHandledRequest" message="tns:NotificationsHandledRequest" />
      <wsdl:output wsaw:Action="http://www.superoffice.net/ws/crm/NetServer/Services88/Pocket/NotificationsHandledResponse" name="NotificationsHandledResponse" message="tns:NotificationsHandledResponse" />
    </wsdl:operation>
  </wsdl:portType>
  <wsdl:binding name="BasicHttpBinding_Pocket" type="tns:Pocket">
    <soap:binding transport="http://schemas.xmlsoap.org/soap/http" />
    <wsdl:operation name="GetMyCallerIDs">
      <soap:operation soapAction="http://www.superoffice.net/ws/crm/NetServer/Services88/Pocket/GetMyCallerIDs" style="document" />
      <wsdl:input name="GetMyCallerIDsRequest">
        <soap:header message="tns:GetMyCallerIDsRequest_Headers" part="ApplicationToken" use="literal" />
        <soap:header message="tns:GetMyCallerIDsRequest_Headers" part="Credentials" use="literal" />
        <soap:header message="tns:GetMyCallerIDsRequest_Headers" part="TimeZone" use="literal" />
        <soap:body use="literal" />
      </wsdl:input>
      <wsdl:output name="GetMyCallerIDsResponse">
        <soap:header message="tns:GetMyCallerIDsResponse_Headers" part="ExceptionInfo" use="literal" />
        <soap:header message="tns:GetMyCallerIDsResponse_Headers" part="ExtraInfo" use="literal" />
        <soap:header message="tns:GetMyCallerIDsResponse_Headers" part="Succeeded" use="literal" />
        <soap:header message="tns:GetMyCallerIDsResponse_Headers" part="TimeZone" use="literal" />
        <soap:body use="literal" />
      </wsdl:output>
    </wsdl:operation>
    <wsdl:operation name="GetCallerIDsFromSelection">
      <soap:operation soapAction="http://www.superoffice.net/ws/crm/NetServer/Services88/Pocket/GetCallerIDsFromSelection" style="document" />
      <wsdl:input name="GetCallerIDsFromSelectionRequest">
        <soap:header message="tns:GetCallerIDsFromSelectionRequest_Headers" part="ApplicationToken" use="literal" />
        <soap:header message="tns:GetCallerIDsFromSelectionRequest_Headers" part="Credentials" use="literal" />
        <soap:header message="tns:GetCallerIDsFromSelectionRequest_Headers" part="TimeZone" use="literal" />
        <soap:body use="literal" />
      </wsdl:input>
      <wsdl:output name="GetCallerIDsFromSelectionResponse">
        <soap:header message="tns:GetCallerIDsFromSelectionResponse_Headers" part="ExceptionInfo" use="literal" />
        <soap:header message="tns:GetCallerIDsFromSelectionResponse_Headers" part="ExtraInfo" use="literal" />
        <soap:header message="tns:GetCallerIDsFromSelectionResponse_Headers" part="Succeeded" use="literal" />
        <soap:header message="tns:GetCallerIDsFromSelectionResponse_Headers" part="TimeZone" use="literal" />
        <soap:body use="literal" />
      </wsdl:output>
    </wsdl:operation>
    <wsdl:operation name="GetPocketStartupData">
      <soap:operation soapAction="http://www.superoffice.net/ws/crm/NetServer/Services88/Pocket/GetPocketStartupData" style="document" />
      <wsdl:input name="GetPocketStartupDataRequest">
        <soap:header message="tns:GetPocketStartupDataRequest_Headers" part="ApplicationToken" use="literal" />
        <soap:header message="tns:GetPocketStartupDataRequest_Headers" part="Credentials" use="literal" />
        <soap:header message="tns:GetPocketStartupDataRequest_Headers" part="TimeZone" use="literal" />
        <soap:body use="literal" />
      </wsdl:input>
      <wsdl:output name="GetPocketStartupDataResponse">
        <soap:header message="tns:GetPocketStartupDataResponse_Headers" part="ExceptionInfo" use="literal" />
        <soap:header message="tns:GetPocketStartupDataResponse_Headers" part="ExtraInfo" use="literal" />
        <soap:header message="tns:GetPocketStartupDataResponse_Headers" part="Succeeded" use="literal" />
        <soap:header message="tns:GetPocketStartupDataResponse_Headers" part="TimeZone" use="literal" />
        <soap:body use="literal" />
      </wsdl:output>
    </wsdl:operation>
    <wsdl:operation name="RegisterDeviceForPushNotification">
      <soap:operation soapAction="http://www.superoffice.net/ws/crm/NetServer/Services88/Pocket/RegisterDeviceForPushNotification" style="document" />
      <wsdl:input name="RegisterDeviceForPushNotificationRequest">
        <soap:header message="tns:RegisterDeviceForPushNotificationRequest_Headers" part="ApplicationToken" use="literal" />
        <soap:header message="tns:RegisterDeviceForPushNotificationRequest_Headers" part="Credentials" use="literal" />
        <soap:header message="tns:RegisterDeviceForPushNotificationRequest_Headers" part="TimeZone" use="literal" />
        <soap:body use="literal" />
      </wsdl:input>
      <wsdl:output name="RegisterDeviceForPushNotificationResponse">
        <soap:header message="tns:RegisterDeviceForPushNotificationResponse_Headers" part="ExceptionInfo" use="literal" />
        <soap:header message="tns:RegisterDeviceForPushNotificationResponse_Headers" part="ExtraInfo" use="literal" />
        <soap:header message="tns:RegisterDeviceForPushNotificationResponse_Headers" part="Succeeded" use="literal" />
        <soap:header message="tns:RegisterDeviceForPushNotificationResponse_Headers" part="TimeZone" use="literal" />
        <soap:body use="literal" />
      </wsdl:output>
    </wsdl:operation>
    <wsdl:operation name="GetRegisteredDevices">
      <soap:operation soapAction="http://www.superoffice.net/ws/crm/NetServer/Services88/Pocket/GetRegisteredDevices" style="document" />
      <wsdl:input name="GetRegisteredDevicesRequest">
        <soap:header message="tns:GetRegisteredDevicesRequest_Headers" part="ApplicationToken" use="literal" />
        <soap:header message="tns:GetRegisteredDevicesRequest_Headers" part="Credentials" use="literal" />
        <soap:header message="tns:GetRegisteredDevicesRequest_Headers" part="TimeZone" use="literal" />
        <soap:body use="literal" />
      </wsdl:input>
      <wsdl:output name="GetRegisteredDevicesResponse">
        <soap:header message="tns:GetRegisteredDevicesResponse_Headers" part="ExceptionInfo" use="literal" />
        <soap:header message="tns:GetRegisteredDevicesResponse_Headers" part="ExtraInfo" use="literal" />
        <soap:header message="tns:GetRegisteredDevicesResponse_Headers" part="Succeeded" use="literal" />
        <soap:header message="tns:GetRegisteredDevicesResponse_Headers" part="TimeZone" use="literal" />
        <soap:body use="literal" />
      </wsdl:output>
    </wsdl:operation>
    <wsdl:operation name="SetPushNotificationTagsForDevice">
      <soap:operation soapAction="http://www.superoffice.net/ws/crm/NetServer/Services88/Pocket/SetPushNotificationTagsForDevice" style="document" />
      <wsdl:input name="SetPushNotificationTagsForDeviceRequest">
        <soap:header message="tns:SetPushNotificationTagsForDeviceRequest_Headers" part="ApplicationToken" use="literal" />
        <soap:header message="tns:SetPushNotificationTagsForDeviceRequest_Headers" part="Credentials" use="literal" />
        <soap:header message="tns:SetPushNotificationTagsForDeviceRequest_Headers" part="TimeZone" use="literal" />
        <soap:body use="literal" />
      </wsdl:input>
      <wsdl:output name="SetPushNotificationTagsForDeviceResponse">
        <soap:header message="tns:SetPushNotificationTagsForDeviceResponse_Headers" part="ExceptionInfo" use="literal" />
        <soap:header message="tns:SetPushNotificationTagsForDeviceResponse_Headers" part="ExtraInfo" use="literal" />
        <soap:header message="tns:SetPushNotificationTagsForDeviceResponse_Headers" part="Succeeded" use="literal" />
        <soap:header message="tns:SetPushNotificationTagsForDeviceResponse_Headers" part="TimeZone" use="literal" />
        <soap:body use="literal" />
      </wsdl:output>
    </wsdl:operation>
    <wsdl:operation name="SetPushNotificationTagsForUser">
      <soap:operation soapAction="http://www.superoffice.net/ws/crm/NetServer/Services88/Pocket/SetPushNotificationTagsForUser" style="document" />
      <wsdl:input name="SetPushNotificationTagsForUserRequest">
        <soap:header message="tns:SetPushNotificationTagsForUserRequest_Headers" part="ApplicationToken" use="literal" />
        <soap:header message="tns:SetPushNotificationTagsForUserRequest_Headers" part="Credentials" use="literal" />
        <soap:header message="tns:SetPushNotificationTagsForUserRequest_Headers" part="TimeZone" use="literal" />
        <soap:body use="literal" />
      </wsdl:input>
      <wsdl:output name="SetPushNotificationTagsForUserResponse">
        <soap:header message="tns:SetPushNotificationTagsForUserResponse_Headers" part="ExceptionInfo" use="literal" />
        <soap:header message="tns:SetPushNotificationTagsForUserResponse_Headers" part="ExtraInfo" use="literal" />
        <soap:header message="tns:SetPushNotificationTagsForUserResponse_Headers" part="Succeeded" use="literal" />
        <soap:header message="tns:SetPushNotificationTagsForUserResponse_Headers" part="TimeZone" use="literal" />
        <soap:body use="literal" />
      </wsdl:output>
    </wsdl:operation>
    <wsdl:operation name="GetPushNotificationTagsForDevice">
      <soap:operation soapAction="http://www.superoffice.net/ws/crm/NetServer/Services88/Pocket/GetPushNotificationTagsForDevice" style="document" />
      <wsdl:input name="GetPushNotificationTagsForDeviceRequest">
        <soap:header message="tns:GetPushNotificationTagsForDeviceRequest_Headers" part="ApplicationToken" use="literal" />
        <soap:header message="tns:GetPushNotificationTagsForDeviceRequest_Headers" part="Credentials" use="literal" />
        <soap:header message="tns:GetPushNotificationTagsForDeviceRequest_Headers" part="TimeZone" use="literal" />
        <soap:body use="literal" />
      </wsdl:input>
      <wsdl:output name="GetPushNotificationTagsForDeviceResponse">
        <soap:header message="tns:GetPushNotificationTagsForDeviceResponse_Headers" part="ExceptionInfo" use="literal" />
        <soap:header message="tns:GetPushNotificationTagsForDeviceResponse_Headers" part="ExtraInfo" use="literal" />
        <soap:header message="tns:GetPushNotificationTagsForDeviceResponse_Headers" part="Succeeded" use="literal" />
        <soap:header message="tns:GetPushNotificationTagsForDeviceResponse_Headers" part="TimeZone" use="literal" />
        <soap:body use="literal" />
      </wsdl:output>
    </wsdl:operation>
    <wsdl:operation name="SendPushNotification">
      <soap:operation soapAction="http://www.superoffice.net/ws/crm/NetServer/Services88/Pocket/SendPushNotification" style="document" />
      <wsdl:input name="SendPushNotificationRequest">
        <soap:header message="tns:SendPushNotificationRequest_Headers" part="ApplicationToken" use="literal" />
        <soap:header message="tns:SendPushNotificationRequest_Headers" part="Credentials" use="literal" />
        <soap:header message="tns:SendPushNotificationRequest_Headers" part="TimeZone" use="literal" />
        <soap:body use="literal" />
      </wsdl:input>
      <wsdl:output name="SendPushNotificationResponse">
        <soap:header message="tns:SendPushNotificationResponse_Headers" part="ExceptionInfo" use="literal" />
        <soap:header message="tns:SendPushNotificationResponse_Headers" part="ExtraInfo" use="literal" />
        <soap:header message="tns:SendPushNotificationResponse_Headers" part="Succeeded" use="literal" />
        <soap:header message="tns:SendPushNotificationResponse_Headers" part="TimeZone" use="literal" />
        <soap:body use="literal" />
      </wsdl:output>
    </wsdl:operation>
    <wsdl:operation name="RunAppointmentAlarmBroker">
      <soap:operation soapAction="http://www.superoffice.net/ws/crm/NetServer/Services88/Pocket/RunAppointmentAlarmBroker" style="document" />
      <wsdl:input name="RunAppointmentAlarmBrokerRequest">
        <soap:header message="tns:RunAppointmentAlarmBrokerRequest_Headers" part="ApplicationToken" use="literal" />
        <soap:header message="tns:RunAppointmentAlarmBrokerRequest_Headers" part="Credentials" use="literal" />
        <soap:header message="tns:RunAppointmentAlarmBrokerRequest_Headers" part="TimeZone" use="literal" />
        <soap:body use="literal" />
      </wsdl:input>
      <wsdl:output name="RunAppointmentAlarmBrokerResponse">
        <soap:header message="tns:RunAppointmentAlarmBrokerResponse_Headers" part="ExceptionInfo" use="literal" />
        <soap:header message="tns:RunAppointmentAlarmBrokerResponse_Headers" part="ExtraInfo" use="literal" />
        <soap:header message="tns:RunAppointmentAlarmBrokerResponse_Headers" part="Succeeded" use="literal" />
        <soap:header message="tns:RunAppointmentAlarmBrokerResponse_Headers" part="TimeZone" use="literal" />
        <soap:body use="literal" />
      </wsdl:output>
    </wsdl:operation>
    <wsdl:operation name="NotifyUsers">
      <soap:operation soapAction="http://www.superoffice.net/ws/crm/NetServer/Services88/Pocket/NotifyUsers" style="document" />
      <wsdl:input name="NotifyUsersRequest">
        <soap:header message="tns:NotifyUsersRequest_Headers" part="ApplicationToken" use="literal" />
        <soap:header message="tns:NotifyUsersRequest_Headers" part="Credentials" use="literal" />
        <soap:header message="tns:NotifyUsersRequest_Headers" part="TimeZone" use="literal" />
        <soap:body use="literal" />
      </wsdl:input>
      <wsdl:output name="NotifyUsersResponse">
        <soap:header message="tns:NotifyUsersResponse_Headers" part="ExceptionInfo" use="literal" />
        <soap:header message="tns:NotifyUsersResponse_Headers" part="ExtraInfo" use="literal" />
        <soap:header message="tns:NotifyUsersResponse_Headers" part="Succeeded" use="literal" />
        <soap:header message="tns:NotifyUsersResponse_Headers" part="TimeZone" use="literal" />
        <soap:body use="literal" />
      </wsdl:output>
    </wsdl:operation>
    <wsdl:operation name="NotificationHandled">
      <soap:operation soapAction="http://www.superoffice.net/ws/crm/NetServer/Services88/Pocket/NotificationHandled" style="document" />
      <wsdl:input name="NotificationHandledRequest">
        <soap:header message="tns:NotificationHandledRequest_Headers" part="ApplicationToken" use="literal" />
        <soap:header message="tns:NotificationHandledRequest_Headers" part="Credentials" use="literal" />
        <soap:header message="tns:NotificationHandledRequest_Headers" part="TimeZone" use="literal" />
        <soap:body use="literal" />
      </wsdl:input>
      <wsdl:output name="NotificationHandledResponse">
        <soap:header message="tns:NotificationHandledResponse_Headers" part="ExceptionInfo" use="literal" />
        <soap:header message="tns:NotificationHandledResponse_Headers" part="ExtraInfo" use="literal" />
        <soap:header message="tns:NotificationHandledResponse_Headers" part="Succeeded" use="literal" />
        <soap:header message="tns:NotificationHandledResponse_Headers" part="TimeZone" use="literal" />
        <soap:body use="literal" />
      </wsdl:output>
    </wsdl:operation>
    <wsdl:operation name="NotificationsHandled">
      <soap:operation soapAction="http://www.superoffice.net/ws/crm/NetServer/Services88/Pocket/NotificationsHandled" style="document" />
      <wsdl:input name="NotificationsHandledRequest">
        <soap:header message="tns:NotificationsHandledRequest_Headers" part="ApplicationToken" use="literal" />
        <soap:header message="tns:NotificationsHandledRequest_Headers" part="Credentials" use="literal" />
        <soap:header message="tns:NotificationsHandledRequest_Headers" part="TimeZone" use="literal" />
        <soap:body use="literal" />
      </wsdl:input>
      <wsdl:output name="NotificationsHandledResponse">
        <soap:header message="tns:NotificationsHandledResponse_Headers" part="ExceptionInfo" use="literal" />
        <soap:header message="tns:NotificationsHandledResponse_Headers" part="ExtraInfo" use="literal" />
        <soap:header message="tns:NotificationsHandledResponse_Headers" part="Succeeded" use="literal" />
        <soap:header message="tns:NotificationsHandledResponse_Headers" part="TimeZone" use="literal" />
        <soap:body use="literal" />
      </wsdl:output>
    </wsdl:operation>
  </wsdl:binding>
  <wsdl:service name="WcfPocketService">
    <wsdl:port name="BasicHttpBinding_Pocket" binding="tns:BasicHttpBinding_Pocket">
      <soap:address location="https://sod.superoffice.com/Cust12345/Remote/Services88/Pocket.svc" />
    </wsdl:port>
  </wsdl:service>
</wsdl:definitions>
```
