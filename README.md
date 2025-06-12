From Hotel-legal-Processer Kafka service project create analyze postKafka-PROPERTY_CHANGES_ALL NEW proprty test step and create test cases for TERMINATED proprty,INACTIVE property,test property

<?xml version="1.0" encoding="UTF-8"?>
<con:soapui-project id="5fbe961b-b02d-444c-87b8-72d1c84e70ed" created="3.52.0" activeEnvironment="Default environment" encryptionMode="Not encrypted" name="Hotel-legal-Processer Kafka service" projectVersion="" updated="3.52.0 2024-04-16T11:49:17Z" xmlns:con="http://eviware.com/soapui/config">
  <con:settings/>
  <con:interface xsi:type="con:RestService" id="2ccafb53-39e3-4b2a-8ff8-54ce87cb7789" name="testDataAPI" type="rest_ex" wadlVersion="https://swagger.io/openapiv3/specification" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
    <con:settings id="53d1d0d0-825b-49ca-ac11-1def451b6fb5"/>
    <con:definitionCache type="TEXT" rootPart="testDataAPI.json">
      <con:part>
        <con:url>testDataAPI.json</con:url>
        <con:content>{"openapi":"3.0.1","info":{"title":"testDataAPI","description":"","version":"1.0.0"},"servers":[{"url":"/"}],"paths":{"/api/kafka/topic/{topicName}/message":{"description":"","get":{"description":"","responses":{"default":{"description":"Default response"}}},"parameters":[{"name":"topicName","in":"path","required":true,"style":"simple","explode":false}]}}}</con:content>
        <con:type>https://swagger.io/openapiv3/specification</con:type>
      </con:part>
    </con:definitionCache>
    <con:endpoints>
      <con:endpoint>http://testdataapi-testops-chi-qa.sharedev.cloud.chotel.com</con:endpoint>
    </con:endpoints>
    <con:resource name="POST" path="api/kafka/topic/{topicName}/message" id="3e3ca903-0af8-4161-9a45-e58c015e00d6">
      <con:settings/>
      <con:parameters>
        <con:parameter required="true">
          <con:name>topicName</con:name>
          <con:value>topicName</con:value>
          <con:style>TEMPLATE</con:style>
          <con:default>topicName</con:default>
        </con:parameter>
      </con:parameters>
      <con:method name="Method 1" id="420e54a3-d547-437d-8c13-b29d07e3705f" method="POST">
        <con:settings/>
        <con:parameters/>
        <con:request name="Request 1" id="c9326f50-56e3-408e-8df8-bdcaa3767896" mediaType="application/json" postQueryString="false">
          <con:settings>
            <con:setting id="com.eviware.soapui.impl.wsdl.WsdlRequest@request-headers">&lt;xml-fragment/></con:setting>
          </con:settings>
          <con:endpoint>http://testdataapi-testops-chi-qa.sharedev.cloud.chotel.com</con:endpoint>
          <con:request/>
          <con:originalUri>http://testdataapi-testops-chi-qa.sharedev.cloud.chotel.com/api/kafka/topic/topicName/message</con:originalUri>
          <con:credentials>
            <con:selectedAuthProfile>No Authorization</con:selectedAuthProfile>
            <con:authType>No Authorization</con:authType>
          </con:credentials>
          <con:jmsConfig JMSDeliveryMode="PERSISTENT"/>
          <con:parameters/>
        </con:request>
      </con:method>
    </con:resource>
    <con:resource name="GET" path="api/kafka/topic/{topicName}/message" id="aa516d1b-789c-4816-a07b-0d43fda2d83b">
      <con:settings/>
      <con:parameters>
        <con:parameter required="true">
          <con:name>topicName</con:name>
          <con:value>topicName</con:value>
          <con:style>TEMPLATE</con:style>
          <con:default>topicName</con:default>
        </con:parameter>
        <con:parameter required="true">
          <con:name>brokerUrl</con:name>
          <con:value/>
          <con:style>QUERY</con:style>
          <con:default/>
        </con:parameter>
        <con:parameter required="true">
          <con:name>trackingId</con:name>
          <con:value/>
          <con:style>QUERY</con:style>
          <con:default/>
        </con:parameter>
        <con:parameter required="true">
          <con:name>timeout</con:name>
          <con:value/>
          <con:style>QUERY</con:style>
          <con:default/>
        </con:parameter>
      </con:parameters>
      <con:method name="Method 1" id="d81863cd-e22b-4961-8052-e04d5765f5d7" method="GET">
        <con:settings/>
        <con:parameters/>
        <con:request name="Request 1" id="80abbdd4-5e47-4bef-8552-faa3be943a04" mediaType="application/json">
          <con:settings/>
          <con:endpoint>http://testdataapi-testops-chi-qa.sharedev.cloud.chotel.com</con:endpoint>
          <con:request/>
          <con:credentials>
            <con:selectedAuthProfile>No Authorization</con:selectedAuthProfile>
            <con:authType>No Authorization</con:authType>
          </con:credentials>
          <con:jmsConfig JMSDeliveryMode="PERSISTENT"/>
          <con:parameters/>
        </con:request>
      </con:method>
    </con:resource>
  </con:interface>
  <con:interface xsi:type="con:WsdlInterface" id="89107fb4-48d3-4c93-84c2-3cd6f1b7ff38" wsaVersion="NONE" name="HotelDistributionSoapBinding" type="wsdl" bindingName="{http://www.choicehotels.com/service/dist/HotelDistribution/v6}HotelDistributionSoapBinding" soapVersion="1_1" anonymous="optional" definition="http://esb.services.ext.pci.qa.chotel.com/HotelDistributionService/v6?WSDL" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
    <con:settings id="3a45a93d-e32b-4456-87d6-1183a5c34b94">
      <con:setting id="a7f043e7-5c2c-45c0-92f8-3a572ca95e3ffileName">HotelDistributionSoapBinding</con:setting>
    </con:settings>
    <con:definitionCache type="TEXT" rootPart="http://esb.services.ext.pci.qa.chotel.com/HotelDistributionService/v6?WSDL">
      <con:part>
        <con:url>http://esb.services.ext.pci.qa.chotel.com/HotelDistributionService/v6?WSDL</con:url>
        <con:content><![CDATA[<WL5G3N0:definitions targetNamespace="http://www.choicehotels.com/service/dist/HotelDistribution/v6" xmlns:WL5G3N0="http://schemas.xmlsoap.org/wsdl/" xmlns:WL5G3N1="http://www.choicehotels.com/schema/v6/common/msg" xmlns:WL5G3N2="http://www.choicehotels.com/schema/v6/dist/msg" xmlns:WL5G3N3="http://www.choicehotels.com/service/dist/HotelDistribution/v6" xmlns:WL5G3N4="http://schemas.xmlsoap.org/wsdl/soap/">
  <WL5G3N0:types>
    <xsd:schema xmlns:cmg="http://www.choicehotels.com/schema/v6/common/msg" xmlns:dst="http://www.choicehotels.com/service/dist/HotelDistribution/v6" xmlns:msg="http://www.choicehotels.com/schema/v6/dist/msg" xmlns:soap="http://schemas.xmlsoap.org/wsdl/soap/" xmlns:wsdl="http://schemas.xmlsoap.org/wsdl/" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <xsd:import namespace="http://www.choicehotels.com/schema/v6/dist/msg" schemaLocation="http://esb.services.ext.pci.qa.chotel.com:80/HotelDistributionService/v6?SCHEMA%2FCdm_Shared_v6%2Fxsd%2Fdistribution%2FHotelDistributionMessages"/>
      <xsd:import namespace="http://www.choicehotels.com/schema/v6/common/msg" schemaLocation="http://esb.services.ext.pci.qa.chotel.com:80/HotelDistributionService/v6?SCHEMA%2FCdm_Shared_v6%2Fxsd%2Fcommon%2FCommonMessages"/>
    </xsd:schema>
  </WL5G3N0:types>
  <WL5G3N0:message name="DescribeRequestMessage">
    <WL5G3N0:part element="WL5G3N1:describe" name="parameters"/>
  </WL5G3N0:message>
  <WL5G3N0:message name="DescribeResponseMessage">
    <WL5G3N0:part element="WL5G3N1:describeResponse" name="parameters"/>
  </WL5G3N0:message>
  <WL5G3N0:message name="GetHotelRequestMessage">
    <WL5G3N0:part element="WL5G3N2:getHotel" name="parameters"/>
  </WL5G3N0:message>
  <WL5G3N0:message name="GetHotelResponseMessage">
    <WL5G3N0:part element="WL5G3N2:getHotelResponse" name="parameters"/>
  </WL5G3N0:message>
  <WL5G3N0:message name="GetHotelSummaryRequestMessage">
    <WL5G3N0:part element="WL5G3N2:getHotelSummary" name="parameters"/>
  </WL5G3N0:message>
  <WL5G3N0:message name="GetHotelSummaryResponseMessage">
    <WL5G3N0:part element="WL5G3N2:getHotelSummaryResponse" name="parameters"/>
  </WL5G3N0:message>
  <WL5G3N0:message name="SearchHotelRequestMessage">
    <WL5G3N0:part element="WL5G3N2:searchHotel" name="parameters"/>
  </WL5G3N0:message>
  <WL5G3N0:message name="SearchHotelResponseMessage">
    <WL5G3N0:part element="WL5G3N2:searchHotelResponse" name="parameters"/>
  </WL5G3N0:message>
  <WL5G3N0:message name="HotelDistributionBusinessFault">
    <WL5G3N0:part element="WL5G3N2:hotelDistributionBusinessFault" name="fault"/>
  </WL5G3N0:message>
  <WL5G3N0:message name="HotelDistributionTechnicalFault">
    <WL5G3N0:part element="WL5G3N2:hotelDistributionTechnicalFault" name="fault"/>
  </WL5G3N0:message>
  <WL5G3N0:portType name="HotelDistribution">
    <WL5G3N0:operation name="describe">
      <WL5G3N0:input message="WL5G3N3:DescribeRequestMessage"/>
      <WL5G3N0:output message="WL5G3N3:DescribeResponseMessage"/>
      <WL5G3N0:fault message="WL5G3N3:HotelDistributionBusinessFault" name="businessFault"/>
      <WL5G3N0:fault message="WL5G3N3:HotelDistributionTechnicalFault" name="technicalFault"/>
    </WL5G3N0:operation>
    <WL5G3N0:operation name="getHotel">
      <WL5G3N0:input message="WL5G3N3:GetHotelRequestMessage"/>
      <WL5G3N0:output message="WL5G3N3:GetHotelResponseMessage"/>
      <WL5G3N0:fault message="WL5G3N3:HotelDistributionBusinessFault" name="businessFault"/>
      <WL5G3N0:fault message="WL5G3N3:HotelDistributionTechnicalFault" name="technicalFault"/>
    </WL5G3N0:operation>
    <WL5G3N0:operation name="getHotelSummary">
      <WL5G3N0:input message="WL5G3N3:GetHotelSummaryRequestMessage"/>
      <WL5G3N0:output message="WL5G3N3:GetHotelSummaryResponseMessage"/>
      <WL5G3N0:fault message="WL5G3N3:HotelDistributionBusinessFault" name="businessFault"/>
      <WL5G3N0:fault message="WL5G3N3:HotelDistributionTechnicalFault" name="technicalFault"/>
    </WL5G3N0:operation>
    <WL5G3N0:operation name="searchHotel">
      <WL5G3N0:input message="WL5G3N3:SearchHotelRequestMessage"/>
      <WL5G3N0:output message="WL5G3N3:SearchHotelResponseMessage"/>
      <WL5G3N0:fault message="WL5G3N3:HotelDistributionBusinessFault" name="businessFault"/>
      <WL5G3N0:fault message="WL5G3N3:HotelDistributionTechnicalFault" name="technicalFault"/>
    </WL5G3N0:operation>
  </WL5G3N0:portType>
  <WL5G3N0:binding name="HotelDistributionSoapBinding" type="WL5G3N3:HotelDistribution">
    <WL5G3N4:binding style="document" transport="http://schemas.xmlsoap.org/soap/http"/>
    <WL5G3N0:operation name="describe">
      <WL5G3N4:operation soapAction="describe"/>
      <WL5G3N0:input>
        <WL5G3N4:body use="literal"/>
      </WL5G3N0:input>
      <WL5G3N0:output>
        <WL5G3N4:body use="literal"/>
      </WL5G3N0:output>
      <WL5G3N0:fault name="businessFault">
        <WL5G3N4:fault name="businessFault" use="literal"/>
      </WL5G3N0:fault>
      <WL5G3N0:fault name="technicalFault">
        <WL5G3N4:fault name="technicalFault" use="literal"/>
      </WL5G3N0:fault>
    </WL5G3N0:operation>
    <WL5G3N0:operation name="getHotel">
      <WL5G3N4:operation soapAction="getHotel"/>
      <WL5G3N0:input>
        <WL5G3N4:body use="literal"/>
      </WL5G3N0:input>
      <WL5G3N0:output>
        <WL5G3N4:body use="literal"/>
      </WL5G3N0:output>
      <WL5G3N0:fault name="businessFault">
        <WL5G3N4:fault name="businessFault" use="literal"/>
      </WL5G3N0:fault>
      <WL5G3N0:fault name="technicalFault">
        <WL5G3N4:fault name="technicalFault" use="literal"/>
      </WL5G3N0:fault>
    </WL5G3N0:operation>
    <WL5G3N0:operation name="getHotelSummary">
      <WL5G3N4:operation soapAction="getHotelSummary"/>
      <WL5G3N0:input>
        <WL5G3N4:body use="literal"/>
      </WL5G3N0:input>
      <WL5G3N0:output>
        <WL5G3N4:body use="literal"/>
      </WL5G3N0:output>
      <WL5G3N0:fault name="businessFault">
        <WL5G3N4:fault name="businessFault" use="literal"/>
      </WL5G3N0:fault>
      <WL5G3N0:fault name="technicalFault">
        <WL5G3N4:fault name="technicalFault" use="literal"/>
      </WL5G3N0:fault>
    </WL5G3N0:operation>
    <WL5G3N0:operation name="searchHotel">
      <WL5G3N4:operation soapAction="searchHotel"/>
      <WL5G3N0:input>
        <WL5G3N4:body use="literal"/>
      </WL5G3N0:input>
      <WL5G3N0:output>
        <WL5G3N4:body use="literal"/>
      </WL5G3N0:output>
      <WL5G3N0:fault name="businessFault">
        <WL5G3N4:fault name="businessFault" use="literal"/>
      </WL5G3N0:fault>
      <WL5G3N0:fault name="technicalFault">
        <WL5G3N4:fault name="technicalFault" use="literal"/>
      </WL5G3N0:fault>
    </WL5G3N0:operation>
  </WL5G3N0:binding>
  <WL5G3N0:service name="HotelDistributionService">
    <WL5G3N0:documentation>OSB Service</WL5G3N0:documentation>
    <WL5G3N0:port binding="WL5G3N3:HotelDistributionSoapBinding" name="HotelDistribution">
      <WL5G3N4:address location="http://esb.services.ext.pci.qa.chotel.com:80/HotelDistributionService/v6"/>
    </WL5G3N0:port>
  </WL5G3N0:service>
</WL5G3N0:definitions>]]></con:content>
        <con:type>http://schemas.xmlsoap.org/wsdl/</con:type>
      </con:part>
      <con:part>
        <con:url>http://esb.services.ext.pci.qa.chotel.com:80/HotelDistributionService/v6?SCHEMA%2FCdm_Shared_v6%2Fxsd%2Fdistribution%2FHotelDistributionMessages</con:url>
        <con:content><![CDATA[<!--Document: HotelDistributionMessages schema contains message types
          used by the HotelDistribution service.

Date: 04-13-2011
Last Updated: 10-19-2012
Authors: Chris Judson, Charlie Taylor-->
<xsd:schema targetNamespace="http://www.choicehotels.com/schema/v6/dist/msg" elementFormDefault="qualified" attributeFormDefault="unqualified" xml:lang="en" xmlns:msg="http://www.choicehotels.com/schema/v6/dist/msg" xmlns:cmg="http://www.choicehotels.com/schema/v6/common/msg" xmlns:dst="http://www.choicehotels.com/schema/v6/dist/cdm" xmlns:cmn="http://www.choicehotels.com/schema/v6/common/cdm" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <xsd:import namespace="http://www.choicehotels.com/schema/v6/common/cdm" schemaLocation="http://esb.services.ext.pci.qa.chotel.com:80/HotelDistributionService/v6?SCHEMA%2FCdm_Shared_v6%2Fxsd%2Fcommon%2FCommonTypes"/>
  <xsd:import namespace="http://www.choicehotels.com/schema/v6/common/cdm" schemaLocation="http://esb.services.ext.pci.qa.chotel.com:80/HotelDistributionService/v6?SCHEMA%2FCdm_Shared_v6%2Fxsd%2Fcommon%2FFaultTypes"/>
  <xsd:import namespace="http://www.choicehotels.com/schema/v6/dist/cdm" schemaLocation="http://esb.services.ext.pci.qa.chotel.com:80/HotelDistributionService/v6?SCHEMA%2FCdm_Shared_v6%2Fxsd%2Fdistribution%2FHotelDistribution"/>
  <xsd:element name="getHotel" type="msg:GetHotelRequestType"/>
  <xsd:element name="getHotelResponse" type="msg:GetHotelResponseType"/>
  <xsd:element name="getHotelSummary" type="msg:GetHotelSummaryRequestType"/>
  <xsd:element name="getHotelSummaryResponse" type="msg:GetHotelSummaryResponseType"/>
  <xsd:element name="hotelDistributionBusinessFault" type="msg:HotelDistributionBusinessFaultType"/>
  <xsd:element name="hotelDistributionTechnicalFault" type="msg:HotelDistributionTechnicalFaultType"/>
  <xsd:element name="searchHotel" type="msg:SearchHotelRequestType"/>
  <xsd:element name="searchHotelResponse" type="msg:SearchHotelResponseType"/>
  <xsd:complexType name="GetHotelRequestType">
    <xsd:sequence>
      <xsd:element name="request" type="msg:GetHotelRequestMessageType"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="GetHotelRequestMessageType">
    <xsd:sequence>
      <xsd:element ref="cmn:requestMessageHeader" minOccurs="1" maxOccurs="1"/>
      <xsd:element ref="cmn:hotelId" minOccurs="1" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="GetHotelResponseType">
    <xsd:sequence>
      <xsd:element name="response" type="msg:GetHotelResponseMessageType"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="GetHotelResponseMessageType">
    <xsd:sequence>
      <xsd:element ref="cmn:responseMessageHeader" minOccurs="1" maxOccurs="1"/>
      <xsd:element ref="dst:hotelDistribution" minOccurs="0" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="GetHotelSummaryRequestType">
    <xsd:sequence>
      <xsd:element name="request" type="msg:GetHotelSummaryRequestMessageType"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="GetHotelSummaryRequestMessageType">
    <xsd:sequence>
      <xsd:element ref="cmn:requestMessageHeader" minOccurs="1" maxOccurs="1"/>
      <xsd:element ref="cmn:hotelId"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="GetHotelSummaryResponseType">
    <xsd:sequence>
      <xsd:element name="response" type="msg:GetHotelSummaryResponseMessageType"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="GetHotelSummaryResponseMessageType">
    <xsd:sequence>
      <xsd:element ref="cmn:responseMessageHeader" minOccurs="1" maxOccurs="1"/>
      <xsd:element ref="dst:hotelDistributionSummary" minOccurs="0" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="HotelDistributionBusinessFaultType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Response message for hotel distribution
                                    errors</xsd:documentation>
    </xsd:annotation>
    <xsd:complexContent>
      <xsd:extension base="cmn:BusinessFaultType"/>
    </xsd:complexContent>
  </xsd:complexType>
  <xsd:complexType name="HotelDistributionTechnicalFaultType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Response message for hotel distribution
                                    errors</xsd:documentation>
    </xsd:annotation>
    <xsd:complexContent>
      <xsd:extension base="cmn:TechnicalFaultType"/>
    </xsd:complexContent>
  </xsd:complexType>
  <xsd:complexType name="SearchHotelRequestType">
    <xsd:sequence>
      <xsd:element name="request" type="msg:SearchHotelRequestMessageType"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="SearchHotelRequestMessageType">
    <xsd:sequence>
      <xsd:element ref="cmn:searchRequestHeader"/>
      <xsd:element name="hotelSearchRequest" type="dst:HotelDistributionSearchCriteriaType" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="hotelSearchFilter" type="dst:HotelDistributionSearchFilterType" maxOccurs="1" minOccurs="0"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="SearchHotelResponseType">
    <xsd:sequence>
      <xsd:element name="response" type="msg:SearchHotelResponseMessageType"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="SearchHotelResponseMessageType">
    <xsd:sequence>
      <xsd:element ref="cmn:searchResponseHeader" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="hotelDistributionSummaries" minOccurs="1" maxOccurs="1">
        <xsd:complexType>
          <xsd:sequence>
            <xsd:element ref="dst:hotelDistributionSearchResult" minOccurs="0" maxOccurs="unbounded"/>
          </xsd:sequence>
        </xsd:complexType>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
</xsd:schema>]]></con:content>
        <con:type>http://www.w3.org/2001/XMLSchema</con:type>
      </con:part>
      <con:part>
        <con:url>http://esb.services.ext.pci.qa.chotel.com:80/HotelDistributionService/v6?SCHEMA%2FCdm_Shared_v6%2Fxsd%2Fcommon%2FCommonTypes</con:url>
        <con:content><![CDATA[<!--Document: The CommonTypes schema contains XSD types that are used
          by multiple canonical schemas. They are pulled together
          in this file to maximize reuse.

Date: 12-10-2010
Last Updated:  04-24-2019
Authors: Chris Judson, Kirk Damron, Charlie Taylor, Jared Sherrill, Andrew Baker, Matthew Schaub, Maddy Lakshmanan, Jim Conger-->
<xsd:schema targetNamespace="http://www.choicehotels.com/schema/v6/common/cdm" elementFormDefault="qualified" attributeFormDefault="unqualified" xml:lang="en" xmlns:cmn="http://www.choicehotels.com/schema/v6/common/cdm" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <xsd:include schemaLocation="http://esb.services.ext.pci.qa.chotel.com:80/HotelDistributionService/v6?SCHEMA%2FCdm_Shared_v6%2Fxsd%2Fcommon%2FSimpleTypes"/>
  <xsd:element name="acceptableValue" type="cmn:AcceptableValueType"/>
  <xsd:element name="acceptableValueList" type="cmn:AcceptableValueListType"/>
  <xsd:element name="accountId" type="cmn:AccountIdType"/>
  <xsd:element name="address" type="cmn:AddressType"/>
  <xsd:element name="addresses" type="cmn:AddressesType"/>
  <xsd:element name="addressPreferences" type="cmn:AddressPreferencesType"/>
  <xsd:element name="addressSearchCriteria" type="cmn:AddressSearchCriteriaType"/>
  <xsd:element name="amount" type="cmn:AmountType"/>
  <xsd:element name="awardId" type="cmn:AwardIdType"/>
  <xsd:element name="brandCode" type="cmn:BrandCodeType"/>
  <xsd:element name="brandReference" type="cmn:BrandReferenceType"/>
  <xsd:element name="campaignId" type="cmn:CampaignIdType"/>
  <xsd:element name="changeOriginator" type="cmn:ChangeOriginatorType"/>
  <xsd:element name="companyProfile" type="cmn:CompanyProfileType"/>
  <xsd:element name="corporateAccountId" type="cmn:CorporateAccountIdType"/>
  <xsd:element name="country" type="cmn:CountryType"/>
  <xsd:element name="countrySubdivision" type="cmn:CountrySubdivisionType"/>
  <xsd:element name="currency" type="cmn:CurrencyType"/>
  <xsd:element name="currencyCode" type="cmn:CurrencyCodeType"/>
  <xsd:element name="dateSpan" type="cmn:DateSpanType"/>
  <xsd:element name="dateTimeSpan" type="cmn:DateTimeSpanType"/>
  <xsd:element name="deadline" type="cmn:DeadlineType"/>
  <xsd:element name="emailAddress" type="cmn:EmailAddressType"/>
  <xsd:element name="emailAddresses" type="cmn:EmailAddressesType"/>
  <xsd:element name="emailAddressPreferences" type="cmn:EmailAddressPreferencesType"/>
  <xsd:element name="eventHeader" type="cmn:EventHeaderType"/>
  <xsd:element name="encryptionScheme" type="cmn:EncryptionSchemeType"/>
  <xsd:element name="guestId" type="cmn:GuestIdType"/>
  <xsd:element name="hotelGroup" type="cmn:HotelGroupType"/>
  <xsd:element name="hotelId" type="cmn:HotelIdType"/>
  <xsd:element name="hotelIds" type="cmn:HotelIdsType"/>
  <xsd:element name="hotelName" type="cmn:HotelNameType"/>
  <xsd:element name="hotelReference" type="cmn:HotelReferenceType"/>
  <xsd:element name="hotelReferences" type="cmn:HotelReferencesType"/>
  <xsd:element name="hotelReservationId" type="cmn:HotelReservationIdType"/>
  <xsd:element name="hotelReservationCancellationId" type="cmn:HotelReservationCancellationIdType"/>
  <xsd:element name="hotelReservationConfirmationId" type="cmn:HotelReservationConfirmationIdType"/>
  <xsd:element name="keywords" type="cmn:KeywordsType"/>
  <xsd:element name="locale" type="cmn:LocaleType"/>
  <xsd:element name="locales" type="cmn:LocalePreferencesType"/>
  <xsd:element name="loyaltyAccountId" type="cmn:LoyaltyAccountIdType"/>
  <xsd:element name="loyaltyProgramId" type="cmn:LoyaltyProgramIdType"/>
  <xsd:element name="messageHeader" type="cmn:MessageHeaderType"/>
  <xsd:element name="messageResponse" type="cmn:MessageResponseType"/>
  <xsd:element name="mobileDeviceAddress" type="cmn:MobileDeviceAddressType"/>
  <xsd:element name="mobileDevicePreferences" type="cmn:MobileDevicePreferencesType"/>
  <xsd:element name="money" type="cmn:MoneyType"/>
  <xsd:element name="numberOfGuests" type="cmn:NumberOfGuestsType"/>
  <xsd:element name="offerId" type="cmn:OfferIdType"/>
  <xsd:element name="operatingHours" type="cmn:OperatingHoursType"/>
  <xsd:element name="operatingSchedule" type="cmn:OperatingScheduleType"/>
  <xsd:element name="organization" type="cmn:OrganizationType"/>
  <xsd:element name="organizationId" type="cmn:OrganizationIdType"/>
  <xsd:element name="passwordHint" type="cmn:PasswordHintType"/>
  <xsd:element name="paymentCardNumber" type="cmn:PaymentCardNumberType"/>
  <xsd:element name="person" type="cmn:PersonType"/>
  <xsd:element name="personName" type="cmn:PersonNameType"/>
  <xsd:element name="phone" type="cmn:PhoneType"/>
  <xsd:element name="phones" type="cmn:PhonesType"/>
  <xsd:element name="phonePreferences" type="cmn:PhonePreferencesType"/>
  <xsd:element name="privacyPreferences" type="cmn:PrivacyPreferencesType"/>
  <xsd:element name="productCode" type="cmn:ProductCodeType"/>
  <xsd:element name="productReference" type="cmn:ProductReferenceType"/>
  <xsd:element name="promotionId" type="cmn:PromotionIdType"/>
  <xsd:element name="ratePlanCode" type="cmn:RatePlanCodeType"/>
  <xsd:element name="relatedOrganization" type="cmn:RelatedOrganizationType"/>
  <xsd:element name="relatedOrganizations" type="cmn:RelatedOrganizationsType"/>
  <xsd:element name="requestMessageHeader" type="cmn:RequestMessageHeaderType"/>
  <xsd:element name="responseMessageHeader" type="cmn:ResponseMessageHeaderType"/>
  <xsd:element name="revisionStamp" type="cmn:RevisionStampType"/>
  <xsd:element name="roomTypeId" type="cmn:RoomTypeIdType"/>
  <xsd:element name="serviceDescriptiveInfo" type="cmn:ServiceDescriptiveInfoType"/>
  <xsd:element name="searchRequestHeader" type="cmn:SearchRequestHeaderType"/>
  <xsd:element name="searchResponseHeader" type="cmn:SearchResponseHeaderType"/>
  <xsd:element name="stayId" type="cmn:StayIdType"/>
  <xsd:element name="tax" type="cmn:TaxType"/>
  <xsd:element name="taxes" type="cmn:TaxesType"/>
  <xsd:element name="taxId" type="cmn:TaxIdType"/>
  <xsd:element name="taxIds" type="cmn:TaxIdsType"/>
  <xsd:element name="travelAgentId" type="cmn:TravelAgentIdType"/>
  <xsd:element name="uniqueId" type="cmn:UniqueIdType"/>
  <xsd:element name="user" type="cmn:UserType"/>
  <xsd:element name="userAuthentication" type="cmn:UserAuthenticationType"/>
  <xsd:element name="userCredentials" type="cmn:UserCredentialsType"/>
  <xsd:complexType name="AcceptableValueListType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A list of acceptable values. The common use-case for
                                    this is to define a set of values for a pick-list.</xsd:documentation>
    </xsd:annotation>
    <xsd:complexContent>
      <xsd:extension base="cmn:AttributeFamilyType"/>
    </xsd:complexContent>
  </xsd:complexType>
  <xsd:complexType name="AcceptableValueType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Defines a value that is acceptable to use in a
                                    specific condition.</xsd:documentation>
    </xsd:annotation>
    <xsd:complexContent>
      <xsd:extension base="cmn:AttributeType"/>
    </xsd:complexContent>
  </xsd:complexType>
  <xsd:complexType name="AccountIdType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Unique identifier to identify a specific
                                    sales account.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="id" type="cmn:StringLength1to32Type" minOccurs="1" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="AddressType">
    <xsd:sequence>
      <xsd:element name="line1" type="cmn:StringLength1to64Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The address lines contain free form
                                      address details.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="line2" type="cmn:StringLength1to64Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The address lines contain free form
                                      address details.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="line3" type="cmn:StringLength1to64Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The address lines contain free form
                                      address details.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="line4" type="cmn:StringLength1to64Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The address lines contain free form
                                      address details.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="city" type="cmn:StringLength1to64Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">City (e.g., Dublin), town, or postal
                                      station (i.e., a postal service territory,
                                      often used in a military address).</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="postalCode" type="cmn:StringLength1to16Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Code used by the country's postal
                                      authority for mail delivery (e.g., zipcode
                                      in the US)</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="county" type="cmn:StringLength1to32Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">County or Region Name (e.g., "Fairfax").</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="stateOrProvince" type="cmn:StateProvinceType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="country" type="cmn:CountryCodeType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">These codes are the upper-case, two-letter
                                      codes as defined by ISO-3166-1 alpha 2</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
    <xsd:attribute name="kind" type="cmn:StringLength1to32Type" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">Type of address (Home, Work, etc.)</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
  </xsd:complexType>
  <xsd:complexType name="AddressesType">
    <xsd:sequence>
      <xsd:element name="address" type="cmn:AddressType" minOccurs="1" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="AddressPreferencesType">
    <xsd:sequence>
      <xsd:element name="primaryAddress" type="cmn:AddressType" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="otherAddress" type="cmn:AddressType" minOccurs="0" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="AddressSearchCriteriaType">
    <xsd:sequence>
      <xsd:element name="city" type="cmn:StringLength1to64Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">City (e.g., Dublin), town, or postal
                                      station (i.e., a postal service territory,
                                      often used in a military address).</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="postalCode" type="cmn:StringLength1to16Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Code used by the country's postal
                                      authority for mail delivery (e.g., zipcode
                                      in the US)</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="county" type="cmn:StringLength1to32Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">County or Region Name (e.g., "Fairfax").</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="stateOrProvince" type="cmn:StateProvinceType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">State or Province name (e.g., "Texas").</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="country" type="cmn:CountryCodeType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">These codes are the upper-case, two-letter
                                      codes as defined by ISO-3166-1 alpha 2</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="AmountType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">The amount for the services with the ability
                                    to track taxes.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="taxes" type="cmn:TaxesType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">A collection of taxes.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="amountBeforeTax" type="cmn:MoneyType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The total amount not including any
                                      associated tax (e.g., sales tax, VAT, GST
                                      or any associated tax).</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="amountAfterTax" type="cmn:MoneyType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The total amount including all associated
                                      taxes (e.g., sales tax, VAT, GST or any
                                      associated tax).</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element ref="cmn:currencyCode" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Provides a currency code to reflect the
                                      currency in which an amount may be
                                      expressed .</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="AreaType">
    <xsd:sequence>
      <xsd:element name="value" type="xsd:double">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Area in UOM.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="units" type="cmn:AreaUnitOfMeasureType">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Area Unit Of Measure.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="AttributeFamilyType">
    <xsd:annotation>
      <xsd:documentation>This is for extensibility within certain predefined
                      extension type (eg, PrivacyRules and
                      PersonalizationAttributes) Personalization attributes are
                      just part of the Guest, so there's no separate op for
                      them. This is not an element because this type is expected
                      to be extended for use.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="description" type="cmn:StringLength1to255Type" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="attributes" minOccurs="1" maxOccurs="1">
        <xsd:complexType>
          <xsd:sequence>
            <xsd:element name="attribute" type="cmn:AttributeType" minOccurs="1" maxOccurs="unbounded"/>
          </xsd:sequence>
        </xsd:complexType>
      </xsd:element>
    </xsd:sequence>
    <xsd:attribute name="kind" type="cmn:AttributeKindType" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">Classifies all attributes in this family (i.e., all
                                    of the contained attributes must implicitly or
                                    explicitly have the same type).</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
  </xsd:complexType>
  <xsd:complexType name="AttributeType">
    <xsd:sequence>
      <xsd:element name="key" type="xsd:string" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="values" minOccurs="1" maxOccurs="1">
        <xsd:complexType>
          <xsd:sequence>
            <xsd:element name="value" type="xsd:string" minOccurs="1" maxOccurs="unbounded"/>
            <xsd:element name="lastUpdateTime" type="xsd:date" minOccurs="0" maxOccurs="1"/>
          </xsd:sequence>
        </xsd:complexType>
      </xsd:element>
    </xsd:sequence>
    <xsd:attribute name="kind" type="cmn:AttributeKindType" use="optional"/>
  </xsd:complexType>
  <xsd:complexType name="AwardIdType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Unique identifier to identify a specific
                                    loyalty award.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="id" type="cmn:StringLength1to32Type" minOccurs="1" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="BaseHeaderType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">This type defines the standard elements and
                                    attributes that are needed for all messages
                                    and events.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="echoToken" type="cmn:StringLength1to128Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">A reference for additional message
                                      identification, assigned by the requesting
                                      host system. When a request message
                                      includes an echo token the corresponding
                                      response message MUST include an echo
                                      token with an identical value.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="timeStamp" type="xsd:dateTime" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Indicates the creation date and time of
                                      the message in UTC using the following
                                      format specified by ISO 8601;
                                      YYYY-MM-DDThh:mm:ssZ with time values
                                      using the 24 hour clock (e.g. 20 November
                                      2003, 1:59:38 pm UTC becomes
                                      2003-11-20T13:59:38Z).</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="duplicate" type="xsd:boolean" default="false" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Used to indicate if the message is a
                                      duplicate message. This can occur when the
                                      system is retrying a message it sent
                                      earlier and there was no response or an
                                      error.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="trackingId" type="cmn:TrackingIdType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Identifier that allows end-to-end tracking
                                      of the business transaction across
                                      synchronous service calls, asynchronous
                                      service calls, faults and message
                                      processing. This identifier is suitable
                                      for tracing a call chain for audit or
                                      troubleshooting purposes.
                                      
                                      If the service is invoked from another
                                      service this is the trackingId passed in
                                      the request header of the invoking
                                      service. Otherwise, this id is generated
                                      by the component (e.g., application) that
                                      is invoking the service.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="contextId" type="cmn:ContextIdType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Identifier that is used to reference state 
                                      maintained across multiple invocations.
                                      For example, a hotel reservation may be
                                      built over several service invocations.
                                      This identifier provides a means for the
                                      client to inform the service that the
                                      current invocation is part of a series of
                                      invocations and provides a means for the
                                      service to manage state across those
                                      invocations. This is not a means for
                                      handling distributed transactions.
     
                                      The client must provide the contextId if
                                      one has been previously returned by the
                                      service and the client does not desire a
                                      new context. The client may also propagate
                                      the contextId from a request made by an
                                      external partner (e.g., an OTA partner).</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element ref="cmn:locale" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Client specific locale when requesting
                                      localized content.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element ref="cmn:organizationId" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The namespace of the entity making this
                                      request. For OTA based clients this
                                      information can be derived from the
                                      POS/Source/RequestorID.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
    <xsd:attribute name="version" type="xsd:decimal" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">The version of the canonical schema used to
                                     create the message payload.</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
    <xsd:attribute name="sequenceNumber" type="xsd:nonNegativeInteger" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">Used to identify the sequence number of the
                                     transaction as assigned by the sending
                                     system; allows for an application to
                                     process messages in a certain order or to
                                     request a resynchronization of messages in
                                     the event that a system has been off-line
                                     and needs to retrieve messages that were
                                     missed.</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
  </xsd:complexType>
  <xsd:complexType name="BrandCodeType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Unique identifier to identify a specific
                                    Brand.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="id" type="cmn:StringLength1to32Type" minOccurs="1" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="BrandReferenceType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">The identity of a marketing brand.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element ref="cmn:brandCode" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="name" type="cmn:StringLength1to64Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Name of the brand (e.g., Sleep,Cambria Suites, Clarion).</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="CampaignIdType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Unique identifier to identify a specific
                                    marketing campaign.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="id" type="cmn:StringLength1to32Type" minOccurs="1" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="ChangeOriginatorType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Describes the originator of the change</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="application" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation>Describes the application that originated the change</xsd:documentation>
        </xsd:annotation>
        <xsd:complexType>
          <xsd:sequence>
            <xsd:element name="owner" type="cmn:StringLength1to64Type" minOccurs="1" maxOccurs="1">
              <xsd:annotation>
                <xsd:documentation>Owner of the application (e.g., Choice Hotels, American Airlines). This
                           is the name of the company, organization, business unit, or other
                           organizational unit.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="name" type="cmn:StringLength1to64Type" minOccurs="1" maxOccurs="1">
              <xsd:annotation>
                <xsd:documentation>Name of the application</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
          </xsd:sequence>
        </xsd:complexType>
      </xsd:element>
      <xsd:element minOccurs="0" maxOccurs="1" ref="cmn:user">
        <xsd:annotation>
          <xsd:documentation>Name of the user who made the change</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="CompanyProfileType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Profile for a company.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="name" type="cmn:StringLength1to64Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Name of the associated company.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element ref="cmn:corporateAccountId" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Code for the associated company.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="contactInfo" type="cmn:ContactInfoType" minOccurs="0" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="ConditionalsType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Collection of conditionals</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="conditional" type="cmn:ConditionalType" minOccurs="0" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="ConditionalType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Rule that governs the use of an entity or other behavior</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="name" type="cmn:ConditionalNameType" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Identifies the conditional and expresses its purpose (e.g., DOWRestriction, LOSTier)</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="description" maxOccurs="1" type="cmn:StringLength1to255Type" minOccurs="0"></xsd:element>
      <xsd:element name="parameters" type="cmn:ParametersType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Data that influences the conditional (e.g., [Fri, Sat] for DOWRestriction, 1 for LOSTier)</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="ContactInfoType">
    <xsd:sequence>
      <xsd:element ref="cmn:addressPreferences" minOccurs="0" maxOccurs="1"/>
      <xsd:element ref="cmn:phonePreferences" minOccurs="0" maxOccurs="1"/>
      <xsd:element ref="cmn:emailAddressPreferences" minOccurs="0" maxOccurs="1"/>
      <xsd:element ref="cmn:mobileDevicePreferences" minOccurs="0" maxOccurs="1"/>
      <xsd:element ref="cmn:privacyPreferences" minOccurs="0" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="CorporateAccountIdType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Unique identifier to identify a specific
                                    corporate account.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="id" type="cmn:StringLength1to32Type" minOccurs="1" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="CountrySubdivisionType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">The definition of a subdivision (the first
                                    level of separation under a country for
                                    example: state, province, district, county)
                                    with its relationship with the country it
                                    belongs to.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="code" type="cmn:CountrySubdivisionCodeType" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="commonAbbreviation" type="cmn:StringLength1to8Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">This is the most common "local"
                                      abbreviation for the subdivision. This
                                      could be the second part of the ISO 3166-2
                                      standard (i.e. SubdivisionCode = US-AZ but
                                      commonAbbreviation = AZ) or some other
                                      abbreviation that is more commonly used.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="countryCode" type="cmn:CountryCodeType" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="name" type="cmn:StateProvinceType" minOccurs="1" maxOccurs="1"/>
    </xsd:sequence>
    <xsd:attribute name="kind" type="cmn:CountrySubdivisionKindType" use="optional"/>
    <xsd:attributeGroup ref="cmn:locale"/>
  </xsd:complexType>
  <xsd:complexType name="CountryType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Definition of a country.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="CRSCode" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation>The country code maintained in the CRS that is carried
                        here for backward compatability. This code has been
                        deprecated and should be used with caution.</xsd:documentation>
        </xsd:annotation>
        <xsd:simpleType>
          <xsd:restriction base="xsd:string">
            <xsd:length value="2"/>
          </xsd:restriction>
        </xsd:simpleType>
      </xsd:element>
      <xsd:element name="currencyCode" type="cmn:CurrencyCodeType" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="dialingCodes" minOccurs="0" maxOccurs="1">
        <xsd:complexType>
          <xsd:sequence>
            <xsd:element name="primaryDialingCode" type="cmn:InternationalDirectDialingCodeType" minOccurs="1" maxOccurs="1"/>
            <xsd:element name="otherDialingCode" type="cmn:InternationalDirectDialingCodeType" minOccurs="0" maxOccurs="unbounded"/>
          </xsd:sequence>
        </xsd:complexType>
      </xsd:element>
      <xsd:element name="iso2Code" type="cmn:CountryCodeType" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="iso3Code" type="cmn:CountryIso3CodeType" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="name" type="cmn:StringLength1to64Type" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="unitOfMeasure" type="cmn:StringLength1to16Type" minOccurs="0" maxOccurs="1"/>
    </xsd:sequence>
    <xsd:attributeGroup ref="cmn:locale"/>
  </xsd:complexType>
  <xsd:complexType name="CurrencyAmountType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Provides a monetary amount and the currency
                                    code to reflect the currency in which this
                                    amount is expressed.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="amount" type="cmn:MoneyType" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">A monetary amount.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element ref="cmn:currencyCode" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Provides a currency code to reflect the
                                      currency in which an amount may be
                                      expressed .</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="CurrencyType">
    <xsd:sequence>
      <xsd:element name="code" type="cmn:CurrencyCodeType" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="decimalPlaces" type="xsd:nonNegativeInteger" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation>The number of decimal places that are valid for this
                        currency code.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="name" type="cmn:StringLength1to32Type" minOccurs="0" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="DateSpanType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Type used to specify a date and/or time
                                    range. The range can be absolute with a
                                    specified start and end date or relative
                                    with a start date and a duration.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="start" type="xsd:date" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The starting value of the time span.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:choice minOccurs="1" maxOccurs="1">
        <xsd:element name="end" type="xsd:date" minOccurs="0" maxOccurs="1">
          <xsd:annotation>
            <xsd:documentation xml:lang="en">The ending value of the time span.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <xsd:element name="duration" type="xsd:duration" minOccurs="0" maxOccurs="1">
          <xsd:annotation>
            <xsd:documentation xml:lang="en">The duration datatype represents a
                                       combination of year, month, day and time
                                       values representing a single duration of
                                       time, encoded as a single string.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
      </xsd:choice>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="DateTimeSpanType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Type used to specify a date and/or time
                                    range. The range can be absolute with a
                                    specified start and end date or relative
                                    with a start date and a duration.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="start" type="xsd:dateTime" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The starting value of the time span.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:choice minOccurs="1" maxOccurs="1">
        <xsd:element name="duration" type="xsd:duration" minOccurs="0" maxOccurs="1">
          <xsd:annotation>
            <xsd:documentation xml:lang="en">The duration datatype represents a
                                       combination of year, month, day and time
                                       values representing a single duration of
                                       time, encoded as a single string.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <xsd:element name="end" type="xsd:dateTime" minOccurs="0" maxOccurs="1">
          <xsd:annotation>
            <xsd:documentation xml:lang="en">The ending value of the time span.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
      </xsd:choice>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="DeadlineType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">The absolute deadline or amount of offset
                                    time before a deadline for a payment or
                                    cancel goes into effect.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:choice minOccurs="1" maxOccurs="1">
        <xsd:element name="absoluteDateTime" type="xsd:dateTime">
          <xsd:annotation>
            <xsd:documentation xml:lang="en">Defines the absolute deadline as a date,
                                       time and GMT offset.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <xsd:sequence>
          <xsd:element name="timeUnitMultiplier" type="cmn:Numeric1to999Type">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">The number of units of timeUnit.</xsd:documentation>
            </xsd:annotation>
          </xsd:element>
          <xsd:element name="timeUnit" type="cmn:TimeUnitType">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">The units of time, e.g.: days, hours,
                                        etc., that apply to the deadline.</xsd:documentation>
            </xsd:annotation>
          </xsd:element>
        </xsd:sequence>
      </xsd:choice>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="DimensionType">
    <xsd:sequence>
      <xsd:element name="length" type="xsd:nonNegativeInteger">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Dimension length in UOM.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="width" type="xsd:nonNegativeInteger">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Dimension width in UOM.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="height" type="xsd:nonNegativeInteger">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Dimension height in UOM.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="units" type="cmn:DistanceUnitOfMeasureType">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Dimension Unit Of Measure.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="area" type="cmn:AreaType">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Actual area if it can't be calculated from
                                      lenght and width (i.e. non-square).</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="DistanceType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Describes a linear measurement.</xsd:documentation>
    </xsd:annotation>
    <xsd:attribute name="value" type="xsd:double" use="required">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">Length in UOM.</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
    <xsd:attribute name="units" type="cmn:DistanceUnitOfMeasureType" use="required">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">Distance Unit Of Measure.</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
  </xsd:complexType>
  <xsd:complexType name="DistanceAndDirectionType">
    <xsd:sequence>
      <xsd:element name="distance" type="cmn:DistanceType">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Distance from origin to target.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="direction" type="cmn:DirectionType">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Direction from origin to target.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="EmailAddressesType">
    <xsd:sequence>
      <xsd:element name="emailAddress" type="cmn:EmailAddressType" minOccurs="1" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="EmailAddressPreferencesType">
    <xsd:sequence>
      <xsd:element name="primaryEmailAddress" type="cmn:EmailAddressType" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="otherEmailAddress" type="cmn:EmailAddressType" minOccurs="0" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="EmailAddressType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Email Address information.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="address" type="cmn:EmailAddressFormatType" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The email adddress</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
    <xsd:attribute name="kind" type="cmn:StringLength1to16Type" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">Specifies the kind of email address (e.g.,
                                     Home, Work)</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
    <xsd:attribute name="undeliverable" type="xsd:boolean" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">Indicates email cannot be delivered to this
                                     email address.</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
  </xsd:complexType>
  <xsd:complexType name="MobileDevicePreferencesType">
    <xsd:sequence>
      <xsd:element name="primaryMobileDevice" type="cmn:MobileDeviceType" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="otherMobileDevices" type="cmn:MobileDeviceType" minOccurs="0" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="MobileDeviceType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A mobile device is a handheld tablet or
                                    other device that is made for
                                    portability, and is therefore both
                                    compact and lightweight. There are many
							        types of mobile devices, the commonest
                                    among them being, mobile phones and
                                    tablets</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="address" type="cmn:MobileDeviceAddressType" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">This is the endpoint of the device
  	  						          generated by a external vendor.For ex,
						              Amazon creates ARN for each device.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element ref="cmn:privacyPreferences" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">This is the per-device
                                      preference of the  customer
                                      regarding push notification</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
    <xsd:attribute name="deviceId" type="xsd:string" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">The device id is a distinctive number
     								  associated with a smartphone or similar
                                      handheld device.</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
    <xsd:attribute name="name" type="cmn:StringLength1to64Type" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">The name of the mobile device eg
                                     Samsung S5.</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
    <xsd:attribute name="modelNumber" type="cmn:StringLength1to64Type" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">The model number of the device eg Model
                                     A1549.This is used to differentiate one
                                     product in a series from another</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
    <xsd:attribute name="operatingSystem" type="cmn:StringLength1to16Type" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">A mobile operating system is the software
                                       platform on top of which other programs
                                       can run on mobile devices.eg iOS</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
    <xsd:attribute name="operatingSystemVersion" type="cmn:StringLength1to16Type" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">A version number is a unique number or set
     								 of numbers assigned to a specific release
                                     of the mobile OS</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
  </xsd:complexType>
  <xsd:complexType name="EncryptionSchemeType">
    <xsd:annotation>
      <xsd:documentation>Describes an the encryption scheme that may be applied to
                      a piece of data.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="algorithm" type="cmn:StringLength1to32Type" maxOccurs="1" minOccurs="1">
        <xsd:annotation>
          <xsd:documentation>The algorithm used (e.g., AES, SHA-256, PGP).</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="algorithmParameter" type="cmn:StringLength1to16Type" maxOccurs="unbounded" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation>Algorithm parameter (e.g., ECB, NoPadding,
                        PKCS5PADDING), one per element.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="keyID" type="cmn:StringLength1to64Type" maxOccurs="1" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation>The identifier of the encryption key used. This MUST NOT
                        be the key itself.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="EventHeaderType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">This type is the basic message header for
                                    all event types. It should be included in
                                    all event messages.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="id" type="cmn:UuidType" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="name" type="cmn:StringLength1to32Type" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The name of the business event that
                                      initiated this event. (i.e. Room Rate,
                                      Hotel Reservation)</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="cause" type="cmn:StringLength1to32Type" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">What caused this event to happen. (i.e.
                                      rate plan created, RACK rate changed, etc.)</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="source" minOccurs="1" maxOccurs="1">
        <xsd:complexType>
          <xsd:sequence>
            <xsd:element name="system" minOccurs="1" maxOccurs="1">
              <xsd:annotation>
                <xsd:documentation>Describes the system that emitted the event</xsd:documentation>
              </xsd:annotation>
              <xsd:complexType>
                <xsd:sequence>
                  <xsd:element name="owner" type="cmn:StringLength1to64Type" minOccurs="1" maxOccurs="1">
                    <xsd:annotation>
                      <xsd:documentation>Owner of the system (e.g., Choice Hotels, American
                              Airlines). This is the name of the company,
                              business unit, or other organizational unit.</xsd:documentation>
                    </xsd:annotation>
                  </xsd:element>
                  <xsd:element name="name" type="cmn:StringLength1to64Type" minOccurs="1" maxOccurs="1">
                    <xsd:annotation>
                      <xsd:documentation>Name of the system</xsd:documentation>
                    </xsd:annotation>
                  </xsd:element>
                </xsd:sequence>
              </xsd:complexType>
            </xsd:element>
            <xsd:element name="user" type="cmn:StringLength1to64Type" minOccurs="0" maxOccurs="1">
              <xsd:annotation>
                <xsd:documentation>Name of the user who caused the event to be emitted</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
          </xsd:sequence>
        </xsd:complexType>
      </xsd:element>
      <xsd:element name="state" type="cmn:StringLength1to16Type" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Used to track the type of event (i.e.
                                      created, changed, deleted)</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="timeStamp" type="xsd:dateTime" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Indicates the creation date and time of
                                      the message in UTC using the following
                                      format specified by ISO 8601;
                                      YYYY-MM-DDThh:mm:ssZ with time values
                                      using the 24 hour clock (e.g. 20 November
                                      2003, 1:59:38 pm UTC becomes
                                      2003-11-20T13:59:38Z).</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="organizationId" minOccurs="0" maxOccurs="1" type="cmn:OrganizationIdType">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The specific identity of the entity
                                      publishing this event.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="trackingId" type="cmn:TrackingIdType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Identifier that allows end-to-end tracking
                                      of the business transaction across
                                      synchronous service calls, asynchronous
                                      service calls, faults and message
                                      processing. This identifier is suitable
                                      for tracing a call chain for audit or
                                      troubleshooting purposes.
                                      
                                      If the event is emitted as a result of a
                                      service invocation, this is the trackingId
                                      passed in the request header. Otherwise,
                                      this id is generated by the component
                                      (e.g., application, sensor) that creates
                                      the event.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="contextId" type="cmn:ContextIdType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Identifier that is used to reference state 
                                      maintained across multiple invocations.
                                      For example, a hotel reservation may be
                                      built over several service invocations.
                                      This identifier provides a means for the
                                      client to inform the service that the
                                      current invocation is part of a series of
                                      invocations and provides a means for the
                                      service to manage state across those
                                      invocations. This is not a means for
                                      handling distributed transactions.
                                      
                                      This is required if the event is
                                      participating in state management and is
                                      omitted otherwise. If the event is emitted
                                      as a result of a service invocation, this
                                      is the contextId passed in the request
                                      header. Otherwise, this id is generated by
                                      the component (e.g., application) that
                                      creates the event.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="GeographicMercatorRectangleType">
    <xsd:sequence>
      <xsd:element name="corner1" type="cmn:GeographicPointType" maxOccurs="1" minOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Any corner of the rectangle.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="corner2" type="cmn:GeographicPointType" maxOccurs="1" minOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The corner diagonally opposite to corner 1.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="GeographicPointsType">
    <xsd:sequence>
      <xsd:element name="point" type="cmn:GeographicPointType" maxOccurs="unbounded" minOccurs="2"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="GeographicPolygonType">
    <xsd:sequence>
      <xsd:element name="points" type="cmn:GeographicPointsType">
        <xsd:annotation>
          <xsd:documentation>The points that define the vertices of the polygon area.
                        It is an error if the polygon sides intersect
                        (overlapping polygon). The first point in the list will
                        be connected to the last point in the list to make a
                        closed area.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="GeographicVicinityType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Used to specify all points within a given
                                    distance from a location on in other words,
                                    a circular area around a location.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="location" type="cmn:GeographicPointType" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation>The center of the circle.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="distance" type="cmn:DistanceType" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation>The radius of the circle.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="GeographicPointType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Used to specify the geographic coordinates
                                    of a location.</xsd:documentation>
    </xsd:annotation>
    <xsd:attribute name="latitude" type="cmn:LatitudeType" use="required">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">The measure of the angular distance on a
                                     meridian north or south of the equator.</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
    <xsd:attribute name="longitude" type="cmn:LongitudeType" use="required">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">The measure of the angular distance on a
                                     meridian east or west of the prime
                                     meridian.</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
  </xsd:complexType>
  <xsd:complexType name="GuestIdType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Unique identifier to identify a specific
                                    Guest.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="id" type="cmn:StringLength1to32Type" minOccurs="1" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="HotelGroupType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Defines a particular Hotel Chain or
                                    Management Company, for example, Hilton,
                                    Marriott.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="group" type="cmn:OrganizationIdType" maxOccurs="1" minOccurs="0"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="HotelIdsType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A collection of HotelIds.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="hotelId" type="cmn:HotelIdType" minOccurs="1" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="HotelIdType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Unique identifier to identify a specific
                                    Hotel.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="id" type="cmn:StringLength1to32Type" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="uuid" type="cmn:UuidType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="altId" type="cmn:StringLength1to32Type" minOccurs="0" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="HotelNameType">
    <xsd:sequence>
      <xsd:element name="name" type="cmn:StringLength1to64Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The primary name for the Hotel.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="HotelNamesType">
    <xsd:sequence>
      <xsd:element name="hotelName" type="cmn:HotelNameType" minOccurs="0" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="HotelReferenceType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Base hotel information that everybody will need.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element ref="cmn:hotelId" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The code that uniquely identifies a single hotel property.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element ref="cmn:hotelGroup" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The hotel group representing this Hotel.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element ref="cmn:hotelName" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The hotel name derived from legal name, brand name and product name.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element ref="cmn:brandReference" minOccurs="0" maxOccurs="1"/>
      <xsd:element ref="cmn:productReference" minOccurs="0" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="HotelReferencesType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Collection of Hotel references.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element ref="cmn:hotelReference" minOccurs="1" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="HotelReservationIdType">
    <xsd:sequence>
      <xsd:element name="id" type="cmn:UniqueIdType" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">This a generic reservation Id.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="HotelReservationCancellationIdType">
    <xsd:sequence>
      <xsd:element name="id" type="cmn:UniqueIdType" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">This a generic reservation Id.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="HotelReservationConfirmationIdType">
    <xsd:sequence>
      <xsd:element name="id" type="cmn:UniqueIdType" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">This a generic reservation Id.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="KeywordsType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A collection of words that can be used to describe or
                                    classify an entity. These words are to aid in the
                                    location of entities having matching words.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="keyword" type="cmn:StringLength1to64Type" minOccurs="1" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="LocalePreferencesType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Code for the language spoken by the customer.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="primaryLocale" type="cmn:LocaleType" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="otherLocale" type="cmn:LocaleType" minOccurs="0" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="LocalesType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Code for the language spoken by the customer.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="locale" type="cmn:LocaleType" minOccurs="1" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="LocaleType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A LocaleType represents a specific
                                    geographical, political, or cultural region.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="language" type="cmn:LanguageCodeType" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">These codes are the lower-case, two-letter
                                      codes as defined by ISO-639-1.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="country" type="cmn:CountryCodeType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">These codes are the upper-case, two-letter
                                      codes as defined by ISO-3166-1 alpha 2.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="variant" type="cmn:StringLength1to32Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The variant argument is an application
                                      specific code. If there are two variants,
                                      separate them with an underscore, and put
                                      the most important one first. For example,
                                      a Traditional Spanish collation might
                                      construct a locale with parameters for
                                      language, country and variant as: "es",
                                      "ES", "Traditional_WIN".</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="LoyaltyAccountIdType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Unique identifier for a loyalty account</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="programId" type="cmn:LoyaltyProgramIdType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="accountNumber" minOccurs="0" maxOccurs="1">
        <xsd:simpleType>
          <xsd:annotation>
            <xsd:documentation xml:lang="en">Specifies the required pattern for a
                                       Loyalty account number.</xsd:documentation>
          </xsd:annotation>
          <xsd:restriction base="xsd:string">
            <xsd:pattern value="[A-Z0-9]{1,19}"/>
          </xsd:restriction>
        </xsd:simpleType>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="LoyaltyProgramIdType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Unique identifier to identify a specific
                                    Loyalty Program.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="id" minOccurs="1" maxOccurs="1">
        <xsd:simpleType>
          <xsd:annotation>
            <xsd:documentation xml:lang="en">Specifes the required pattern for a
                                       Loyalty Program identifier.</xsd:documentation>
          </xsd:annotation>
          <xsd:restriction base="xsd:string">
            <xsd:pattern value="[A-Z]{1,8}"/>
          </xsd:restriction>
        </xsd:simpleType>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="MessageHeaderType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">This type extends the BaseHeaderType and is
                                    a placeholder in the event there needs to be
                                    more elements added to the BaseHeaderType.
                                    It should be used as the header for all
                                    messages.</xsd:documentation>
    </xsd:annotation>
    <xsd:complexContent>
      <xsd:extension base="cmn:BaseHeaderType"/>
    </xsd:complexContent>
  </xsd:complexType>
  <xsd:complexType name="OrganizationType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Describes an entity such as an internal business unit
                                    or an external partner.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element ref="cmn:organizationId" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="name" type="cmn:StringLength1to128Type" minOccurs="0" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="ParametersType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A set of parameters</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="parameter" type="cmn:ParameterType" minOccurs="1" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="ParameterType">
    <xsd:annotation>
      <xsd:documentation>Defines a parameter</xsd:documentation>
    </xsd:annotation>
    <xsd:attribute name="value" type="cmn:StringLength1to128Type" use="required"/>
  </xsd:complexType>
  <xsd:complexType name="ProximityType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Describes the distance to a location
                                    relative to a subject location.</xsd:documentation>
    </xsd:annotation>
    <xsd:complexContent>
      <xsd:extension base="cmn:DistanceType">
        <xsd:attribute name="text" type="cmn:StringLength1to64Type" use="optional">
          <xsd:annotation>
            <xsd:documentation xml:lang="en">Text descibing the distance between a
                                        location and the subject location (e.g.,
                                        "on premises", "walking distance",
                                        "two blocks").</xsd:documentation>
          </xsd:annotation>
        </xsd:attribute>
      </xsd:extension>
    </xsd:complexContent>
  </xsd:complexType>
  <xsd:complexType name="RelatedOrganizationsType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A collection of related organizations.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element ref="cmn:relatedOrganization" minOccurs="1" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="RelatedOrganizationType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Describes a relationship to an organization.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element ref="cmn:organization" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="relationshipKind" type="cmn:OrganizationRelationshipKindType" minOccurs="1" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="RequestMessageHeaderType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A specialization of MessageHeader for
                                    requests</xsd:documentation>
    </xsd:annotation>
    <xsd:complexContent>
      <xsd:extension base="cmn:MessageHeaderType">
        <xsd:sequence>
          <xsd:element name="clientIP" type="cmn:IPAddressType" minOccurs="0" maxOccurs="1">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">IP address of the user. A common use for this
                                        is security auditing. The IP address should be
                                        that of the user's browser or mobile app. This
                                        may not be known for B2B integrations.</xsd:documentation>
            </xsd:annotation>
          </xsd:element>
          <xsd:element name="clientAppName" type="cmn:StringLength1to64Type" minOccurs="0" maxOccurs="1">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">Name of the application used by the user
                                       (e.g., US Website, iPhone App, Android App). A common
                                        use for this is security auditing.</xsd:documentation>
            </xsd:annotation>
          </xsd:element>
        </xsd:sequence>
      </xsd:extension>
    </xsd:complexContent>
  </xsd:complexType>
  <xsd:complexType name="ResponseMessageHeaderType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A specialization of MessageHeader for
                                    responses</xsd:documentation>
    </xsd:annotation>
    <xsd:complexContent>
      <xsd:extension base="cmn:MessageHeaderType"/>
    </xsd:complexContent>
  </xsd:complexType>
  <xsd:complexType name="SearchRequestHeaderType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A specialization of RequestMessageHeader for
                                    search requests</xsd:documentation>
    </xsd:annotation>
    <xsd:complexContent>
      <xsd:extension base="cmn:RequestMessageHeaderType">
        <xsd:sequence>
          <xsd:element name="searchLocator" type="cmn:SearchLocatorType" minOccurs="0" maxOccurs="1"/>
        </xsd:sequence>
      </xsd:extension>
    </xsd:complexContent>
  </xsd:complexType>
  <xsd:complexType name="SearchResponseHeaderType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A specialization of ResponseMessageHeader
                                    for search responses</xsd:documentation>
    </xsd:annotation>
    <xsd:complexContent>
      <xsd:extension base="cmn:ResponseMessageHeaderType">
        <xsd:sequence>
          <xsd:element name="searchStatus" type="cmn:SearchStatusType" minOccurs="1" maxOccurs="1"/>
          <xsd:element name="searchLocator" type="cmn:SearchLocatorType" minOccurs="0" maxOccurs="1"/>
        </xsd:sequence>
      </xsd:extension>
    </xsd:complexContent>
  </xsd:complexType>
  <xsd:complexType name="MessageResponseType">
    <xsd:sequence>
      <xsd:element ref="cmn:responseMessageHeader"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="NumberOfGuestsType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Unique identifier to identify a specific
                                    Guest.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="numberOfAdults" type="cmn:Numeric1to999Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The number of adult guests.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="numberOfMinors" type="cmn:Numeric0to999Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The number of minor guests.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
    <xsd:attribute name="perRoom" type="xsd:boolean"/>
  </xsd:complexType>
  <xsd:complexType name="OfferIdType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Unique identifier to identify a specific
                                    marketing offer.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="id" type="cmn:StringLength1to32Type" minOccurs="1" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="OperatingHoursType">
    <xsd:sequence>
      <xsd:element name="dayOfWeek" type="cmn:DayOfWeekType" minOccurs="0" maxOccurs="7">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Day of the week that is applicable for this open/close
                                      pair.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="open" type="xsd:time" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Time this entity is open for operation.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="close" type="xsd:time" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Time this entity is closed for operation.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="openFullDay" type="xsd:boolean" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Specifies that this entity is open the entire day.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="closedFullDay" type="xsd:boolean" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Specifies that the entity is closed the entire day.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="OperatingScheduleType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Schedule of operating hours.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="operatingHours" type="cmn:OperatingHoursType" minOccurs="1" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="PasswordHintType">
    <xsd:annotation>
      <xsd:documentation>Describes a hint a user has established for the purpose of
                      password recovery.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="question" type="cmn:StringLength1to64Type" maxOccurs="1" minOccurs="1">
        <xsd:annotation>
          <xsd:documentation>The hint question.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="response" type="cmn:StringLength1to64Type" maxOccurs="1" minOccurs="1">
        <xsd:annotation>
          <xsd:documentation>The response required to activate this hint.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="PaymentCardNumberType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Identification information for a specific
                                    credit card.</xsd:documentation>
    </xsd:annotation>
    <xsd:choice>
      <xsd:element name="lastFourDigits" type="cmn:StringLength1to4Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Contains only the last 4 digits of the
                                      payment card number.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="token" type="cmn:PaymentCardTokenType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Token representing the credit card</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="number" type="cmn:StringLength1to16Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Credit card account number. The number
                                      embossed on the card. WARNING: this data
                                      must be handled in accordance with PCI
                                      regulations and corporate policy.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:choice>
  </xsd:complexType>
  <xsd:complexType name="PersonContactType">
    <xsd:sequence>
      <xsd:element name="person" type="cmn:PersonType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="contactInfo" type="cmn:ContactInfoType" minOccurs="0" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="PersonNameType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">This provides name information for a person.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="prefix" type="cmn:StringLength1to8Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Salutation of honorific. (e.g., Mr. Mrs.,
                                      Ms., Miss, Dr.)</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="given" type="cmn:StringLength1to32Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Given name, first name or names</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="middle" type="cmn:StringLength1to32Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The middle name of the person name</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="surname" type="cmn:StringLength1to32Type" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Family name, last name.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="suffix" type="cmn:StringLength1to32Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Name suffix (e.g., Jr., Sr., III).</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="designation" type="cmn:StringLength1to32Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Degree, honors and professional
                                      designations (e.g. Ph.D., M.D., CPA).</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="PersonType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">PersonType is the basic components for
                                    making up a person.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element ref="cmn:personName" minOccurs="1" maxOccurs="1"/>
      <xsd:element ref="cmn:locales" minOccurs="0" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="PhoneType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Telephone information.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="countryAccessCode" type="cmn:NumericStringLength1to3Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Code assigned by telecommunications
                                      authorities for international country
                                      access identifier.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="areaCode" type="cmn:NumericStringLength1to8Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Code assigned for telephones in a specific
                                      region, city, or area.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="phoneNumber" type="cmn:StringLength1to32Type" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Telephone number assigned to a single
                                      location. It can support area code + number</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="extension" type="cmn:NumericStringLength1to5Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Extension to reach a specific party at the
                                      phone number.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element ref="cmn:privacyPreferences" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">This is the per-phone preference of the customer
                                      regarding text messages.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
    <xsd:attribute name="kind" type="cmn:StringLength1to32Type" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">Specifies the type of phone number. (Home,
                                     Mobile, etc.)</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
  </xsd:complexType>
  <xsd:complexType name="PhonePreferencesType">
    <xsd:sequence>
      <xsd:element name="primaryPhone" type="cmn:PhoneType" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="otherPhone" type="cmn:PhoneType" minOccurs="0" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="PhonesType">
    <xsd:sequence>
      <xsd:element name="phone" type="cmn:PhoneType" minOccurs="1" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="PrivacyPreferencesType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Set of preferences for a distint data item
                                    (e.g., email address, home phone, business
                                    address)</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="preference" type="cmn:PrivacyPreferenceType" minOccurs="0" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="PrivacyPreferenceType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Privacy preference for a distinct option</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="name" type="cmn:StringLength1to64Type" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Option name (e.g., "corporate marketing",
                                      "partner sharing")</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="optIn" type="xsd:boolean" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">True if consumer has opted-in, either
                                      implicitly or explicitly</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="explicit" type="xsd:boolean" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">True if consumer has made an explicit
                                      opt-in/opt-out selection. False if the
                                      opt-in/opt-out setting was derived from a
                                      default.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="ProductCodeType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Unique identifier to identify a specific
                                    Product.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="id" type="cmn:StringLength1to32Type" minOccurs="1" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="ProductReferenceType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">The identity of a marketing product.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element ref="cmn:productCode" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="name" type="cmn:StringLength1to64Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Name of the product (e.g., Inn, Suite, Resort)</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="PromotionIdType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Unique identifier to identify a specific
                                    Promotion.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="id" type="cmn:StringLength1to32Type" minOccurs="1" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="RatePlanCodeType">
    <xsd:sequence>
      <xsd:annotation>
        <xsd:documentation xml:lang="en">Unique identifier to identify a specific
                                     Rate Plan.</xsd:documentation>
      </xsd:annotation>
      <xsd:element name="code" type="cmn:StringLength1to32Type" minOccurs="1" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="RevisionStampType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Describes the who and when aspects of a change</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="changeOriginator" minOccurs="1" maxOccurs="1" type="cmn:ChangeOriginatorType"/>
      <xsd:element name="timeStamp" type="xsd:dateTime" minOccurs="0" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="RoomTypeIdType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Unique identifier to identify a specific
                                    Room Type.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="id" type="cmn:StringLength1to32Type" minOccurs="1" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="RouteType">
    <xsd:sequence>
      <xsd:element name="points" type="cmn:GeographicPointsType" maxOccurs="1" minOccurs="1">
        <xsd:annotation>
          <xsd:documentation>The points that define the route. These are the
                        generated points that attempt to pass through the
                        waypoints.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="waypoints" type="cmn:WaypointsType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation>The points used to determine the route. The route is the
                        best attempt to pass through these points, starting at
                        the first waypoint, passing as close as possible to the
                        remaining waypoints, ending at the last waypoint.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="RouteAreaType">
    <xsd:sequence>
      <xsd:element name="route" type="cmn:RouteType" maxOccurs="1" minOccurs="1"/>
      <xsd:element name="distance" type="cmn:DistanceType" maxOccurs="1" minOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="SearchLocatorType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">This type is used to iterate over a large
                                    data set.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="id" type="cmn:StringLength1to64Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">A unique id that refers to the query
                                      result set.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="index" type="xsd:nonNegativeInteger" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Index of the next item in the result set.
                                      The starting item of the next window on
                                      the full result set.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="size" type="xsd:nonNegativeInteger" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Defines the size of the window on the full
                                      result set. Example: a window of 50 items
                                      within a result set of 200 items.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="SearchStatusType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Describes the status of a search response</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="done" type="xsd:boolean" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">A flag to indicate that he end of the
                                      result set has been reached.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="totalCount" type="xsd:nonNegativeInteger" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The total number of records in the full
                                      result set.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="ServiceDescriptiveInfoType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Describes characteristics of a service
                                    that would be useful when interacting with
                                    the service.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="generalInfo">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Describes the aspects of the service that
                                      invariant across all operations.</xsd:documentation>
        </xsd:annotation>
        <xsd:complexType>
          <xsd:sequence>
            <xsd:element name="name" type="cmn:StringLength1to64Type" minOccurs="1" maxOccurs="1">
              <xsd:annotation>
                <xsd:documentation xml:lang="en">The name of the service as exposed on
                                         the API.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="description" type="xsd:string" minOccurs="1" maxOccurs="1">
              <xsd:annotation>
                <xsd:documentation xml:lang="en">Describes the purpose of the service.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="supportedLocales" minOccurs="0" maxOccurs="1">
              <xsd:annotation>
                <xsd:documentation xml:lang="en">Enumerates the locales supported by
                                         the service. A client may examine the
                                         set of supported locales to determine
                                         what locale to specify when calling
                                         any of the read operations
                                         (e.g., get, list, search) provided by
                                         the service.</xsd:documentation>
              </xsd:annotation>
              <xsd:complexType>
                <xsd:sequence>
                  <xsd:element ref="cmn:locale" minOccurs="1" maxOccurs="unbounded"/>
                </xsd:sequence>
              </xsd:complexType>
            </xsd:element>
            <xsd:element name="properties" minOccurs="0" maxOccurs="1">
              <xsd:annotation>
                <xsd:documentation xml:lang="en">Describes properties of the service
                                         that are invariant across all
                                         operations. A property could be a
                                         list of allowed or supported values
                                         for a specific type of parameter
                                         (e.g., address kind).</xsd:documentation>
              </xsd:annotation>
              <xsd:complexType>
                <xsd:sequence>
                  <xsd:element name="property" type="cmn:AttributeType" minOccurs="1" maxOccurs="unbounded"/>
                </xsd:sequence>
              </xsd:complexType>
            </xsd:element>
          </xsd:sequence>
        </xsd:complexType>
      </xsd:element>
      <xsd:element name="operations">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Describes each of the operations provided
                                      by the service. The input and output
                                      paramter names are specified in the key
                                      of the parameter element. The key
                                      represents the fully qualified name of the
                                      parameter using dotted notation
                                      (e.g., guest.preferences.bedPreference,
                                      country.unitOfMeasure). If the parameter
                                      is itself a key the parameter name
                                      includes that key (e.g., guest.
                                      preferences.generalPreferences.attributes.
                                      attribute.key.ARMED_SERVICES_BRANCH).</xsd:documentation>
        </xsd:annotation>
        <xsd:complexType>
          <xsd:sequence>
            <xsd:element name="operation" minOccurs="1" maxOccurs="unbounded">
              <xsd:complexType>
                <xsd:sequence>
                  <xsd:element name="name" type="cmn:StringLength1to64Type" minOccurs="1" maxOccurs="1">
                    <xsd:annotation>
                      <xsd:documentation>The name of the operation as exposed on the API.</xsd:documentation>
                    </xsd:annotation>
                  </xsd:element>
                  <xsd:element name="description" type="xsd:string" minOccurs="1" maxOccurs="1">
                    <xsd:annotation>
                      <xsd:documentation xml:lang="en">Describes the purpose of the
                                            operation.</xsd:documentation>
                    </xsd:annotation>
                  </xsd:element>
                  <xsd:element name="inputParameters" minOccurs="0" maxOccurs="1">
                    <xsd:annotation>
                      <xsd:documentation xml:lang="en">Describes the input paramters of the
                                            operation. This is most commonly
                                            used to provide a list of allowed or
                                            supported values for a given
                                            parameter (e.g., address kind).</xsd:documentation>
                    </xsd:annotation>
                    <xsd:complexType>
                      <xsd:sequence>
                        <xsd:element name="parameter" type="cmn:AttributeType" minOccurs="1" maxOccurs="unbounded"/>
                      </xsd:sequence>
                    </xsd:complexType>
                  </xsd:element>
                  <xsd:element name="outputParameters" minOccurs="0" maxOccurs="1">
                    <xsd:annotation>
                      <xsd:documentation xml:lang="en">Describes the output paramters of
                                            the operation. This is most commonly
                                            used to provide a list of expected
                                            values for a given parameter (e.g.,
                                            address kind).</xsd:documentation>
                    </xsd:annotation>
                    <xsd:complexType>
                      <xsd:sequence>
                        <xsd:element name="parameter" type="cmn:AttributeType" minOccurs="1" maxOccurs="unbounded"/>
                      </xsd:sequence>
                    </xsd:complexType>
                  </xsd:element>
                </xsd:sequence>
              </xsd:complexType>
            </xsd:element>
          </xsd:sequence>
        </xsd:complexType>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="StayIdType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Unique identifier to identify a specific
                                    Stay.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="id" type="cmn:StringLength1to32Type" minOccurs="1" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="TaxesType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A collection of various taxes with a total.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="tax" type="cmn:TaxType" minOccurs="0" maxOccurs="99">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">An individual tax.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="totalTax" type="cmn:MoneyType" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Used to provide a total of all the taxes.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element ref="cmn:currencyCode" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Provides a currency code to reflect the
                                      currency in which an amount may be
                                      expressed .</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="TaxIdsType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A collection of tax identifiers.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="taxId" type="cmn:TaxIdType" minOccurs="1" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="TaxIdType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">An identifier used for taxing purposes.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="id" type="cmn:StringLength1to64Type" minOccurs="1" maxOccurs="1"/>
    </xsd:sequence>
    <xsd:attribute name="kind" type="cmn:TaxIdKindType" use="optional"/>
  </xsd:complexType>
  <xsd:complexType name="TaxType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A tax that may be applied to a business
                                    transaction.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="name" type="cmn:StringLength1to32Type" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Name of the tax. The name or the code is
                                      required.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="code" type="cmn:StringLength1to16Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Code identifying the fee (e.g.,agency fee,
                                      municipality fee). The name or the code is
                                      required.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="description" type="cmn:StringLength1to255Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Text description of the taxes in a given
                                      language.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:choice>
        <xsd:element ref="cmn:money" minOccurs="0" maxOccurs="1">
          <xsd:annotation>
            <xsd:documentation xml:lang="en">Provides the amount for the fee or tax.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <xsd:element name="percent" type="cmn:PercentType" minOccurs="0" maxOccurs="1">
          <xsd:annotation>
            <xsd:documentation xml:lang="en">Fee percentage is optional and is for
                                       reference only.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
      </xsd:choice>
      <xsd:element name="frequency" type="cmn:ChargeUnitType" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Defines when and how this tax is applied.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="effectiveDateRange" type="cmn:DateSpanType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The inclusive date range in which this tax is in
                                      effect.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="TravelAgentIdType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Unique identifier to identify a specific
                                    travel agent account.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="id" type="cmn:StringLength1to32Type" minOccurs="1" maxOccurs="1"/>
    </xsd:sequence>
    <xsd:attribute name="issuingAuthority" type="cmn:StringLength1to32Type" use="optional">
      <xsd:annotation>
        <xsd:documentation>Authority that issued the id (e.g., IATA, CLIA, TRUE, ARC)</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
  </xsd:complexType>
  <xsd:complexType name="UniqueIdType">
    <xsd:sequence>
      <xsd:element name="id" type="cmn:StringLength1to64Type" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">A unique identifying value assigned by the
                                      creating system. The ID attribute may be
                                      used to reference a primary-key value
                                      within a database or a key in a particular
                                      implementation.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="companyName" type="cmn:StringLength1to64Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Identifies the external company that is
                                      associated with the UniqueID.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="context" type="cmn:StringLength1to32Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Used to identify the source system of the
                                      identifier (e.g., IATA, CRS, PMS, RMS).</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="sourceTimeStamp" type="xsd:dateTime" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Timestamp of when the record was created
                                      in the source system.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="UrlsType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Represents the set of URLs.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="url" type="cmn:UrlType" minOccurs="0" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="UserAuthenticationType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">The state of a user's access to a resource.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="authenticated" type="xsd:boolean" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The user was successfully authenticated.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="message" type="cmn:StringLength1to255Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">An authentication related message. This
                                      may contain acceptable use warnings or
                                      authentication error messages.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="UserCredentialsType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">The credentials provided by a user to gain
                                    access to a resource.</xsd:documentation>
    </xsd:annotation>
    <xsd:attribute name="username" type="cmn:UsernameType" use="required"/>
    <xsd:attribute name="password" type="cmn:PasswordType" use="optional"/>
    <xsd:attribute name="passwordEncrypted" type="xsd:boolean" use="optional"/>
    <xsd:attribute name="applicationInstanceId" type="cmn:ApplicationInstanceIdType" use="optional"/>
    <xsd:attribute name="clientReferral" type="cmn:ClientAuthenticationReferralType" use="optional"/>
  </xsd:complexType>
  <xsd:complexType name="UserType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Describes an application user. This may be a
                                    real person or a process.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="id" type="cmn:StringLength1to128Type" maxOccurs="1" minOccurs="1">
        <xsd:annotation>
          <xsd:documentation>User identifier. This may be the user's ID (e.g., the
                        uid attribute in LDAP) or some other identifier used for
                        authentication.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="name" type="cmn:StringLength1to64Type" maxOccurs="1" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation>User name. This may be the user's name (e.g., the cn
                        attribute in LDAP) or the process name assigned by an
                        application.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="location" type="cmn:StringLength1to32Type" maxOccurs="1" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation>User location. This is the user's physical location
                        (e.g., the l attribute in LDAP).</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="WaypointsType">
    <xsd:sequence>
      <xsd:element name="waypoint" type="cmn:WaypointType" maxOccurs="unbounded" minOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="WaypointType">
    <xsd:sequence>
      <xsd:element name="location" type="cmn:GeographicPointType" maxOccurs="1" minOccurs="1"/>
      <xsd:element name="name" type="xsd:string" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation>The name of the location of this waypoint.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <!--AttributeGroups go below here-->
  <xsd:attributeGroup name="ChargeUnitGroup">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Specifies charge information by unit (e.g.,
                                    room, person, item) and frequency (e.g.,
                                    daily, weekly, stay).</xsd:documentation>
    </xsd:annotation>
    <xsd:attribute name="chargeUnit" type="cmn:ChargeUnitType" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">This is the unit for which the charge
                                     applies (e.g. room, person, seat). Refer to
                                     OpenTravel Code List Charge Type (CHG).</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
    <xsd:attribute name="chargeFrequency" type="cmn:ChargeUnitType" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">This is the timeframe used to apply the
                                     charge during the course of the reservation
                                     (e.g. Daily, Weekly, Stay).</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
    <xsd:attribute name="chargeUnitExempt" type="xsd:positiveInteger" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">Number of units permitted before charges
                                     are applied (e.g., more than 4 persons).</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
    <xsd:attribute name="chargeFrequencyExempt" type="xsd:positiveInteger" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">ChargeFrequency exemptions before charges
                                     are applied (e.g. after 2 nights).</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
    <xsd:attribute name="maxChargeUnitApplies" type="xsd:positiveInteger" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">Maximum number of Units for which the
                                     charge will be applied (e.g., waive charges
                                     above 10 rooms).</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
    <xsd:attribute name="maxChargeFrequencyApplies" type="xsd:positiveInteger" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">Maximum number of times the charge will be
                                     applied (e.g. waive charges above 30
                                     nights).</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
  </xsd:attributeGroup>
  <xsd:attributeGroup name="locale">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A LocaleType represents a specific
                                    geographical, political, or cultural region.</xsd:documentation>
    </xsd:annotation>
    <xsd:attribute name="language" type="cmn:LanguageCodeType" use="required">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">These codes are the lower-case, two-letter
                                     codes as defined by ISO-639-1.</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
    <xsd:attribute name="country" type="cmn:CountryCodeType" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">These codes are the upper-case, two-letter
                                     codes as defined by ISO-3166-1 alpha 2.</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
    <xsd:attribute name="variant" type="cmn:StringLength1to32Type" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">The variant argument is an application
                                     specific code. If there are two variants,
                                     separate them with an underscore, and put
                                     the most important one first. For example,
                                     a Traditional Spanish collation might
                                     construct a locale with parameters for
                                     language, country and variant as: "es",
                                     "ES", "Traditional_WIN".</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
  </xsd:attributeGroup>
</xsd:schema>]]></con:content>
        <con:type>http://www.w3.org/2001/XMLSchema</con:type>
      </con:part>
      <con:part>
        <con:url>http://esb.services.ext.pci.qa.chotel.com:80/HotelDistributionService/v6?SCHEMA%2FCdm_Shared_v6%2Fxsd%2Fcommon%2FSimpleTypes</con:url>
        <con:content><![CDATA[<!--Document: The SimpleTypes schema contains only simple types that are used
          by multiple canonical schemas. They are used to put restrictions
          on elements.

Date: 12-10-2010
Last Updated:  07-20-2015
Authors: Chris Judson, Kirk Damron, Charlie Taylor, Datta Parupudi, Jared Sherrill, Andrew Baker, Maddy Lakshmanan, Jim Conger-->
<xsd:schema targetNamespace="http://www.choicehotels.com/schema/v6/common/cdm" elementFormDefault="qualified" attributeFormDefault="unqualified" xml:lang="en" xmlns:cmn="http://www.choicehotels.com/schema/v6/common/cdm" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <xsd:element name="countryCode" type="cmn:CountryCodeType"/>
  <xsd:element name="emailAddressFormat" type="cmn:EmailAddressFormatType"/>
  <xsd:element name="languageCode" type="cmn:LanguageCodeType"/>
  <xsd:element name="stateOrProvince" type="cmn:StateProvinceType"/>
  <xsd:simpleType name="AlphaNumericStringLength1to19Type">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Used forAlpha-Numeric Strings, length 1 to
                                    19.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:string">
      <xsd:pattern value="[0-9a-zA-Z]{1,19}"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="ApplicationInstanceIdType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">The id associated with a specific end user's application. 
                                    For mobile apps, the application id may be one generated 
                                    by the native OS for the application. For other applications,
                                    such as browsers, the id may be generated centrally and 
                                    saved in a cookie or local storage.
                                    Each install of an application will have its own unique id. 
                                    The id can be useful as a factor for authenticating
                                    the end user making requests to central systems.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to128Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="AreaUnitOfMeasureType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Describes the units an area measurement
                                    (e.g., Square Feet, Square Meters, Acres).</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to32Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="AttributeKindType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Classifies an attribute. This is useful when grouping
                                    the attributes as in an acceptable values list.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to64Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="ChargeUnitType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Describes how a given fee is charged
                                    (e.g., Per Week, Per Day, Per Hour, Per Room,
                                    Per Person, Per Stay, Per Reservation, Per Occurrence,
                                    Per Room Per Stay, Per Room Per Night,
                                    Per Person Per Stay, Per Person Per Night,
                                    One Time Use).</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to32Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="ClientAuthenticationReferralType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Opaque value signifying at least 1  
   authentication factor has been verified for an end user.  The details of this
   value are deliberately vague, allowing the authentication mechanism to 
   evolve over time.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:string"/>
  </xsd:simpleType>
  <xsd:simpleType name="CompassPointType">
    <xsd:restriction base="xsd:string">
      <xsd:enumeration value="North"/>
      <xsd:enumeration value="South"/>
      <xsd:enumeration value="East"/>
      <xsd:enumeration value="West"/>
      <xsd:enumeration value="Southwest"/>
      <xsd:enumeration value="Southeast"/>
      <xsd:enumeration value="Northwest"/>
      <xsd:enumeration value="Northeast"/>
      <xsd:enumeration value="NorthNorthwest"/>
      <xsd:enumeration value="NorthNortheast"/>
      <xsd:enumeration value="SouthSouthwest"/>
      <xsd:enumeration value="SouthSoutheast"/>
      <xsd:enumeration value="EastNortheast"/>
      <xsd:enumeration value="EastSoutheast"/>
      <xsd:enumeration value="WestNorthwest"/>
      <xsd:enumeration value="WestSouthwest"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="ConditionalNameType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">The name of a condition</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to64Type"></xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="ContextIdType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Identifier that is used to reference state 
                                    maintained across multiple invocations. For
                                    example, a hotel reservation may be built
                                    over several service invocations. This
                                    identifier provides a means for the client
                                    to inform the service that the current
                                    invocation is part of a series of
                                    invocations and provides a means for the
                                    service to manage state across those
                                    invocations. This is not a means for
                                    handling distributed transactions.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to64Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="CountryCodeType">
    <xsd:annotation>
      <xsd:documentation>The country that this listing is located in. The value
                      must be a ISO 3166 uppercase 2-letter country code
                      (http://www.iso.org/iso/en/prods-services/iso3166ma/02iso-3166-code-lists/list-en1.html).
                      For example, United States is US and Canada is CA.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:string">
      <xsd:pattern value="[A-Z]{2}"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="CountryIso3CodeType">
    <xsd:annotation>
      <xsd:documentation>The ISO 3166 uppercase 3-letter country code.
                      (http://en.wikipedia.org/wiki/ISO_3166-1_alpha-3). For
                      example, United States is USA and Canada is CAN.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:string">
      <xsd:pattern value="[A-Z]{3}"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="CountrySubdivisionCodeType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A subdivision is the first level of
                                    demarcation under a country (i.e.
                                    state/province/district) as defined in the
                                    ISO 3166-2 standard. This code includes the
                                    country code and '-' in front of it (i.e.
                                    US-AZ, MX-JAL).</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to8Type">
      <xsd:pattern value="[A-Z]{2}-[A-Z0-9]{1,3}"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="CountrySubdivisionKindType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Specifies the type of subdivision. 
            (e.g. County, State, or Province)</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to32Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="CurrencyCodeType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">The alpha-3 currency code as defined by ISO
                                    4217.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:string">
      <xsd:pattern value="[A-Z]{3}"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="DayOfWeekType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A three letter abbreviation for the days of
                                    the week (e.g. may be the starting day for
                                    the availability requested, days of
                                    operation, rate effective day, etc.).</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:string">
      <xsd:enumeration value="Mon"/>
      <xsd:enumeration value="Tue"/>
      <xsd:enumeration value="Wed"/>
      <xsd:enumeration value="Thu"/>
      <xsd:enumeration value="Fri"/>
      <xsd:enumeration value="Sat"/>
      <xsd:enumeration value="Sun"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="DirectionType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Direction, in degrees, from due North in a
                                    clockwise direction.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:double">
      <xsd:minInclusive value="0.0"/>
      <xsd:maxInclusive value="360.0"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="DistanceUnitOfMeasureType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Describes the units of a distance measurement
                                   (e.g., Inches, Feet, Yards, Miles, Millimeters,
                                   Centimeters, Meters, Kilometers).</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to32Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="EmailAddressFormatType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A restriction specifying a well-formed email
                                    address.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:string">
      <xsd:minLength value="6"/>
      <xsd:maxLength value="256"/>
      <xsd:pattern value="(.)+@(.)+\.([^\.])+"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="GuaranteeKindCodeType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Describes the guarantee method used for a reservation
                                    (e.g., Cash, Direct Bill, Voucher, Credit Card,
                                    Debit Card, Check, Loyalty Points, PrePay, Deposit,
                                    Travel Agent, Hold Time, None).</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to32Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="IATACodeType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:string">
      <xsd:length value="8"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="IATACityCodeType">
    <!--TODO remove in CDM 7-->
    <xsd:annotation>
      <xsd:documentation xml:lang="en">** DEPRECATED **
                                    Use IATALocationCodeType instead.
                                    The 3 letter code that identifies the IATA Airport
                                    code.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:string">
      <xsd:length value="3"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="IATALocationCodeType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">The 3 letter IATA code that identifies an airport or a
                                    city (e.g., PHX, ORD)</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:string">
      <xsd:length value="3"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="IATALocationKindType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A string that identifies the kind of IATA location
                                    (possible values are Airport, City etc.)</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to16Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="InternationalDirectDialingCodeType">
    <xsd:annotation>
      <xsd:documentation>The country calling codes defined by ITU-T recommendations
                      E.123 and E.164, also called IDD (International Direct
                      Dialing)</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:integer">
      <xsd:minInclusive value="1"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="IPAddressType">
    <xsd:annotation>
      <xsd:documentation>This type is constrained to match IPv4 addresses, 
    				   it may be extended in the future to include IPv6 
    				   in the future.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:string">
      <xsd:pattern value="^([01]?\d\d?|2[0-4]\d|25[0-5])\.([01]?\d\d?|2[0-4]\d|25[0-5])\.([01]?\d\d?|2[0-4]\d|25[0-5])\.([01]?\d\d?|2[0-4]\d|25[0-5])$"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="LanguageCodeType">
    <xsd:annotation>
      <xsd:documentation>The language used in this feed. The value must be an ISO
                      639 lowercase 2-letter language code
                      (http://www.w3.org/WAI/ER/IG/ert/iso639.htm#2letter). For
                      example English is en, French is fr.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:language">
      <xsd:pattern value="[a-z]{2}"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="LatitudeType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">For example, the latitude for 1600
                                    Amphitheatre Parkway, Mountain View, CA
                                    94043 is 37.423738</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:decimal">
      <xsd:minInclusive value="-90.0"/>
      <xsd:maxInclusive value="90.0"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="LongitudeType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">For example, the longitude for 1600
                                    Amphitheatre Parkway, Mountain View, CA
                                    94043 is -122.090101</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:decimal">
      <xsd:minInclusive value="-180.0"/>
      <xsd:maxInclusive value="180.0"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="MMDDDateType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Month and day parts of a date separated by a
                                    forward slash.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:string">
      <xsd:pattern value="(0[1-9]|1[0-2])/(0[1-9]|[12][0-9]|3[01])"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="MMYYDateType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Month and year parts of a date separated by
                                    a forward slash.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:string">
      <xsd:pattern value="(0[1-9]|1[0-2])/[0-9][0-9]"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="MobileDeviceAddressType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">This is the endpoint of the device
                                    generated by a external vendor.
                                    For example, Amazon creates ARN for
                                    each device.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:string"/>
  </xsd:simpleType>
  <xsd:simpleType name="MoneyType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Specifies a monetary amount that is not
                                    localized, max 3 decimals.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:decimal">
      <xsd:fractionDigits value="3"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="NonNegativeDecimal">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Used for Numeric values, from 1 to 999
                                    inclusive.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:decimal">
      <xsd:minInclusive value="0"/>
      <xsd:fractionDigits value="6"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="NotificationMethodType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Describes the a notification method (e.g., Email,
                                    Standard Mail, Phone, SMS, MMS, Push Notification).</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to32Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="Numeric0to999Type">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Used for Numeric values, from 0 to 999
                                    inclusive.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:integer">
      <xsd:minInclusive value="0"/>
      <xsd:maxInclusive value="999"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="Numeric1to999Type">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Used for Numeric values, from 1 to 999
                                    inclusive.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:integer">
      <xsd:minInclusive value="1"/>
      <xsd:maxInclusive value="999"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="Numeric0to99Type">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Used for Numeric values, from 0 to 99
                                    inclusive.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:integer">
      <xsd:minInclusive value="0"/>
      <xsd:maxInclusive value="99"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="Numeric1to99Type">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Used for Numeric values, from 1 to 99
                                    inclusive.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:integer">
      <xsd:minInclusive value="1"/>
      <xsd:maxInclusive value="99"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="NumericStringLength1to3Type">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Used for Numeric Strings length 1 to 3.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:string">
      <xsd:pattern value="[0-9]{1,3}"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="NumericStringLength1to5Type">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Used for Numeric Strings, length 1 to 5.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:string">
      <xsd:pattern value="[0-9]{1,5}"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="NumericStringLength1to8Type">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Used for Numeric Strings, length 1 to 8.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:string">
      <xsd:pattern value="[0-9]{1,8}"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="NumericStringLength1to19Type">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Used for Numeric Strings, length 1 to 19.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:string">
      <xsd:pattern value="[0-9]{1,19}"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="OrganizationIdType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">The identifier that represents a specific
                                    organization within a multi-organization
                                    environment.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to32Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="OrganizationRelationshipKindType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Classifies a relationship to an organization.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to32Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="OTACodeType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Used for codes in the OpenTravel Code
                                    tables. Possible values of this pattern are
                                    1, 101, 101.EQP, or 101.EQP.X.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:string">
      <xsd:pattern value="[0-9A-Z]{1,3}(\.[A-Z]{3}(\.X){0,1}){0,1}"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="PasswordType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Represents a password used for authentication.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to128Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="PaymentCardCodeType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">The 2 letter code that identifies the credit
                                    card.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:string">
      <xsd:length value="2"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="PaymentCardTokenType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">The token string that represents a payment
                                    card.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to32Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="PercentType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Used for percentage values.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:decimal"/>
  </xsd:simpleType>
  <xsd:simpleType name="SICCodeType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A Standard Industrial Classification (SIC)
                                    code - used to classify companies by
                                    industry.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to4Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="StateProvinceType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Represents a subdivision of a country (e.g
                                    state, province, territory). This is used to
                                    complete an address that fits local
                                    standards. This could be the name (e.g.,
                                    Texas) or an ISO 3166-2 code (e.g., US-TX)
                                    or the subdivision part of the ISO 3166-2
                                    code (e.g., TX) or an abbreviation (e.g.,
                                    Tex).</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to64Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="StringLength1to4Type">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Used for Character Strings, length 1 to 4.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:string">
      <xsd:minLength value="1"/>
      <xsd:maxLength value="4"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="StringLength1to5Type">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Used for Character Strings, length 1 to 5.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:string">
      <xsd:minLength value="1"/>
      <xsd:maxLength value="5"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="StringLength1to8Type">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Used for Character Strings, length 1 to 8.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:string">
      <xsd:minLength value="1"/>
      <xsd:maxLength value="8"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="StringLength1to16Type">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Used for Character Strings, length 1 to 16.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:string">
      <xsd:minLength value="1"/>
      <xsd:maxLength value="16"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="StringLength1to32Type">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Used for Character Strings, length 1 to 32.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:string">
      <xsd:minLength value="1"/>
      <xsd:maxLength value="32"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="StringLength1to64Type">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Used for Character Strings, length 1 to 64.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:string">
      <xsd:minLength value="1"/>
      <xsd:maxLength value="64"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="StringLength1to128Type">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Used for Character Strings, length 1 to 128.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:string">
      <xsd:minLength value="1"/>
      <xsd:maxLength value="128"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="StringLength1to255Type">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Used for Character Strings, length 1 to 255.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:string">
      <xsd:minLength value="1"/>
      <xsd:maxLength value="255"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="StockSymbolType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Abbreviation used to uniquely identify
                                    shares of a particuar stock.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to8Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="TaxIdKindType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Distinguishes types of tax identifiers.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to32Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="TrackingIdType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Identifier that allows end-to-end tracking
                                    of the business transaction across
                                    synchronous service calls, asynchronous
                                    service calls, faults and message
                                    processing. This identifier is suitable for
                                    tracing a call chain for audit or
                                    troubleshooting purposes.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to64Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="TimeUnitType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Defines the unit in which the time is
                                    expressed (e.g. year, day, hour).</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:string">
      <xsd:enumeration value="Year"/>
      <xsd:enumeration value="Month"/>
      <xsd:enumeration value="Week"/>
      <xsd:enumeration value="Day"/>
      <xsd:enumeration value="Hour"/>
      <xsd:enumeration value="Minute"/>
      <xsd:enumeration value="Second"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="UuidType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Unique identifier as defined by the Open
                                    Software Foundation.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:string">
      <xsd:minLength value="1"/>
      <xsd:maxLength value="36"/>
      <xsd:pattern value="[0-9a-fA-F]{8}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{12}"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="UrlType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Represents a URL for a Web address.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:anyURI"/>
  </xsd:simpleType>
  <xsd:simpleType name="UsernameType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Represents a user's name or identifier.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to128Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="YYYYDateType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">4-digit year part of a date.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:string">
      <xsd:pattern value="[0-9]{4}"/>
    </xsd:restriction>
  </xsd:simpleType>
</xsd:schema>]]></con:content>
        <con:type>http://www.w3.org/2001/XMLSchema</con:type>
      </con:part>
      <con:part>
        <con:url>http://esb.services.ext.pci.qa.chotel.com:80/HotelDistributionService/v6?SCHEMA%2FCdm_Shared_v6%2Fxsd%2Fcommon%2FFaultTypes</con:url>
        <con:content><![CDATA[<!--Document: Represents the base error types to be used within Choice

Date: 01-21-2011
Last Updated: 05-16-2013
Authors: G Chang, Chris Judson-->
<xsd:schema targetNamespace="http://www.choicehotels.com/schema/v6/common/cdm" elementFormDefault="qualified" attributeFormDefault="unqualified" xml:lang="en" xmlns:cmn="http://www.choicehotels.com/schema/v6/common/cdm" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <xsd:include schemaLocation="http://esb.services.ext.pci.qa.chotel.com:80/HotelDistributionService/v6?SCHEMA%2FCdm_Shared_v6%2Fxsd%2Fcommon%2FSimpleTypes"/>
  <xsd:element name="businessFault" type="cmn:BusinessFaultType"/>
  <xsd:element name="technicalFault" type="cmn:TechnicalFaultType"/>
  <xsd:complexType name="BaseFaultHeaderType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Defines the header information that
                                       should be included in all faults</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="serviceName" type="cmn:StringLength1to64Type" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="trackingId" type="cmn:TrackingIdType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">This is the trackingId passed in the
                                           request header.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="contextId" type="cmn:ContextIdType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">This is the contextId passed in the
                                           request header.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="dateTime" type="xsd:dateTime" minOccurs="1" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="BaseFaultDetailType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Defines the details used in every fault.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="faultName" type="cmn:StringLength1to64Type" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="faultCode" type="cmn:StringLength1to16Type" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="description" type="xsd:string" minOccurs="0" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="BusinessFaultType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Defines the business fault which is used
                                       for things such as date range validations</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="header" type="cmn:BaseFaultHeaderType" maxOccurs="1"/>
      <xsd:element name="details">
        <xsd:complexType>
          <xsd:sequence>
            <xsd:element name="detail" maxOccurs="unbounded">
              <xsd:complexType>
                <xsd:complexContent>
                  <xsd:extension base="cmn:BaseFaultDetailType">
                    <xsd:sequence>
                      <xsd:element name="property" type="cmn:StringLength1to255Type" minOccurs="0" maxOccurs="1">
                        <xsd:annotation>
                          <xsd:documentation>The name of the parameter in error using dot and square bracket
                                      notation (as in Java) to qualify the parameter name (e.g.,
                                      guest.contactInfo.addressPreferences.otherAddress[0].line1)</xsd:documentation>
                        </xsd:annotation>
                      </xsd:element>
                    </xsd:sequence>
                  </xsd:extension>
                </xsd:complexContent>
              </xsd:complexType>
            </xsd:element>
          </xsd:sequence>
        </xsd:complexType>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="TechnicalFaultType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Defines the technical fault which is used
                                       for things such as database or network
                                       failure</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="header" type="cmn:BaseFaultHeaderType" maxOccurs="1"/>
      <xsd:element name="details">
        <xsd:complexType>
          <xsd:sequence>
            <xsd:element name="detail" maxOccurs="unbounded">
              <xsd:complexType>
                <xsd:complexContent>
                  <xsd:extension base="cmn:BaseFaultDetailType">
                    <xsd:sequence>
                      <xsd:element name="applicationName" type="cmn:StringLength1to32Type" minOccurs="0" maxOccurs="1">
                        <xsd:annotation>
                          <xsd:documentation xml:lang="en">Used to specify the
                                                           name of the
                                                           application that
                                                           threw the fault.</xsd:documentation>
                        </xsd:annotation>
                      </xsd:element>
                      <xsd:element name="stackTrace" type="xsd:string" minOccurs="0" maxOccurs="1"/>
                      <xsd:element name="type" type="cmn:StringLength1to64Type" minOccurs="0" maxOccurs="1">
                        <xsd:annotation>
                          <xsd:documentation xml:lang="en">The type can be used
                                                           to group faults
                                                           together (i.e.
                                                           database, network,
                                                           etc.)</xsd:documentation>
                        </xsd:annotation>
                      </xsd:element>
                    </xsd:sequence>
                  </xsd:extension>
                </xsd:complexContent>
              </xsd:complexType>
            </xsd:element>
          </xsd:sequence>
        </xsd:complexType>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
</xsd:schema>]]></con:content>
        <con:type>http://www.w3.org/2001/XMLSchema</con:type>
      </con:part>
      <con:part>
        <con:url>http://esb.services.ext.pci.qa.chotel.com:80/HotelDistributionService/v6?SCHEMA%2FCdm_Shared_v6%2Fxsd%2Fdistribution%2FHotelDistribution</con:url>
        <con:content><![CDATA[<!--Document: Definition of the Hotel entity.

Date: 11-10-2010
Last Updated: 03-07-2019
Authors: Charlie Taylor, Chris Judson, Kirk Damron, Datta Parupudi, Sachin Gidadhubli, Snigdha Majumdar-->
<xsd:schema targetNamespace="http://www.choicehotels.com/schema/v6/dist/cdm" elementFormDefault="qualified" attributeFormDefault="unqualified" xml:lang="en" xmlns:dst="http://www.choicehotels.com/schema/v6/dist/cdm" xmlns:cmn="http://www.choicehotels.com/schema/v6/common/cdm" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <xsd:import namespace="http://www.choicehotels.com/schema/v6/common/cdm" schemaLocation="http://esb.services.ext.pci.qa.chotel.com:80/HotelDistributionService/v6?SCHEMA%2FCdm_Shared_v6%2Fxsd%2Fcommon%2FCommonTypes"/>
  <xsd:include schemaLocation="http://esb.services.ext.pci.qa.chotel.com:80/HotelDistributionService/v6?SCHEMA%2FCdm_Shared_v6%2Fxsd%2Fdistribution%2FDistributionCommonTypes"/>
  <xsd:element name="auditableConfigurableHotelDistribution" type="dst:AuditableConfigurableHotelDistributionType"/>
  <xsd:element name="configurableHotelDistribution" type="dst:ConfigurableHotelDistributionType"/>
  <xsd:element name="destinations" type="dst:DestinationsType"/>
  <xsd:element name="faqCategories" type="dst:FaqCategoriesType"/>
  <xsd:element name="hotelAmenities" type="dst:HotelAmenitiesType"/>
  <xsd:element name="hotelAmenity" type="dst:HotelAmenityType"/>
  <xsd:element name="hotelAuditEntries" type="dst:HotelAuditEntriesType"/>
  <xsd:element name="hotelAuditTrailSearchCriteria" type="dst:HotelAuditTrailSearchCriteriaType"/>
  <xsd:element name="hotelDistribution" type="dst:HotelDistributionType"/>
  <xsd:element name="hotelDistributionSearchCriteria" type="dst:HotelDistributionSearchCriteriaType"/>
  <xsd:element name="hotelDistributionSearchResult" type="dst:HotelDistributionSearchResultType"/>
  <xsd:element name="hotelDistributionSummary" type="dst:HotelDistributionSummaryType"/>
  <xsd:element name="meetingRoom" type="dst:MeetingRoomType"/>
  <xsd:element name="meetingRooms" type="dst:MeetingRoomsType"/>
  <xsd:complexType name="AssociatedIATACitiesType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A collection of associated IATA cities.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="associatedIATACity" type="dst:AssociatedIATACityType" minOccurs="1" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="AssociatedIATACityType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Describes an association between a location
                                    (e.g., a hotel) and an IATA city.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="iataCityCode" type="cmn:IATACityCodeType" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The IATA City.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="distance" type="cmn:DistanceType" maxOccurs="1" minOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Distance to the IATA City.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="compassPointType" type="cmn:CompassPointType" maxOccurs="1" minOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Direction to the IATA City.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="AirportType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Represents an airport POI.</xsd:documentation>
    </xsd:annotation>
    <xsd:complexContent>
      <xsd:extension base="dst:LocalDestinationType"/>
    </xsd:complexContent>
  </xsd:complexType>
  <xsd:complexType name="AirportsType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Represents the set of airport POIs.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="airport" type="dst:AirportType" minOccurs="0" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="AlertType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Details pertaining to a Hotel alert message.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="id" type="xsd:integer" minOccurs="0" maxOccurs="1"/>
      <!--TODO set minOccurs="1" in CDM 7-->
      <xsd:element name="text" type="xsd:string" minOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">alert message description.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="date" type="cmn:DateTimeSpanType">
        <!--TODO rename to dateRange in CDM 7-->
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Date and time span of this alert.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="agentOnly" type="xsd:boolean">
        <!--TODO remove in CDM 7-->
        <xsd:annotation>
          <xsd:documentation xml:lang="en">*** DEPRECATED ***
                                      This data is unique to the agent UI application and
                                      will not be available going forward.
                                      
                                      Alert is for agent only.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="AlertsType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Represents the set of Hotel alert messages.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="alert" type="dst:AlertType" minOccurs="0" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="AlternateHotelNamesType">
    <xsd:sequence>
      <xsd:element name="GDSName" type="cmn:StringLength1to64Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The Hotel name encoded for GDS, that is,
                                      ASCII.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="legalNameExtension" type="cmn:StringLength1to64Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">A Hotel specific extension to the Hotel
                                      name.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="AttractionsType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Represents the set of attraction POIs.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="attraction" type="dst:AttractionType" minOccurs="0" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="AttractionType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Represents an attraction POI.</xsd:documentation>
    </xsd:annotation>
    <xsd:complexContent>
      <xsd:extension base="dst:LocalDestinationType">
        <xsd:sequence>
          <xsd:element name="callAheadRecommended" type="xsd:boolean" minOccurs="1" maxOccurs="1"/>
        </xsd:sequence>
      </xsd:extension>
    </xsd:complexContent>
  </xsd:complexType>
  <xsd:complexType name="AuditableConfigurableHotelDistributionType">
    <xsd:annotation>
      <xsd:documentation>Describes a hotel along with pertinent metadata necessary
                      to audit changes the hotel</xsd:documentation>
    </xsd:annotation>
    <xsd:complexContent>
      <xsd:extension base="dst:ConfigurableHotelDistributionType">
        <xsd:sequence>
          <xsd:element name="changeAudit">
            <xsd:annotation>
              <xsd:documentation>Describes the auditable aspects of the change to the
                          hotel</xsd:documentation>
            </xsd:annotation>
            <xsd:complexType>
              <xsd:sequence>
                <xsd:element ref="cmn:changeOriginator" minOccurs="1" maxOccurs="1">
                  <xsd:annotation>
                    <xsd:documentation>Describes who or what made the change to the hotel</xsd:documentation>
                  </xsd:annotation>
                </xsd:element>
                <xsd:element name="changeAuthorization">
                  <xsd:annotation>
                    <xsd:documentation>Describes the authorization vehicle for the hotel
                             change</xsd:documentation>
                  </xsd:annotation>
                  <xsd:complexType>
                    <xsd:sequence>
                      <xsd:element name="who" type="cmn:StringLength1to64Type" minOccurs="1" maxOccurs="1">
                        <xsd:annotation>
                          <xsd:documentation>Name of the person who authorized the change</xsd:documentation>
                        </xsd:annotation>
                      </xsd:element>
                      <xsd:element name="why" type="cmn:StringLength1to128Type" minOccurs="0" maxOccurs="1">
                        <xsd:annotation>
                          <xsd:documentation>Reason for the change</xsd:documentation>
                        </xsd:annotation>
                      </xsd:element>
                    </xsd:sequence>
                  </xsd:complexType>
                </xsd:element>
                <xsd:element name="timeStamp" type="xsd:dateTime" minOccurs="0" maxOccurs="1">
                  <xsd:annotation>
                    <xsd:documentation>Time when the change to the hotel occured</xsd:documentation>
                  </xsd:annotation>
                </xsd:element>
              </xsd:sequence>
            </xsd:complexType>
          </xsd:element>
        </xsd:sequence>
      </xsd:extension>
    </xsd:complexContent>
  </xsd:complexType>
  <xsd:complexType name="DestinationsType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Collection of all destination types.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="airports" type="dst:AirportsType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="attractions" type="dst:AttractionsType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="restaurants" type="dst:RestaurantsType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="lounges" type="dst:LoungesType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="institutions" type="dst:InstitutionsType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="transportations" type="dst:TransportationType" minOccurs="0" maxOccurs="1"/>
    </xsd:sequence>
    <xsd:attributeGroup ref="cmn:locale"/>
  </xsd:complexType>
  <xsd:complexType name="BuildingCapacitySummaryType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Building and room capacity related
                                    properties of the hotel.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="guestRooms" type="xsd:nonNegativeInteger" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Total number of rooms at the hotel.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="meetingRooms" type="xsd:nonNegativeInteger" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The total number of unique meeting rooms
                                      provided at the hotel.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="largestMeetingRoomSpace" type="cmn:AreaType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The amount of room space for the largest
                                      unique meeting room at the hotel.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="floors" type="xsd:nonNegativeInteger" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Total number of floors at the hotel which
                                      could include floors without guest rooms
                                      (i.e. pool, maintenance, etc.).</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="CheckInCheckOutPolicyType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Hotel check-in and check-out policy
                                    information.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="checkInTime" type="xsd:time" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The checkin time required by this hotel
                                      for a room stay.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="checkOutTime" type="xsd:time" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The checkout time required by this hotel
                                      for a room stay.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="ConfigurableHotelDistributionType">
    <xsd:sequence>
      <xsd:element ref="dst:hotelDistribution" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="configuration">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Contains the configuration metadata.</xsd:documentation>
        </xsd:annotation>
        <xsd:complexType>
          <xsd:sequence>
            <xsd:element name="hotelNameOverridden" type="xsd:boolean" minOccurs="1" maxOccurs="1">
              <xsd:annotation>
                <xsd:documentation xml:lang="en">Indicates whether or not the hotel name
                                         has been changed from the standard
                                         naming convention.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="reservationSource" type="cmn:StringLength1to32Type" minOccurs="0" maxOccurs="1">
              <xsd:annotation>
                <xsd:documentation xml:lang="en">Source of reservations for this hotel
                                         (e.g., CRS, ChoiceAdvantage).</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="minRateCeiling" type="xsd:boolean" minOccurs="0" maxOccurs="1">
              <xsd:annotation>
                <xsd:documentation xml:lang="en">A minimum rate ceiling is in effect for
                                         this hotel.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="employeeDiscountRateLoadLevel" type="dst:EmployeeDiscountRateLoadLevelType" minOccurs="0" maxOccurs="1"></xsd:element>
            <xsd:element ref="dst:coOpParticipationSet" minOccurs="0" maxOccurs="1"/>
            <xsd:element name="rateManagementStrategy" type="dst:RateManagementStrategyType" minOccurs="0" maxOccurs="1"/>
            <xsd:element name="contractExecuted" type="xsd:boolean" minOccurs="0" maxOccurs="1">
              <xsd:annotation>
                <xsd:documentation xml:lang="en">Indicates whether or not the franchise
                                         contract for this hotel has been
                                         executed.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="platformFeatures" type="cmn:AttributeFamilyType" minOccurs="0" maxOccurs="1">
              <xsd:annotation>
                <xsd:documentation xml:lang="en">Indicates what platform features are enabled/disabled
                                         for this hotel (e.g., AutoInventoryRollIn).</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
          </xsd:sequence>
        </xsd:complexType>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="ContactInfoType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Collection of contact information for the
                                    hotel property.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="hotelMailingAddress" type="cmn:AddressType" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Mailing address of the hotel property.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="hotelEmailAddresses" type="cmn:EmailAddressesType" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">e-mail address of the hotel property.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="contactNumbers" type="cmn:PhonesType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Contact numbers of the hotel property.
                                      Examples are telephone and fax numbers.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="emergencyContacts" minOccurs="0" maxOccurs="unbounded">
        <xsd:complexType>
          <xsd:complexContent>
            <xsd:extension base="cmn:PersonContactType">
              <xsd:sequence>
                <xsd:element name="title" type="cmn:StringLength1to32Type" minOccurs="0" maxOccurs="1">
                  <xsd:annotation>
                    <xsd:documentation>Title of the person in the context of an emergency
                             contact (e.g., Owner, General Manager, Assistant
                             Manager, Night Manager).</xsd:documentation>
                  </xsd:annotation>
                </xsd:element>
                <xsd:element name="sequence" type="xsd:short" minOccurs="1" maxOccurs="1">
                  <xsd:annotation>
                    <xsd:documentation>Specifies the order of preference for an emergency
                             contact.</xsd:documentation>
                  </xsd:annotation>
                </xsd:element>
              </xsd:sequence>
            </xsd:extension>
          </xsd:complexContent>
        </xsd:complexType>
      </xsd:element>
      <xsd:element name="urls" type="cmn:UrlsType" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">A set of URLs to websites containing hotel
                                      information.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="DescriptionsType">
    <xsd:sequence>
      <xsd:element name="description" type="dst:DescriptionType" minOccurs="0" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="DescriptionType">
    <xsd:sequence>
      <xsd:element name="kind" type="cmn:StringLength1to16Type" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="text" type="xsd:string" minOccurs="1" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="DrivingDirectionsType">
    <xsd:sequence>
      <xsd:element name="drivingDirection" type="dst:DrivingDirectionType" minOccurs="0" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="DrivingDirectionType">
    <xsd:sequence>
      <xsd:element name="kind" type="cmn:StringLength1to16Type" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="title" type="cmn:StringLength1to32Type" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="directions" type="xsd:string" minOccurs="1" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="FaqType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Represents a FAQ.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="question" type="xsd:string" minOccurs="0"/>
      <xsd:element name="answer" type="xsd:string" minOccurs="0"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="FaqCategoryType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Represents the set of FAQs.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="category" type="cmn:StringLength1to32Type" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="faq" type="dst:FaqType" minOccurs="0" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="FaqCategoriesType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Represents the set of FAQs.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="faqCategories" type="dst:FaqCategoryType" minOccurs="0" maxOccurs="unbounded"/>
    </xsd:sequence>
    <xsd:attributeGroup ref="cmn:locale"/>
  </xsd:complexType>
  <xsd:complexType name="GreenQuestionsType">
    <xsd:sequence>
      <xsd:element name="environmentalCertifications" type="xsd:string" minOccurs="0"/>
      <xsd:element name="environmentalPrograms" type="xsd:string" minOccurs="0"/>
      <xsd:element name="environmentalCertificateAvailable" type="xsd:boolean" minOccurs="0"/>
      <xsd:element name="recycleProgramAvailable" type="xsd:boolean" minOccurs="0"/>
      <xsd:element name="environmentalSafeCleanersUsed" type="xsd:boolean" minOccurs="0"/>
      <xsd:element name="waterConservationProgramAvailable" type="xsd:boolean" minOccurs="0"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="GroupAmenityPolicyType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Defines a group amenity policy.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="relatedAmenities" minOccurs="1" maxOccurs="1">
        <xsd:complexType>
          <xsd:sequence>
            <xsd:element name="relatedAmenity" minOccurs="1" maxOccurs="unbounded">
              <xsd:complexType>
                <xsd:complexContent>
                  <xsd:extension base="dst:AmenityType"/>
                </xsd:complexContent>
              </xsd:complexType>
            </xsd:element>
          </xsd:sequence>
        </xsd:complexType>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="GroupBaggagePolicyType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Defines the group baggage service provided by the
                                    hotel.</xsd:documentation>
    </xsd:annotation>
    <xsd:attribute name="conditions" type="dst:GroupBaggageConditionsType" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">Describles baggage service conditions for a group
                                     (e.g., available, not available or manadatory).</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
    <xsd:attribute name="charge" type="xsd:boolean" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">Indicates whether or not there is a charge for using
                                     the baggage service.</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
    <xsd:attribute name="chargeUnit" type="cmn:ChargeUnitType" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">This is the unit for which the charge
                                     applies (e.g. room, person, seat). Refer to
                                     OpenTravel Code List Charge Type (CHG).</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
    <xsd:attribute name="amount" type="cmn:NonNegativeDecimal" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">Describes the charges for baggage service</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
  </xsd:complexType>
  <xsd:complexType name="GroupComplimentaryRoomPolicyType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Defines the group complimentary room policy.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="complimentaryRoomRatio" type="dst:GroupComplimentaryRoomRatioType" minOccurs="1" maxOccurs="1"></xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="GroupComplimentaryRoomRatioType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Defines the number of complimentary rooms per rooms
                                    paid for a group. Example: 1:15 (1 complimentary room
                                    for every 15 paid rooms).</xsd:documentation>
    </xsd:annotation>
    <xsd:attribute name="complimentaryRooms" type="xsd:nonNegativeInteger" use="required">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">Number of complimentary rooms provided.</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
    <xsd:attribute name="paidRooms" type="xsd:nonNegativeInteger" use="required">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">Number of rooms paid.</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
  </xsd:complexType>
  <xsd:complexType name="GroupPoliciesType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A collection of Group Policies.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="groupPolicy" type="dst:GroupPolicyType" minOccurs="0" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="GroupPolicyType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Defines a policy for accepting groups at a hotel.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="baggagePolicy" type="dst:GroupBaggagePolicyType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="breakfastPolicy" type="dst:GroupAmenityPolicyType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="complimentaryRoomPolicy" type="dst:GroupComplimentaryRoomPolicyType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="parkingPolicy" type="dst:GroupAmenityPolicyType" minOccurs="0" maxOccurs="1"/>
    </xsd:sequence>
    <xsd:attribute name="groupKind" type="dst:GroupKindType" use="required">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">Specifies the type of group to which this policy
                                     applies.</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
    <xsd:attribute name="sellableTo18AndUnder" type="xsd:boolean" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">Indicates whether or not hotel will sell the room to ages 18 and under.</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
    <xsd:attribute name="separateSettlementAccepted" type="xsd:boolean" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">Indicates whether or not hotel will allow members of
                                     group to pay separately.</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
    <xsd:attribute name="separateArrivalAccepted" type="xsd:boolean" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">Indicates whether or not the hotel will allow members
                                     of group to arrive separately.</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
    <xsd:attribute name="childStayFree" type="xsd:boolean" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">Indicates whether or not the hotel will allow
                                     children to stay free when staying with an adult.</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
    <xsd:attribute name="welcomeReception" type="xsd:boolean" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">Indicates whether or not the hotel will provide
                                     welcome reception for the group.</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
  </xsd:complexType>
  <xsd:complexType name="HotelAmenityType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Represents a Hotel level amenity, for
                                    example, a swimming pool, concierge.</xsd:documentation>
    </xsd:annotation>
    <xsd:complexContent>
      <xsd:extension base="dst:AmenityType">
        <xsd:sequence>
          <xsd:element name="distanceFromHotel" type="cmn:ProximityType" minOccurs="0" maxOccurs="1"/>
        </xsd:sequence>
      </xsd:extension>
    </xsd:complexContent>
  </xsd:complexType>
  <xsd:complexType name="HotelAmenitiesType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Represents the set of Hotel amenities.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="amenity" type="dst:HotelAmenityType" minOccurs="1" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="HotelAuditEntryType">
    <xsd:annotation>
      <xsd:documentation>An abridged hotel audit entry.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="hotelId" type="cmn:HotelIdType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation>The hotelId for which the audit Entry
      is being returned.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="timeStamp" type="xsd:dateTime" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation>The time of the audit entry</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="changeOriginator" type="cmn:ChangeOriginatorType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation>Who or what made the change to the
      hotel</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="changeAuthorizor" type="cmn:StringLength1to64Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation>Name of the person who authorized the change.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="HotelAuditEntriesType">
    <xsd:annotation>
      <xsd:documentation>A collection of audit entries.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="hotelAuditEntry" type="dst:HotelAuditEntryType" minOccurs="0" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="HotelAuditTrailSearchCriteriaType">
    <xsd:annotation>
      <xsd:documentation>Criteria for searching audit entries</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="dateTimeSpan" type="cmn:DateTimeSpanType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation>The time range for which the audit
      entries are being requested</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="hotelId" type="cmn:HotelIdType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation>The hotelId for which the audit entries
      are being requested.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="hotelChangeKind" type="dst:HotelChangeKindType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation>The hotel change category for which the audit entries
      are being requested.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="amenityCode" type="dst:AmenityCodeType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation>The amenity code for which the search is to be performed</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="roomTypeCode" type="dst:RoomTypeCodeType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation>The room type code for which the search is to be performed</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="changeOriginator" type="cmn:ChangeOriginatorType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation>Who or what made the change to the
      hotel</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="changeAuthorizor" type="cmn:StringLength1to64Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation>Name of the person who authorized the change</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="HotelConfigurationParametersType">
    <!--TODO need to add more response elements for 
                                                                other hotel configurations like hotel names 
                                                                and default amenities-->
    <xsd:annotation>
      <xsd:documentation>Specifies the rule-based parameters needed to configure a hotel</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="nonSmokingMandatory" type="xsd:boolean" minOccurs="0" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="HotelDistributionSearchCriteriaType">
    <xsd:sequence>
      <xsd:element name="brandCodeList" minOccurs="0" maxOccurs="1">
        <xsd:complexType>
          <xsd:sequence>
            <xsd:element ref="cmn:brandCode" minOccurs="1" maxOccurs="unbounded"/>
          </xsd:sequence>
        </xsd:complexType>
      </xsd:element>
      <xsd:element name="productCodeList" minOccurs="0" maxOccurs="1">
        <xsd:complexType>
          <xsd:sequence>
            <xsd:element ref="cmn:productCode" minOccurs="1" maxOccurs="unbounded"/>
          </xsd:sequence>
        </xsd:complexType>
      </xsd:element>
      <xsd:element name="address" type="cmn:AddressSearchCriteriaType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="geographicMercatorRectangleArea" type="cmn:GeographicMercatorRectangleType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">This element allows you to search a
                                      rectangular area. NOT CURRENTLY SUPPORTED.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="geographicPolygonArea" minOccurs="0" maxOccurs="1" type="cmn:GeographicPolygonType">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">This element allows you to search a given
                                      area of any shape. NOT CURRENTLY SUPPORTED.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="geographicVicinityArea" type="cmn:GeographicVicinityType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="hotelAmenityPreferences" type="dst:HotelAmenityPreferencesType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="hotelIdList" minOccurs="0" maxOccurs="1">
        <xsd:complexType>
          <xsd:sequence>
            <xsd:element ref="cmn:hotelId" minOccurs="1" maxOccurs="unbounded"/>
          </xsd:sequence>
        </xsd:complexType>
      </xsd:element>
      <xsd:element name="hotelStatuses" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The status of the hotel (i.e. Active,
                                      Suspended, Terminated, etc.).</xsd:documentation>
        </xsd:annotation>
        <xsd:complexType>
          <xsd:sequence>
            <xsd:element ref="dst:hotelStatus" minOccurs="1" maxOccurs="unbounded"/>
          </xsd:sequence>
        </xsd:complexType>
      </xsd:element>
      <xsd:element name="roomAmenityPreferences" type="dst:RoomAmenityPreferencesType" maxOccurs="1" minOccurs="0"/>
      <xsd:element name="propertySystemTypeList" minOccurs="0" maxOccurs="1">
        <xsd:complexType>
          <xsd:sequence>
            <xsd:element name="propertySystemType" type="cmn:StringLength1to64Type" minOccurs="1" maxOccurs="unbounded"/>
          </xsd:sequence>
        </xsd:complexType>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="HotelDistributionSearchFilterType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">This filter enables a way to specify which
                                    elements of the HotelSummary should be
                                    populated on a search response. The standard
                                    behavior is to return a fully populated
                                    HotelSummary; clients must explicitly
                                    suppress elements they do not wish to
                                    receive in a search response.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="suppressAmenities" type="xsd:boolean" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">When 'true', do not return hotelAmenities
                                      and roomAmenities. Note that roomTypes are
                                      still returned unless explicitly
                                      suppressed.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="suppressRoomTypes" type="xsd:boolean" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">When 'true', do not return roomTypes.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="HotelDistributionSearchResultType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Represents a single search result element. A
                                    search result element is comprised a
                                    HotelDistributionSummary and its associated
                                    distance and direction from the search
                                    origin when the origin is a defined point
                                    (lat/long).</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element ref="dst:hotelDistributionSummary" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Hotel summary information.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="hotelDistanceFromOrigin" type="cmn:DistanceAndDirectionType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Distance and direction of this hotel from
                                      the origin of the seach.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="HotelDistributionSummaryType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">An abbreviated version of hotel information.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element ref="cmn:hotelReference" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The base hotel information including hotel
                                      code, name, brand, etc.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="alternateHotelNames" type="dst:AlternateHotelNamesType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">A text field used to communicate an
                                      abbreviated name of the hotel.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="businessAddress" type="cmn:AddressType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Public address of the hotel property.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="primaryPhoneNumber" type="cmn:PhoneType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The most commonly published phone number.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="effectiveDate" type="xsd:date" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Date this hotel became active for selling
                                      purposes.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="hotelEffectiveStatus" type="dst:HotelEffectiveStatusType" minOccurs="0"/>
      <xsd:element name="geoLocation" type="dst:GeographicLocationType" minOccurs="0"/>
      <xsd:element name="cityLocation" type="cmn:StringLength1to255Type" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Brief description of hotel location, for
                                      example, "close to downtown".</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="locationCode" type="dst:HotelLocationCodeType" minOccurs="0"/>
      <xsd:element name="IATACityCode" type="cmn:IATACityCodeType" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The IATA (International Air Transportation
                                      Association) city code; for example DCA,
                                      ORD.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="associatedIATACities" type="dst:AssociatedIATACitiesType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The set of IATA cities associted with this
                                      hotel.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="pointRedemptionTiers" type="dst:PointRedemptionTiersType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Point redemption details.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="currencyCode" type="cmn:CurrencyCodeType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The code specifying a monetary unit using
                                      ISO 4217, three alpha code.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="generalDescription" type="xsd:string" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="buildingCapacitySummary" type="dst:BuildingCapacitySummaryType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Building and room capacity related
                                      properties of the hotel.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="hotelAmenities" type="dst:HotelAmenitiesType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Hotel-level amenities (pool, etc).</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="timeZoneInfo" type="dst:TimeZoneInfoType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Offset in hours from GMT.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="ratings" type="dst:HotelRatingsType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="close" type="cmn:DateSpanType" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Date hotel is to be closed to
                                      distribution services.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="closureReason" type="dst:HotelClosureReasonType" minOccurs="0" maxOccurs="1"/>
    </xsd:sequence>
    <xsd:attribute name="coOpParticipant" type="xsd:boolean" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">Indicates whether or not hotel participates in CoOp Marketing Program.</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
    <xsd:attributeGroup ref="cmn:locale"/>
  </xsd:complexType>
  <xsd:complexType name="HotelDistributionType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Hotel property comprehensive information.</xsd:documentation>
    </xsd:annotation>
    <xsd:complexContent>
      <xsd:extension base="dst:HotelDistributionSummaryType">
        <xsd:sequence>
          <xsd:element name="descriptions" type="dst:DescriptionsType" minOccurs="0" maxOccurs="1">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">A text field used to communicate hotel
                                        descriptive information to channel
                                        partners.</xsd:documentation>
            </xsd:annotation>
          </xsd:element>
          <xsd:element name="alerts" type="dst:AlertsType" minOccurs="0" maxOccurs="1">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">Information that needs to be conveyed to
                                        the guest (e.g., "the pool is closed
                                        until 3/15" or "lobby is being
                                        renovated").</xsd:documentation>
            </xsd:annotation>
          </xsd:element>
          <xsd:element name="contactInfo" type="dst:ContactInfoType" minOccurs="0"/>
          <xsd:element ref="cmn:relatedOrganizations" minOccurs="0" maxOccurs="1"/>
          <xsd:element ref="dst:acceptedPaymentForms" minOccurs="0" maxOccurs="1"/>
          <xsd:element name="defaultLocale" type="cmn:LocaleType" minOccurs="0">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">Default locale to be used for this hotel
                                        which can be different from the country
                                        the hotel resides in.</xsd:documentation>
            </xsd:annotation>
          </xsd:element>
          <xsd:element name="drivingDirections" type="dst:DrivingDirectionsType" minOccurs="0">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">A text field used to communicate basic
                                        driving instructions for the hotel.</xsd:documentation>
            </xsd:annotation>
          </xsd:element>
          <xsd:element name="destinations" type="dst:DestinationsType" minOccurs="0"/>
          <xsd:element name="faqs" type="dst:FaqCategoriesType" minOccurs="0" maxOccurs="1">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">Used by call center agents to
                                        communicate hotel-specific infomation to
                                        prospective guests.</xsd:documentation>
            </xsd:annotation>
          </xsd:element>
          <xsd:element name="groupPolicies" type="dst:GroupPoliciesType" minOccurs="0" maxOccurs="1">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">Defines the group polices for this hotel.</xsd:documentation>
            </xsd:annotation>
          </xsd:element>
          <xsd:element name="hotelManagement" type="dst:HotelManagementType" minOccurs="0"/>
          <xsd:element name="childrenStayFree" type="xsd:boolean" minOccurs="0" maxOccurs="1">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">If true, children stay free.</xsd:documentation>
            </xsd:annotation>
          </xsd:element>
          <xsd:element name="maxAgeChildStaysFree" type="xsd:short" minOccurs="0" maxOccurs="1">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">The maximum age at which the child can
                                        stay for free.</xsd:documentation>
            </xsd:annotation>
          </xsd:element>
          <xsd:element name="generalPolicy" type="xsd:string" minOccurs="0" maxOccurs="1"/>
          <xsd:element name="petPolicy" type="cmn:StringLength1to255Type" minOccurs="0" maxOccurs="1"/>
          <xsd:element name="checkInCheckOutPolicy" type="dst:CheckInCheckOutPolicyType" minOccurs="0" maxOccurs="1"/>
          <xsd:element name="roomTypes" type="dst:RoomTypesType" minOccurs="0" maxOccurs="1">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">Room type information.</xsd:documentation>
            </xsd:annotation>
          </xsd:element>
          <xsd:element name="meetingRooms" type="dst:MeetingRoomsType" minOccurs="0">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">Hotel specific meeting room information.</xsd:documentation>
            </xsd:annotation>
          </xsd:element>
          <xsd:element name="fees" type="dst:FeesType" minOccurs="0">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">Recurring charges information.</xsd:documentation>
            </xsd:annotation>
          </xsd:element>
          <xsd:element name="losTiers" type="dst:LOSTiersType" minOccurs="0" maxOccurs="1">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">Length of stay tiers.</xsd:documentation>
            </xsd:annotation>
          </xsd:element>
          <xsd:element name="mlosStrategy" type="dst:MLOSStrategyType" minOccurs="0" maxOccurs="1">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">Minimum/Maximum length of stay strategy</xsd:documentation>
            </xsd:annotation>
          </xsd:element>
          <xsd:element name="greenQuestions" type="dst:GreenQuestionsType" minOccurs="0">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">Green properties for the hotel.</xsd:documentation>
            </xsd:annotation>
          </xsd:element>
          <xsd:element name="awards" minOccurs="0" maxOccurs="1">
            <xsd:complexType>
              <xsd:sequence>
                <xsd:element name="award" type="dst:HotelAwardType" minOccurs="1" maxOccurs="unbounded"/>
              </xsd:sequence>
            </xsd:complexType>
          </xsd:element>
          <xsd:element name="constructionDate" type="xsd:date" minOccurs="0" maxOccurs="1">
            <xsd:annotation xml:lang="en">
              <xsd:documentation>Date hotel construction completed.</xsd:documentation>
            </xsd:annotation>
          </xsd:element>
          <xsd:element name="openingDate" type="xsd:date" minOccurs="0" maxOccurs="1">
            <xsd:annotation xml:lang="en">
              <xsd:documentation>Date hotel opened for business.</xsd:documentation>
            </xsd:annotation>
          </xsd:element>
          <xsd:element name="openingKind" type="dst:HotelOpeningType" minOccurs="0" maxOccurs="1"/>
          <xsd:element name="refurbishInfo" type="dst:RefurbishInfoType" minOccurs="0" maxOccurs="1"/>
          <xsd:element name="propertySystemType" type="cmn:StringLength1to64Type" minOccurs="0">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">The Property Management System used at
                                        this hotel.</xsd:documentation>
            </xsd:annotation>
          </xsd:element>
          <xsd:element name="propertySystemIntegration" type="cmn:StringLength1to64Type" minOccurs="0" maxOccurs="1">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">The technology used to integrate from central
                                        systems to the property system (e.g., Siteminder,
                                        Talaria, EDI).</xsd:documentation>
            </xsd:annotation>
          </xsd:element>
          <xsd:element name="bookTillTimeForPreviousDay" type="xsd:time" minOccurs="0">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">Represents the time, past midnight, that
                                        will be honored when making reservations
                                        to be acredited to the previous day. For
                                        example, if the time is 2AM, then a
                                        reservation made at 1AM on Monday, June
                                        2nd will be counted as having been
                                        booked on Sunday, June 1st.</xsd:documentation>
            </xsd:annotation>
          </xsd:element>
          <xsd:element name="travelAgentTerms" type="dst:TravelAgentTermsType" minOccurs="0" maxOccurs="1">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">Represents the hotel specific terms for
                                        travel agents bookings.</xsd:documentation>
            </xsd:annotation>
          </xsd:element>
          <xsd:element name="taxInclusive" type="xsd:boolean" minOccurs="0" maxOccurs="1">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">If true, taxes are implicitly included
                                        in the rates.</xsd:documentation>
            </xsd:annotation>
          </xsd:element>
          <xsd:element name="taxes" type="cmn:TaxesType" minOccurs="0" maxOccurs="1">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">Taxes that may be added to the guest
                                        folio.</xsd:documentation>
            </xsd:annotation>
          </xsd:element>
          <xsd:element name="specialInventory" type="dst:SpecialInventoryType" minOccurs="0" maxOccurs="1"/>
          <xsd:element name="officeHours" type="cmn:OperatingScheduleType" minOccurs="0" maxOccurs="1">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">Schedule of on-site staffing who are available to address
                                        customer concerns.</xsd:documentation>
            </xsd:annotation>
          </xsd:element>
        </xsd:sequence>
      </xsd:extension>
    </xsd:complexContent>
  </xsd:complexType>
  <xsd:complexType name="HotelManagementType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Collection of contact information for the
                                    hotel property.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="generalManager" type="cmn:PersonContactType" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">General Manager of the hotel property.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="salesManager" type="cmn:PersonContactType" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Sales Manager of the hotel property.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="HotelEffectiveStatusType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Represents the current status of this hotel,
                                    e.g., "active","suspended" and when that
                                    status became effective.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element ref="dst:hotelStatus" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="effectiveDate" type="xsd:date">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The date this status went into effect.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="HotelRatingsType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A collection of hotel ratings.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="rating" type="dst:HotelRatingType" minOccurs="1" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="HotelRatingType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A rating of a hotel by a specific organization,
                                    product or process.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="name" type="cmn:StringLength1to64Type" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Name of the rating. This is typically the name of
                                      the organization providing the rating (e.g., AAA,
                                      HTI, Bazaarvoice) but it could also be a specific
                                      rating product or process name from an organization
                                      that offers multiple rating products.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="ratingValue" minOccurs="1" maxOccurs="1">
        <xsd:complexType>
          <xsd:sequence>
            <xsd:element name="value" type="cmn:StringLength1to16Type" minOccurs="1" maxOccurs="1">
              <xsd:annotation>
                <xsd:documentation xml:lang="en">Rating value achieved by the hotel
                                         (e.g., [1-5] for AAA, [1-10] for HTI,
                                         [Bronze, Silver, Gold] for some other
                                         org).</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="units" type="cmn:StringLength1to16Type" minOccurs="0" maxOccurs="1">
              <xsd:annotation>
                <xsd:documentation xml:lang="en">Units of the rating value (e.g., stars,
                                         points).</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="maxPossibleValue" type="cmn:StringLength1to16Type" minOccurs="0" maxOccurs="1">
              <xsd:annotation>
                <xsd:documentation xml:lang="en">Maximum possible rating value (e.g., 5 for AAA,
                                         10 for HTI, Gold for some other org).</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
          </xsd:sequence>
        </xsd:complexType>
      </xsd:element>
      <xsd:element name="reviewStatistics" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Statistics describing the set of reviews associated
                                      with this rating.</xsd:documentation>
        </xsd:annotation>
        <xsd:complexType>
          <xsd:sequence>
            <xsd:element name="recommendations" type="xsd:positiveInteger" minOccurs="0" maxOccurs="1">
              <xsd:annotation>
                <xsd:documentation xml:lang="en">Number of review responses indicating the
                                         reviewer would recommend the hotel to others.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="totalReviews" type="xsd:positiveInteger" minOccurs="0" maxOccurs="1">
              <xsd:annotation>
                <xsd:documentation xml:lang="en">Total number of review responses.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
          </xsd:sequence>
        </xsd:complexType>
      </xsd:element>
      <xsd:element name="likelyhoodToRecommend" type="cmn:PercentType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The likelyhood of this hotel to be
                                      recommended (LTR).</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="HotelTravelAgentCommissionType">
    <xsd:complexContent>
      <xsd:extension base="dst:CommissionType">
        <xsd:sequence>
          <xsd:element name="enabled" type="xsd:boolean" minOccurs="1" maxOccurs="1">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">Travel Agent commission enabled at this
                                        hotel.</xsd:documentation>
            </xsd:annotation>
          </xsd:element>
        </xsd:sequence>
      </xsd:extension>
    </xsd:complexContent>
  </xsd:complexType>
  <xsd:complexType name="InstitutionType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Represents an institution POI.</xsd:documentation>
    </xsd:annotation>
    <xsd:complexContent>
      <xsd:extension base="dst:LocalDestinationType"/>
    </xsd:complexContent>
  </xsd:complexType>
  <xsd:complexType name="InstitutionsType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Represents the set of institution POIs.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="institution" type="dst:InstitutionType" minOccurs="0" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="LocalDestinationType">
    <xsd:sequence>
      <xsd:element name="code" type="cmn:StringLength1to16Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Code for this destination (e.g. IATA
                                      airport code, attaction code, university
                                      code) which could be an offical code or a
                                      custom code.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="name" type="cmn:StringLength1to64Type" maxOccurs="1"/>
      <xsd:element name="description" type="xsd:string" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Description of this POI.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="sequence" type="xsd:short" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation>Specifies the order of preference for this destination.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="geographicLocation" type="cmn:GeographicPointType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="address" type="cmn:AddressType" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Two character State/Province code.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="phoneNumber" type="cmn:PhoneType" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Phone number for the destination.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="url" type="cmn:UrlType" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">URL for the destination.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="distanceFromHotel" type="cmn:DistanceType" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Distance from hotel.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="directionFromHotel" type="cmn:CompassPointType" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Compass direction from hotel.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="feeRequired" type="xsd:boolean" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">There is a charge associated with this POI.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="hoursOfOperation" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Hours that the restaurant is open. This
                                      collection allows for multiple open and
                                      close times throughout the day.</xsd:documentation>
        </xsd:annotation>
        <xsd:complexType>
          <xsd:sequence>
            <xsd:element name="operatingHours" type="cmn:OperatingHoursType" minOccurs="1" maxOccurs="unbounded"/>
          </xsd:sequence>
        </xsd:complexType>
      </xsd:element>
      <xsd:element name="transportationCodes" minOccurs="0" maxOccurs="1">
        <!--TODO remove in CDM 7-->
        <xsd:annotation>
          <xsd:documentation xml:lang="en">*** DEPRECATED ***
                                      Use transportationModes instead.
                                      
                                      A collection of transportation codes.</xsd:documentation>
        </xsd:annotation>
        <xsd:complexType>
          <xsd:sequence>
            <xsd:element name="code" type="cmn:StringLength1to16Type" minOccurs="1" maxOccurs="unbounded">
              <xsd:annotation>
                <xsd:documentation xml:lang="en">Code describing transportation options
                                         between the hotel and this destination.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
          </xsd:sequence>
        </xsd:complexType>
      </xsd:element>
      <xsd:element name="transportationModes" minOccurs="0" maxOccurs="1">
        <xsd:complexType>
          <xsd:sequence>
            <xsd:element name="transporationMode" minOccurs="1" maxOccurs="unbounded">
              <xsd:annotation>
                <xsd:documentation xml:lang="en">Describes an option for transporation between the
                                         hotel and this destination.</xsd:documentation>
              </xsd:annotation>
              <xsd:complexType>
                <xsd:sequence>
                  <xsd:element name="code" type="cmn:StringLength1to16Type" minOccurs="1" maxOccurs="1"/>
                  <xsd:element name="description" type="cmn:StringLength1to128Type" minOccurs="0" maxOccurs="1"/>
                  <xsd:element name="callAheadRecommended" type="xsd:boolean" minOccurs="0" maxOccurs="1">
                    <xsd:annotation>
                      <xsd:documentation xml:lang="en">Recommend calling ahead.</xsd:documentation>
                    </xsd:annotation>
                  </xsd:element>
                  <xsd:element name="feeRequired" type="xsd:boolean" minOccurs="0" maxOccurs="1">
                    <xsd:annotation>
                      <xsd:documentation xml:lang="en">Indicates if there is a charge associated.</xsd:documentation>
                    </xsd:annotation>
                  </xsd:element>
                  <xsd:element name="hoursOfOperation" minOccurs="0" maxOccurs="1">
                    <xsd:annotation>
                      <xsd:documentation xml:lang="en">Hours that the mode of transportation is open. This
                                      collection allows for multiple open and
                                      close times throughout the day.</xsd:documentation>
                    </xsd:annotation>
                    <xsd:complexType>
                      <xsd:sequence>
                        <xsd:element name="operatingHours" type="cmn:OperatingHoursType" minOccurs="1" maxOccurs="unbounded"/>
                      </xsd:sequence>
                    </xsd:complexType>
                  </xsd:element>
                </xsd:sequence>
              </xsd:complexType>
            </xsd:element>
          </xsd:sequence>
        </xsd:complexType>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="LOSTierType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Represents a length of stay tier.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="level" type="xsd:nonNegativeInteger" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">LOS level.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="min" type="xsd:nonNegativeInteger" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Minimum LOS for this tier.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="max" type="xsd:nonNegativeInteger" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Maximum LOS for this tier.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
    <xsd:attribute name="active" type="xsd:boolean"/>
  </xsd:complexType>
  <xsd:complexType name="LOSTiersType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Represents the set of length of stay tiers.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="losTier" type="dst:LOSTierType" minOccurs="0" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="LoungeType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Represents a lounge POI.</xsd:documentation>
    </xsd:annotation>
    <xsd:complexContent>
      <xsd:extension base="dst:LocalDestinationType">
        <xsd:sequence>
          <xsd:element name="dancingAvailable" type="xsd:boolean"/>
          <xsd:element name="foodAvailable" type="xsd:boolean"/>
          <xsd:element name="entertainmentAvailable" type="xsd:boolean"/>
          <xsd:element name="locationRelativeToHotel" type="cmn:StringLength1to32Type">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">Allows for short description of relative
                                        location (i.e. In Hotel, Across the
                                        Street, On Corner).</xsd:documentation>
            </xsd:annotation>
          </xsd:element>
        </xsd:sequence>
      </xsd:extension>
    </xsd:complexContent>
  </xsd:complexType>
  <xsd:complexType name="LoungesType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Represents the set of lounge POIs.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="lounge" type="dst:LoungeType" minOccurs="0" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="MeetingRoomAmenityType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Represents a meeting room level amenity, for
                                    example, AV equipment, catering.</xsd:documentation>
    </xsd:annotation>
    <xsd:complexContent>
      <xsd:extension base="dst:AmenityType"/>
    </xsd:complexContent>
  </xsd:complexType>
  <xsd:complexType name="MeetingRoomType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Details pertaining to a Hotel meeting room.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="code" type="cmn:StringLength1to16Type">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Meeting Room code.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="name" type="cmn:StringLength1to64Type" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Meeting Room name.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="description" type="xsd:string" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Meeting Room description.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="seatingCapacity" type="xsd:nonNegativeInteger" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Meeting Room maximum capacity.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="dimensions" type="cmn:DimensionType" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Details regarding the room dimensions.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="meetingRoomConfiguration" type="dst:MeetingRoomConfigurationType" minOccurs="0" maxOccurs="unbounded"/>
      <xsd:element name="amenities" type="dst:MeetingRoomAmenityType" minOccurs="0" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="MeetingRoomsType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Details pertaining to the set of Hotel
                                    meeting rooms.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="largestRoomSpace" type="cmn:AreaType" minOccurs="0">
        <!--TODO remove in CDM 7-->
        <xsd:annotation>
          <xsd:documentation xml:lang="en">*** DEPRECATED ***
                                      Use largestMeetingRoomSpace in buildingCapacitySummary instead.
                                      
                                      The amount of room space for the largest
                                      unique meeting room at the hotel.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="smallestRoomSpace" type="cmn:AreaType" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The amount of room space for the smallest
                                      unique meeting room at the hotel.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="totalRoomSpace" type="cmn:AreaType" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The total amount of unique room space
                                      provided at the hotel.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="largestSeatingCapacity" type="xsd:nonNegativeInteger" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The largest seating capacity available in
                                      the largest meeting room.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="smallestSeatingCapacity" type="xsd:nonNegativeInteger" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The smallest seating capacity available in
                                      a meeting room.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="totalSeatingCapacity" type="xsd:nonNegativeInteger" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The total seating capacity available at
                                      the hotel.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="largestConferenceCapacity" type="xsd:nonNegativeInteger" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The total seating capacity for a conference
                                      available at the hotel.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="largestBanquetCapacity" type="xsd:nonNegativeInteger" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The total seating capacity for a banquet
                                      available at the hotel.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="largestRoomHeight" type="cmn:DistanceType" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The ceiling height of the largest meeting
                                      room.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="meetingRoom" type="dst:MeetingRoomType" minOccurs="0" maxOccurs="unbounded"/>
    </xsd:sequence>
    <xsd:attributeGroup ref="cmn:locale"/>
  </xsd:complexType>
  <xsd:complexType name="MeetingRoomConfigurationType">
    <xsd:sequence>
      <xsd:element name="code" type="cmn:StringLength1to16Type">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Room configuration code.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="name" type="cmn:StringLength1to64Type">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Room configuration name.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="seatingCapacity" type="xsd:nonNegativeInteger">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Maximum capacity for this configuration.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="RefurbishInfoType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Represents information regarding the last
                                    refurbishment of the hotel.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="year" type="xsd:int" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Year of hotel refurbishment.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="refurbishDate" type="xsd:date" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Date of hotel refurbishment.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="percentage" type="cmn:PercentType" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Percentage of total rooms refurbished.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="extent" type="dst:RefurbishExtentType" minOccurs="0"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="RestaurantType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Represents a restaurant POI.</xsd:documentation>
    </xsd:annotation>
    <xsd:complexContent>
      <xsd:extension base="dst:LocalDestinationType">
        <xsd:sequence>
          <xsd:element name="breakfastAvailable" type="xsd:boolean" minOccurs="0" maxOccurs="1"/>
          <xsd:element name="lunchAvailable" type="xsd:boolean" minOccurs="0" maxOccurs="1"/>
          <xsd:element name="dinnerAvailable" type="xsd:boolean" minOccurs="0" maxOccurs="1"/>
          <xsd:element name="callAheadRecommended" type="xsd:boolean" minOccurs="0" maxOccurs="1">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">Recommend calling ahead.</xsd:documentation>
            </xsd:annotation>
          </xsd:element>
          <xsd:element name="locationRelativeToHotel" type="cmn:StringLength1to32Type" minOccurs="0">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">Allows for short description of relative
                                        location (i.e. In Hotel, Across the
                                        Street, On Corner).</xsd:documentation>
            </xsd:annotation>
          </xsd:element>
          <xsd:element name="restaurantSpecialities" minOccurs="0" maxOccurs="1">
            <xsd:complexType>
              <xsd:sequence>
                <xsd:element name="restaurantSpeciality" minOccurs="1" maxOccurs="unbounded">
                  <xsd:annotation>
                    <xsd:documentation xml:lang="en">Restaurant specialties clasifies restaurants, ie. Mexican, Italian.</xsd:documentation>
                  </xsd:annotation>
                  <xsd:complexType>
                    <xsd:sequence>
                      <xsd:element name="code" type="cmn:StringLength1to16Type" minOccurs="1" maxOccurs="1"/>
                      <xsd:element name="description" type="cmn:StringLength1to128Type" minOccurs="0" maxOccurs="1"/>
                    </xsd:sequence>
                  </xsd:complexType>
                </xsd:element>
              </xsd:sequence>
            </xsd:complexType>
          </xsd:element>
        </xsd:sequence>
      </xsd:extension>
    </xsd:complexContent>
  </xsd:complexType>
  <xsd:complexType name="RestaurantsType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Represents the set of restaurant POIs.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="restaurant" type="dst:RestaurantType" minOccurs="0" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="RoomTypeSummariesType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Represents the set of Room Types.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="roomTypeSummary" type="dst:RoomTypeSummaryType" minOccurs="1" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="SpecialInventoryItemType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Descibes an item of special inventory that
                                    may be available at a hotel.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="id" type="cmn:UniqueIdType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="name" type="cmn:StringLength1to32Type" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="count" type="xsd:nonNegativeInteger" minOccurs="0" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="SpecialInventoryType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Descibes the special inventory that may be
                                    available at a hotel. This reprents things
                                    that have limited quantities but are not
                                    tracked with the same controls used for room
                                    inventory (e.g., cribs, roll-away beds,
                                    refrigerators).</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="items" type="dst:SpecialInventoryItemType" minOccurs="1" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="TimeZoneInfoType">
    <xsd:sequence>
      <xsd:element name="GMTOffset" type="xsd:integer" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Offset in minutes from GMT.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="timezoneLocation" type="cmn:StringLength1to16Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The name of the timezone (i.e. Pacific,
                                      Eastern, etc.).</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="observesDaylightSavingsTime" type="xsd:boolean" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Whether or not the timezone observers
                                      daylight savings time.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="TransportLocationType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">This type represents a transportation
                                    location (i.e. a train station, ferry
                                    terminal, car rental, subway station, etc.).</xsd:documentation>
    </xsd:annotation>
    <xsd:complexContent>
      <xsd:extension base="dst:LocalDestinationType">
        <xsd:sequence>
          <xsd:element name="longDistance" type="xsd:boolean" minOccurs="1" maxOccurs="1"/>
        </xsd:sequence>
      </xsd:extension>
    </xsd:complexContent>
  </xsd:complexType>
  <xsd:complexType name="TransportationType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Represents the set of transportation POIs.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="transportation" type="dst:TransportLocationType" minOccurs="0" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="TravelAgentTermsType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Terms for travel agents who facilitate
                                    bookings at this hotel.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="travelAgentCommission" type="dst:HotelTravelAgentCommissionType" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="travelAgentGuaranteePeriod" type="cmn:DateSpanType" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Travel Agent guarantee period.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:simpleType name="GroupBaggageConditionsType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Describles baggage service conditions for a group(e.g., available, not available or manadatory).</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to16Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="GroupKindType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Specifies the type of group.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to32Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="HotelAwardType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Denotes an award received by the hotel (e.g., RingOfHonor, BestOfChoice, Gold, Platinum).</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to32Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="HotelChangeKindType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A classifier of Hotel Distribution Change Categories.
                                    (e.g., HOTEL_AMENITY, ROOM_AMENITY ROOM_TYPE)</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to32Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="HotelClosureReasonType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Indicates the reason for the closure of a
                                    hotel (e.g., Pre-Sell, Off-Season, Temporary,
                                    Pending Termination).</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to64Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="HotelLocationCodeType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Contains CARS (City, Airport, Resort,
                                    Suburb) code.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to16Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="HotelOpeningType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Classifies how a hotel was opened (e.g., NewBuild, Conversion).</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to32Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="MLOSStrategyType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Minimum/Maximum Length of Stay (MLOS) Stategy
                                    (e.g., ArrivalDateStrategy, TraditionalStrategy)</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to32Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="RefurbishExtentType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Describes the extent of the refurbishment (e.g., Full, Rooms, Lobby).</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to32Type"/>
  </xsd:simpleType>
</xsd:schema>]]></con:content>
        <con:type>http://www.w3.org/2001/XMLSchema</con:type>
      </con:part>
      <con:part>
        <con:url>http://esb.services.ext.pci.qa.chotel.com:80/HotelDistributionService/v6?SCHEMA%2FCdm_Shared_v6%2Fxsd%2Fdistribution%2FDistributionCommonTypes</con:url>
        <con:content><![CDATA[<!--Document: The DistributionCommonTypes schema contains the schema types
          that are common to the distribution domain.

Date: 12-10-2010
Last Updated: 02-27-2019
Authors: Chris Judson, Charlie Taylor, Kirk Damron, Datta Parupudi, Janice Goff, Niall Broderick, Rob Hewitt, Chris Lang, Josh Noble, Shriram Surya Suburaman-->
<xsd:schema targetNamespace="http://www.choicehotels.com/schema/v6/dist/cdm" elementFormDefault="qualified" attributeFormDefault="unqualified" xml:lang="en" xmlns:dst="http://www.choicehotels.com/schema/v6/dist/cdm" xmlns:cmn="http://www.choicehotels.com/schema/v6/common/cdm" xmlns:spt="http://www.choicehotels.com/schema/v6/support/cdm" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <xsd:import namespace="http://www.choicehotels.com/schema/v6/common/cdm" schemaLocation="http://esb.services.ext.pci.qa.chotel.com:80/HotelDistributionService/v6?SCHEMA%2FCdm_Shared_v6%2Fxsd%2Fcommon%2FCommonTypes"/>
  <xsd:import namespace="http://www.choicehotels.com/schema/v6/support/cdm" schemaLocation="http://esb.services.ext.pci.qa.chotel.com:80/HotelDistributionService/v6?SCHEMA%2FCdm_Shared_v6%2Fxsd%2Fsupport%2FPayment"/>
  <xsd:element name="acceptedPaymentForm" type="dst:AcceptedPaymentFormType"/>
  <xsd:element name="acceptedPaymentFormCode" type="dst:AcceptedPaymentFormCodeType"/>
  <xsd:element name="acceptedPaymentForms" type="dst:AcceptedPaymentFormsType"/>
  <xsd:element name="additionalGuestRate" type="dst:AdditionalGuestRateType"/>
  <xsd:element name="amenityCategory" type="dst:AmenityCategoryType"/>
  <xsd:element name="amenityCategoryList" type="dst:AmenityCategoryListType"/>
  <xsd:element name="amenityCode" type="dst:AmenityCodeType"/>
  <xsd:element name="areaAvailability" type="dst:AreaAvailabilityType"/>
  <xsd:element name="arrivalTransportationInfo" type="dst:ArrivalTransportationInfoType"/>
  <xsd:element name="bed" type="dst:BedType"/>
  <xsd:element name="beds" type="dst:BedsType"/>
  <xsd:element name="cancelPolicies" type="dst:CancelPoliciesType"/>
  <xsd:element name="cancelPolicy" type="dst:CancelPolicyType"/>
  <xsd:element name="commission" type="dst:CommissionType"/>
  <xsd:element name="coOpParticipation" type="dst:CoOpParticipationType"/>
  <xsd:element name="coOpParticipationSet" type="dst:CoOpParticipationSetType"/>
  <xsd:element name="destinationSystemCodes" type="dst:DestinationSystemCodesType"/>
  <xsd:element name="distributionChannel" type="dst:DistributionChannelType"/>
  <xsd:element name="distributionChannelId" type="dst:DistributionChannelIdType"/>
  <xsd:element name="distributionChannels" type="dst:DistributionChannelsType"/>
  <xsd:element name="distributionPartner" type="dst:DistributionPartnerType"/>
  <xsd:element name="distributionPartnerReference" type="dst:DistributionPartnerReferenceType"/>
  <xsd:element name="groupReservationId" type="dst:GroupReservationIdType"/>
  <xsd:element name="groupReservationReference" type="dst:GroupReservationReferenceType"/>
  <xsd:element name="guarantee" type="dst:GuaranteeType"/>
  <xsd:element name="guarantees" type="dst:GuaranteesType"/>
  <xsd:element name="hotelStatus" type="dst:HotelStatusType"/>
  <xsd:element name="multiAvailability" type="dst:MultiAvailabilityType"/>
  <xsd:element name="pricingAvailability" type="dst:PricingAvailabilityType"/>
  <xsd:element name="rateAccessSet" type="dst:RateAccessSetType"/>
  <xsd:element name="rateAccess" type="dst:RateAccessType"/>
  <xsd:element name="rateByNumberOfGuests" type="dst:RateByNumberOfGuestsType"/>
  <xsd:element name="ratePlan" type="dst:HotelRatePlanType"/>
  <xsd:element name="ratePlans" type="dst:HotelRatePlansType"/>
  <xsd:element name="ratePlanAccessAssignment" type="dst:RatePlanAccessAssignmentType"/>
  <xsd:element name="ratePlanAccessAssignments" type="dst:RatePlanAccessAssignmentsType"/>
  <xsd:element name="ratePlanCategories" type="dst:RatePlanCategoriesType"/>
  <xsd:element name="ratePlanCategory" type="dst:RatePlanCategoryType"/>
  <xsd:element name="ratePlanCode" type="cmn:RatePlanCodeType"/>
  <xsd:element name="ratePlanCodes" type="dst:RatePlanCodesType"/>
  <xsd:element name="ratePlanUsageTerm" type="dst:RatePlanUsageTermType"/>
  <xsd:element name="ratePlanUsageTerms" type="dst:RatePlanUsageTermsType"/>
  <xsd:element name="reservationAgent" type="dst:ReservationAgentType"/>
  <xsd:element name="roomAmenities" type="dst:RoomAmenitiesType"/>
  <xsd:element name="roomAmenity" type="dst:RoomAmenityType"/>
  <xsd:element name="roomRate" type="dst:RoomRateType"/>
  <xsd:element name="roomRateCalendar" type="dst:RoomRateCalendarType"/>
  <xsd:element name="roomRateRange" type="dst:RoomRateRangeType"/>
  <xsd:element name="roomRateRanges" type="dst:RoomRateRangesType"/>
  <xsd:element name="roomRates" type="dst:RoomRatesType"/>
  <xsd:element name="roomStay" type="dst:RoomStayType"/>
  <xsd:element name="roomType" type="dst:RoomTypeType"/>
  <xsd:element name="roomTypes" type="dst:RoomTypesType"/>
  <xsd:element name="salesContact" type="dst:SalesContactType"/>
  <xsd:element name="salesContacts" type="dst:SalesContactsType"/>
  <xsd:element name="singleHotelAvailability" type="dst:SingleHotelAvailabilityType"/>
  <xsd:element name="splitCommission" type="dst:SplitCommissionType"/>
  <xsd:complexType name="AcceptedPaymentFormsType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A collection of accepted payment forms.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="acceptedPaymentForm" type="dst:AcceptedPaymentFormType" minOccurs="1" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="AcceptedPaymentFormType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Describes an accepted form of payment.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="code" type="dst:AcceptedPaymentFormCodeType" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="kind" type="dst:AcceptedPaymentFormKindType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="description" type="cmn:StringLength1to255Type" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="use" minOccurs="0" maxOccurs="1">
        <xsd:complexType>
          <xsd:attribute name="guarantee" type="xsd:boolean" use="required">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">The payment method can be used as a guarantee.</xsd:documentation>
            </xsd:annotation>
          </xsd:attribute>
          <xsd:attribute name="settlement" type="xsd:boolean" use="required">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">The payment method can be used to settle a bill.</xsd:documentation>
            </xsd:annotation>
          </xsd:attribute>
          <xsd:attribute name="deposit" type="xsd:boolean" use="required">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">The payment method can be used as a deposit.</xsd:documentation>
            </xsd:annotation>
          </xsd:attribute>
        </xsd:complexType>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="AdditionalChargesType">
    <xsd:sequence>
      <xsd:element name="additionalCharge" type="dst:AdditionalChargeType" minOccurs="1" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="AdditionalChargeType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Additional charges for the room (i.e. Cribs
                                    or rollaways)</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element ref="dst:amenityCode" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The room amenity code for this charge.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="amount" type="cmn:AmountType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The amount for the charge per quantity.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="description" type="cmn:StringLength1to255Type" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="quantity" type="xsd:positiveInteger" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The number of items associated with this
                                      charge.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="AdditionalGuestRateType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Collection of incremental charges per age
                                    qualifying code for additional guests.
                                    Amount charged for additional occupant is
                                    with respect to age group of the base guests.</xsd:documentation>
    </xsd:annotation>
    <xsd:complexContent>
      <xsd:extension base="cmn:AmountType">
        <xsd:sequence>
          <xsd:element name="additionalGuestAmountDescription" type="cmn:StringLength1to255Type" minOccurs="0" maxOccurs="1">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">Text description of the
                                        AdditionalGuestAmount in a given
                                        language.</xsd:documentation>
            </xsd:annotation>
          </xsd:element>
        </xsd:sequence>
        <xsd:attribute name="maxAdditionalGuests" type="cmn:Numeric1to999Type" use="optional">
          <xsd:annotation>
            <xsd:documentation xml:lang="en">Increase the base rate by the additional
                                       occupant amount for each additional
                                       occupant of the same age group up to this
                                       maximum number of occupants of this age
                                       group.</xsd:documentation>
          </xsd:annotation>
        </xsd:attribute>
        <xsd:attributeGroup ref="dst:AgeQualifyingGroup"/>
      </xsd:extension>
    </xsd:complexContent>
  </xsd:complexType>
  <xsd:complexType name="AdvancedBookingDaysType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Defines the minimum and maximum number of
                                    days that a reservation must be made to get
                                    the rate plan.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="minimum" type="xsd:integer" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="maximum" type="xsd:integer" minOccurs="1" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="AmenityCategoryListType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A list of amenity categories.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="amenityCategory" type="dst:AmenityCategoryType" minOccurs="0" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="AmenityCategoryType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Defines a classification on amenities</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="code" type="cmn:StringLength1to8Type">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Category code (e.g., 'LAUND', 'PARK',
                                      'PET')</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="description" type="cmn:StringLength1to64Type">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Category description (e.g., 'Laundry',
                                      'Parking', 'Pets')</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="AmenityPreferenceType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">An amenity preference for search criteria.</xsd:documentation>
    </xsd:annotation>
    <xsd:attribute name="code" type="dst:AmenityCodeType" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">Code describing this amenity.</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
    <xsd:attribute name="otaCode" type="cmn:OTACodeType" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">OTA code and table expressed as follows:
                                      "code.table", for example, 100.RMA, 22.SEC.</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
  </xsd:complexType>
  <xsd:complexType name="AmenityType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Describes an amenity, for example, full breakfast,
                                    guest laundry.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="otaCodes" type="dst:OTACodesType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">OTA code mappings for this amenity.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="operatingSchedule" type="cmn:OperatingScheduleType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Specifies when this amenity is available for use.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="additionalInfo" type="xsd:string" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Consumer facing textual info about this amenity.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
    <xsd:attribute name="code" type="dst:AmenityCodeType" use="required">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">Code describing this amenity.</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
    <xsd:attribute name="description" type="cmn:StringLength1to128Type" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">Description of this amenity.</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
    <xsd:attribute name="sequence" type="xsd:short" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">Specifies the sort order preference for an amenity.
                                     Absence of a value for this attribute implies zero.</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
    <xsd:attribute name="charge" type="xsd:boolean" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">There is a charge for using this amenity. Absence of
                                     a value for this attribute implies false.</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
    <xsd:attribute name="fee" type="cmn:MoneyType" use="optional">
      <xsd:annotation>
        <xsd:documentation>Fee for this amenity in currency of hotel.</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
    <xsd:attribute name="feeApplicibility" type="cmn:ChargeUnitType" use="optional">
      <xsd:annotation>
        <xsd:documentation>Applicability for the fee (per person, per adult, per day, per 24 hour period, etc.).</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
  </xsd:complexType>
  <xsd:complexType name="AreaAvailabilityType">
    <!--TODO remove in CDM 7-->
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Represents a set of hotels having availability in a
                                    given geographical area. *** DEPRECATED ***</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="hotel" minOccurs="0" maxOccurs="unbounded">
        <xsd:complexType>
          <xsd:sequence>
            <xsd:element ref="cmn:hotelReference" minOccurs="1" maxOccurs="1"/>
            <xsd:element name="distanceFromOrigin" type="cmn:DistanceAndDirectionType" minOccurs="0" maxOccurs="1">
              <xsd:annotation>
                <xsd:documentation xml:lang="en">Distance and direction of this hotel from
                                         the origin of the seach.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="checkInOutDate" type="cmn:DateSpanType" minOccurs="1" maxOccurs="1"/>
            <xsd:element ref="cmn:numberOfGuests" minOccurs="0" maxOccurs="1"/>
            <xsd:element ref="dst:roomRateRange" minOccurs="0" maxOccurs="1"/>
            <xsd:element name="availabilityStatus" type="dst:RateIndicatorType" minOccurs="0" maxOccurs="1"/>
          </xsd:sequence>
        </xsd:complexType>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="ArrivalTransportationInfoType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Transportation information.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="type" type="dst:ArrivalTransportationType">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Type of transportation used to get to the
                                      hotel (Air, Rail, Bus, etc.).</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="id" type="cmn:StringLength1to64Type" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Identifier of the transportation, like a
                                      flight number</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="time" type="xsd:time" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Estimated time of transport</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="AvailabilityStatusesType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">The StatusApplicationControl is used to
                                    indicate to which block codes/rate
                                    plans/inventory codes a status should be
                                    applied.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="availabilityStatus" type="dst:AvailabilityStatusType" minOccurs="1" maxOccurs="unbounded"/>
      <xsd:element name="hotelId" type="cmn:HotelIdType" minOccurs="1" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="AvailabilityStatusPeriodType">
    <xsd:sequence>
      <xsd:annotation>
        <xsd:documentation xml:lang="en">Specifies the valid date range and avail
                                     status for the message.</xsd:documentation>
      </xsd:annotation>
      <xsd:element name="bookingLimit" type="dst:BookingLimitType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Limits that number of rooms that can be
                                      booked.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="dayOfWeekPattern" type="dst:DayOfWeekPatternType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="lengthsOfStay" type="dst:LOSsType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Collection of Length of Stay elements.
                                      These LOS elements indicate what LOS
                                      restrictions are to be added or removed.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="restrictionStatus" type="dst:RestrictionStatusType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Availability status assigned to the room
                                      rate combination.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="validDateRange" type="cmn:DateSpanType" minOccurs="1" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="AvailabilityStatusType">
    <xsd:sequence>
      <xsd:annotation>
        <xsd:documentation xml:lang="en">Used to indicate to which block codes/rate
                                     plans/inventory codes a status should be
                                     applied.</xsd:documentation>
      </xsd:annotation>
      <xsd:element name="availStatusPeriod" type="dst:AvailabilityStatusPeriodType" minOccurs="1" maxOccurs="unbounded"/>
      <xsd:element ref="cmn:hotelReference" minOccurs="1" maxOccurs="1"/>
      <xsd:element ref="dst:ratePlanCode" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">A string value may be used to request a
                                      particular code or an ID if the guest
                                      qualifies for a specific rate, such as
                                      AARP, AAA, a corporate rate, etc., or to
                                      specify a negotiated code as a result of a
                                      negotiated rate. If it is empty than the
                                      status applies to all rate plans.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element ref="dst:ratePlanCategory" minOccurs="0" maxOccurs="1"/>
      <xsd:element ref="cmn:roomTypeId" minOccurs="1" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="BedsType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A collection of bed types that can be
                                    assigned to a room.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="bed" type="dst:BedType" minOccurs="0" maxOccurs="unbounded"></xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="BedType">
    <xsd:attribute name="type" type="cmn:StringLength1to16Type" use="required">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">Bed type, e.g. 'King','Twin".</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
    <xsd:attribute name="count" type="xsd:nonNegativeInteger" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">Number of this type of bed assigned to
                                     an associated room type.</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
    <xsd:attribute name="gdsSequence" type="xsd:nonNegativeInteger" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">GDS sequencing value.</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
  </xsd:complexType>
  <xsd:complexType name="BookingLimitType">
    <xsd:sequence>
      <xsd:annotation>
        <xsd:documentation xml:lang="en">Used to control the number of rooms that can be
                                    booked.</xsd:documentation>
      </xsd:annotation>
      <xsd:element name="limit" type="cmn:Numeric0to999Type" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Room limit value.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="messageType" type="dst:BookingLimitMessageKindType" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Action to be performed for the booking
                                      limit.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="CancelPoliciesType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A collection of CancelPenalty.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="policy" type="dst:CancelPolicyType" minOccurs="0" maxOccurs="unbounded">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Defines the cancellation penalty of the
                                      hotel facility.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="CancelPolicyType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">The CancelPenalty class defines the
                                    cancellation policy of the hotel facility.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="applicableDateRange" type="cmn:DateSpanType" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The date time span for which the policy
                                      applies.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="deadline" type="cmn:DeadlineType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Cancellation deadline, absolute or
                                      relative.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="cancellationRefundAmount" type="dst:CancellationRefundAmountType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Used to specify the cancellation amount.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="penaltyDescription" type="cmn:StringLength1to255Type" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Text description of the Penalty in a given
                                      language.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
    <xsd:attribute name="nonRefundable" type="xsd:boolean" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">Indicates that any prepayment for the
                                     reservation is non refundable, therefore a
                                     100% penalty on the prepayment is applied,
                                     irrespective of deadline.</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
    <xsd:attribute name="code" type="cmn:StringLength1to16Type" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">A system specific room type to which this
                                     cancellation penalty applies.</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
  </xsd:complexType>
  <xsd:complexType name="CommissionType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Describes an amount that is payable as part
                                    of a sales agreement.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="percentage" type="cmn:PercentType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="fixed" type="cmn:CurrencyAmountType" minOccurs="0" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="CoOpParticipationSetType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Descibes participation in one or more
                                    co-operative marketing programs.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="coOpParticipation" type="dst:CoOpParticipationType" minOccurs="1" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="CoOpParticipationType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Descibes participation in a co-operative
                                    marketing program.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="coOpName" type="cmn:StringLength1to64Type" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="beginDate" type="xsd:date" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Beginning date of co-op participation.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="endDate" type="xsd:date" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Ending date of co-op participation.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="ReservationPaymentsType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A collection of reservation payments.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="reservationPayment" type="dst:ReservationPaymentType" minOccurs="1" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="ReservationPaymentType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Describes a payment that applies to a reservation.
                                    This includes deposits and pre-payments as well as
                                    collateral used to guarantee the reservation.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="paymentsAccepted" type="spt:PaymentsType" minOccurs="1" maxOccurs="unbounded">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Collection of forms of payment accepted
                                      for payment.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="totalDepositAmount" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Total amounts of deposit/payments. NOTE:
                                      If the payment is a loyalty redemption the
                                      amount of points, miles, etc. is not
                                      reflected here and instead a placeholder
                                      value such as 25.00USD or 0.00USD is used.</xsd:documentation>
        </xsd:annotation>
        <xsd:complexType>
          <xsd:complexContent>
            <xsd:extension base="cmn:AmountType">
              <xsd:attribute name="voucherUsed" use="optional">
                <xsd:annotation>
                  <xsd:documentation>True if a voucher was used for the reservation.</xsd:documentation>
                </xsd:annotation>
              </xsd:attribute>
              <xsd:attribute name="loyaltyRedemptionUsed" use="optional">
                <xsd:annotation>
                  <xsd:documentation>True if a loyalty redemption was used for the
                            reservation.</xsd:documentation>
                </xsd:annotation>
              </xsd:attribute>
            </xsd:extension>
          </xsd:complexContent>
        </xsd:complexType>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="DestinationSystemCodesType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A collection of DestinationSystemCode.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="destinationSystemCode" type="cmn:StringLength1to64Type" minOccurs="1" maxOccurs="unbounded">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The destination system code defines a
                                      system to which information is to be
                                      provided.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="DistributionChannelIdType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">The unique identifier of distribution channel.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="id" type="cmn:StringLength1to32Type" minOccurs="1" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="DistributionChannelsType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A collection of distribution channels.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="distributionChannel" type="dst:DistributionChannelType" minOccurs="0" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="DistributionChannelType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Describes a distribution channel.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="id" type="dst:DistributionChannelIdType" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="kind" type="dst:DistributionChannelKindType" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="description" type="cmn:StringLength1to128Type" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="distributionPartnerReference" type="dst:DistributionPartnerReferenceType" minOccurs="0" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="DistributionPartnerReferenceType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A reference to a distribution partner.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="code" type="dst:DistributionPartnerCodeType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="name" type="cmn:StringLength1to64Type" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="kind" type="dst:DistributionPartnerKindType" minOccurs="0" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="DistributionPartnerType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Describes a distribution partner.</xsd:documentation>
    </xsd:annotation>
    <xsd:complexContent>
      <xsd:extension base="dst:DistributionPartnerReferenceType">
        <xsd:sequence>
          <xsd:element name="description" type="cmn:StringLength1to128Type" minOccurs="0" maxOccurs="1"/>
        </xsd:sequence>
      </xsd:extension>
    </xsd:complexContent>
  </xsd:complexType>
  <xsd:complexType name="FeesType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A collection of fees.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="fee" type="dst:FeeType" maxOccurs="unbounded">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Fee Amount that is applied to the rate.
                                      Fees are used for non tax amounts like
                                      service charges.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="FeeTaxType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Defines the fees and/or taxes associated
                                    with a charge (e.g. taxes associated with a
                                    hotel rate).</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:choice minOccurs="1" maxOccurs="1">
        <xsd:element name="amount" type="cmn:MoneyType">
          <xsd:annotation>
            <xsd:documentation xml:lang="en">Used to provide a total of all the taxes.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
        <xsd:element name="percent" type="cmn:PercentType">
          <xsd:annotation>
            <xsd:documentation xml:lang="en">Fee percentage.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
      </xsd:choice>
      <xsd:element name="feeTaxcode" type="dst:FeeTaxCodeType" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Code identifying the fee (e.g.,agency fee,
                                      municipality fee).</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="FeeType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Used for non-tax fees and charges (e.g.
                                    service charges) .</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="description" type="xsd:string" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Text description of the fees in a given
                                      language.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="effectiveDate" type="cmn:DateSpanType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Indicates the starting date for fee.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="code" type="cmn:StringLength1to8Type" maxOccurs="1" minOccurs="0"/>
      <xsd:choice maxOccurs="1">
        <xsd:element name="amount" type="cmn:AmountType" maxOccurs="1" minOccurs="0"/>
        <xsd:element name="percent" type="cmn:PercentType" minOccurs="0" maxOccurs="1">
          <xsd:annotation>
            <xsd:documentation xml:lang="en">Fee percentage is optional and is for
                                       reference only.</xsd:documentation>
          </xsd:annotation>
        </xsd:element>
      </xsd:choice>
    </xsd:sequence>
    <xsd:attributeGroup ref="cmn:ChargeUnitGroup">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">Specifies charge information by unit (e.g.,
                                     room, person, item) and frequency (e.g.,
                                     daily, weekly, stay).</xsd:documentation>
      </xsd:annotation>
    </xsd:attributeGroup>
  </xsd:complexType>
  <xsd:complexType name="GeographicLocationType">
    <xsd:sequence>
      <xsd:element name="point" minOccurs="0" maxOccurs="1">
        <xsd:complexType>
          <xsd:complexContent>
            <xsd:extension base="cmn:GeographicPointType">
              <xsd:sequence>
                <xsd:element name="determinationMethod" type="cmn:StringLength1to16Type" minOccurs="0" maxOccurs="1">
                  <xsd:annotation>
                    <xsd:documentation xml:lang="en">Determination method (e.g. GPS
                                           device, address geocoding, etc.).</xsd:documentation>
                  </xsd:annotation>
                </xsd:element>
                <xsd:element name="locationVerified" type="xsd:boolean" minOccurs="0" maxOccurs="1">
                  <xsd:annotation>
                    <xsd:documentation xml:lang="en">Whether the geographic location has
                                           been verified.</xsd:documentation>
                  </xsd:annotation>
                </xsd:element>
                <xsd:element name="verificationDate" type="xsd:date" minOccurs="0" maxOccurs="1">
                  <xsd:annotation>
                    <xsd:documentation xml:lang="en">The date the geographic location was
                                           verified.</xsd:documentation>
                  </xsd:annotation>
                </xsd:element>
              </xsd:sequence>
            </xsd:extension>
          </xsd:complexContent>
        </xsd:complexType>
      </xsd:element>
      <xsd:element name="geopoliticalLocation" type="cmn:AddressType" minOccurs="0" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="GroupReservationIdType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">The unique identifier of a group reservation.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="id" type="cmn:StringLength1to32Type" minOccurs="1" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="GroupReservationReferenceType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A reference to a group reservation.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="groupReservationId" type="dst:GroupReservationIdType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="groupName" type="cmn:StringLength1to128Type" minOccurs="0" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="GuaranteeMethodType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Describes the method used to guarantee a reservation.</xsd:documentation>
    </xsd:annotation>
    <xsd:complexContent>
      <xsd:extension base="spt:PaymentFormType">
        <xsd:sequence>
          <xsd:element name="guaranteeDescription" type="xsd:string" minOccurs="0" maxOccurs="1">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">Text description of the Guarantee in a
                                       given language.</xsd:documentation>
            </xsd:annotation>
          </xsd:element>
        </xsd:sequence>
        <xsd:attribute name="holdTime" type="xsd:time" use="optional">
          <xsd:annotation>
            <xsd:documentation xml:lang="en">The room will held up until this time
                                      without a guarantee.</xsd:documentation>
          </xsd:annotation>
        </xsd:attribute>
      </xsd:extension>
    </xsd:complexContent>
  </xsd:complexType>
  <xsd:complexType name="GuaranteesType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A collection of reservation hold guarantees</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="guarantee" type="dst:GuaranteeType" minOccurs="1" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="GuaranteeType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">The guarantee information to hold a
                                    reservation</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="guaranteesAccepted" minOccurs="0" maxOccurs="1">
        <xsd:complexType>
          <xsd:sequence>
            <xsd:element name="guaranteeAccepted" minOccurs="1" maxOccurs="unbounded">
              <xsd:annotation>
                <xsd:documentation xml:lang="en">Guarantee Detail.</xsd:documentation>
              </xsd:annotation>
              <xsd:complexType>
                <xsd:complexContent>
                  <xsd:extension base="spt:PaymentFormType">
                    <xsd:attribute name="cardHolderInfoReqInd" type="xsd:boolean" use="optional">
                      <xsd:annotation>
                        <xsd:documentation xml:lang="en">If true, credit card holder
                                             information is required. If false,
                                             it is not required.</xsd:documentation>
                      </xsd:annotation>
                    </xsd:attribute>
                    <xsd:attribute name="nameReqInd" type="xsd:boolean" use="optional">
                      <xsd:annotation>
                        <xsd:documentation xml:lang="en">If true, the credit card holder
                                             name is required. If false, it is
                                             not required.</xsd:documentation>
                      </xsd:annotation>
                    </xsd:attribute>
                    <xsd:attribute name="addressReqInd" type="xsd:boolean" use="optional">
                      <xsd:annotation>
                        <xsd:documentation xml:lang="en">If true, credit card holder address
                                             is required. If false, it is not
                                             required.</xsd:documentation>
                      </xsd:annotation>
                    </xsd:attribute>
                    <xsd:attribute name="phoneReqInd" type="xsd:boolean" use="optional">
                      <xsd:annotation>
                        <xsd:documentation xml:lang="en">If true, credit card holder phone
                                             number is required. If false, it is
                                             not required.</xsd:documentation>
                      </xsd:annotation>
                    </xsd:attribute>
                    <xsd:attribute name="bookingSourceAllowedInd" type="xsd:boolean" use="optional">
                      <xsd:annotation>
                        <xsd:documentation xml:lang="en">When true, the booking source may
                                             be used to guarantee the booking.</xsd:documentation>
                      </xsd:annotation>
                    </xsd:attribute>
                    <xsd:attribute name="corpDiscountNbrAllowedInd" type="xsd:boolean" use="optional">
                      <xsd:annotation>
                        <xsd:documentation xml:lang="en">When true, the corporate discount
                                             number may be used to guarantee the
                                             booking.</xsd:documentation>
                      </xsd:annotation>
                    </xsd:attribute>
                  </xsd:extension>
                </xsd:complexContent>
              </xsd:complexType>
            </xsd:element>
          </xsd:sequence>
        </xsd:complexType>
      </xsd:element>
      <xsd:element name="deadline" type="cmn:DeadlineType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Guarantee deadline, absolute or relative.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="comments" type="xsd:string" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="guaranteeDescription" type="xsd:string" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Text description of the Guarantee in a
                                      given language.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
    <xsd:attribute name="retributionType" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">An enumerated type defining the type of
                                     action taken when the deadline has been
                                     exceeded. Valid values: Res Automatically
                                     Cancelled, Res No Longer Guaranteed.</xsd:documentation>
      </xsd:annotation>
      <xsd:simpleType>
        <xsd:restriction base="cmn:StringLength1to32Type">
          <xsd:enumeration value="ReservationAutoCancelled"/>
          <xsd:enumeration value="ReservationNotGuaranteed"/>
        </xsd:restriction>
      </xsd:simpleType>
    </xsd:attribute>
    <xsd:attribute name="guaranteeCode" type="cmn:StringLength1to32Type" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">Guarantee Code</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
    <xsd:attribute name="guaranteeKind" type="cmn:GuaranteeKindCodeType" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">GuaranteeType: GuaranteeType An enumerated
                                     type defining the guarantee to be applied
                                     to this reservation.</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
    <xsd:attribute name="holdTime" type="xsd:time" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">The room will held up until this time
                                     without a guarantee.</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
  </xsd:complexType>
  <xsd:complexType name="HotelAmenityPreferenceType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A hotel amenity preference to be used when
                                    searching for hotels and/or rooms. For
                                    example, on a RoomAvailability search, only
                                    consider hotels that include a heated pool
                                    and an onsite restaurant.</xsd:documentation>
    </xsd:annotation>
    <xsd:complexContent>
      <xsd:extension base="dst:AmenityPreferenceType"/>
    </xsd:complexContent>
  </xsd:complexType>
  <xsd:complexType name="HotelAmenityPreferencesType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A collection of hotel amenity preferences.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="amenity" type="dst:HotelAmenityPreferenceType" minOccurs="0" maxOccurs="unbounded"/>
    </xsd:sequence>
    <xsd:attribute name="verbose" type="xsd:boolean" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">When true, return all details for a hotel amenity.</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
  </xsd:complexType>
  <xsd:complexType name="HotelPolicyQualifierType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Defines the applicability of a hotel policy.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element ref="cmn:countryCode" minOccurs="0" maxOccurs="1"/>
      <xsd:element ref="cmn:stateOrProvince" minOccurs="0" maxOccurs="1"/>
      <xsd:element ref="cmn:brandCode" minOccurs="0" maxOccurs="1"/>
      <xsd:element ref="cmn:productCode" minOccurs="0" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="HotelRatePlanType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">All details pertaining to a specific rate
                                    plan.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="active" type="xsd:boolean" maxOccurs="1" minOccurs="0"/>
      <xsd:element name="advancedBookingDays" type="dst:AdvancedBookingDaysType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="availabilityStatus" type="dst:RateIndicatorType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Indicates whether RatePlan has
                                      availablity; "AvailableForSale",
                                      "NoAvailability", "Restricted"</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="awardEligibility" type="xsd:boolean" maxOccurs="1" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Indicates whether rate plan is eligible to
                                      earn reward program points.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="bookingChannels" minOccurs="0" maxOccurs="1">
        <!--TODO remove in CDM 7-->
        <xsd:annotation>
          <xsd:documentation xml:lang="en">*** DEPRECATED ***
                                      Use distributionChannels instead.
                                      
                                      Booking channels enabled for rate plan.</xsd:documentation>
        </xsd:annotation>
        <xsd:complexType>
          <xsd:sequence>
            <xsd:element name="bookingChannel" minOccurs="1" maxOccurs="unbounded">
              <xsd:annotation>
                <xsd:documentation xml:lang="en">Describes a booking channel, e.g., .com.</xsd:documentation>
              </xsd:annotation>
              <xsd:complexType>
                <xsd:sequence>
                  <xsd:element name="code" type="cmn:StringLength1to4Type" minOccurs="1" maxOccurs="1">
                    <xsd:annotation>
                      <xsd:documentation xml:lang="en">Channel specific code.</xsd:documentation>
                    </xsd:annotation>
                  </xsd:element>
                </xsd:sequence>
              </xsd:complexType>
            </xsd:element>
          </xsd:sequence>
        </xsd:complexType>
      </xsd:element>
      <xsd:element name="distributionChannels" type="dst:DistributionChannelsType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="bookingRequirement" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Booking requirement for rate plan, for
                                      example, Travel Agent ID, Rewards Program
                                      ID.</xsd:documentation>
        </xsd:annotation>
        <xsd:complexType>
          <xsd:sequence>
            <xsd:element name="code" type="cmn:StringLength1to4Type" minOccurs="1" maxOccurs="1">
              <xsd:annotation>
                <xsd:documentation xml:lang="en">Booking code.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="authorizationRequired" type="xsd:boolean" minOccurs="1" maxOccurs="1">
              <xsd:annotation>
                <xsd:documentation xml:lang="en">Indicates whether rate plan
                                         authorization is required.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
          </xsd:sequence>
        </xsd:complexType>
      </xsd:element>
      <xsd:element name="cancelPolicies" type="dst:CancelPoliciesType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">A collection of Cancellation Policies.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="checkInRequirement" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Check-in requirements for rate plan, for
                                      example, Corporate ID, Military ID.</xsd:documentation>
        </xsd:annotation>
        <xsd:complexType>
          <xsd:sequence>
            <xsd:element name="code" type="cmn:StringLength1to4Type" minOccurs="1" maxOccurs="1">
              <xsd:annotation>
                <xsd:documentation xml:lang="en">Check-in ID code.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
          </xsd:sequence>
        </xsd:complexType>
      </xsd:element>
      <xsd:element name="commission" type="dst:CommissionType" maxOccurs="1" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">When present, this rate plan is
                                      commisionable.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="description" type="cmn:StringLength1to255Type" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="effectiveDate" type="cmn:DateSpanType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Effective date range for this rate plan.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="excludeExtraPersonCharge" type="xsd:boolean" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">True indicates no extra person charges.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="excludedRoomTypes" type="dst:RoomTypesType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Defines room types explicitly excluded
                                      from this rate plan.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="featuredRatePlan" type="xsd:boolean" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Rate plan has special emphasis.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="gdsSequence" type="xsd:nonNegativeInteger" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Used to order rate plans when presented to the GDS channel.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="guaranteeMethod" type="dst:GuaranteeMethodType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="guaranteePolicies" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">A collection of Guarantee Policies.</xsd:documentation>
        </xsd:annotation>
        <xsd:complexType>
          <xsd:sequence>
            <xsd:element name="guaranteePolicy" type="dst:GuaranteeType" maxOccurs="unbounded">
              <xsd:annotation>
                <xsd:documentation xml:lang="en">GuaranteePolicy.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
          </xsd:sequence>
        </xsd:complexType>
      </xsd:element>
      <xsd:element ref="cmn:hotelId" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="limitStayToDOW" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Declares which DOW rate plan is available.
                                      True indicates that the rate plan in
                                      available on the particular day.</xsd:documentation>
        </xsd:annotation>
        <xsd:complexType>
          <xsd:sequence>
            <xsd:element name="sunday" type="xsd:boolean" minOccurs="1" maxOccurs="1"/>
            <xsd:element name="monday" type="xsd:boolean" minOccurs="1" maxOccurs="1"/>
            <xsd:element name="tuesday" type="xsd:boolean" minOccurs="1" maxOccurs="1"/>
            <xsd:element name="wednesday" type="xsd:boolean" minOccurs="1" maxOccurs="1"/>
            <xsd:element name="thursday" type="xsd:boolean" minOccurs="1" maxOccurs="1"/>
            <xsd:element name="friday" type="xsd:boolean" minOccurs="1" maxOccurs="1"/>
            <xsd:element name="saturday" type="xsd:boolean" minOccurs="1" maxOccurs="1"/>
          </xsd:sequence>
        </xsd:complexType>
      </xsd:element>
      <xsd:element name="maxRoomsPerBooking" type="xsd:integer" maxOccurs="1" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The maximum rooms that can be booked for
                                      this rate plan.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="maxLOS" type="dst:LengthOfStayType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The maximum length of stay allowed by this
                                      rate plan.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="minLOS" type="dst:LengthOfStayType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The minimum length of stay required by
                                      this rate plan.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="name" type="cmn:StringLength1to64Type" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="participation" type="cmn:StringLength1to16Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Indicates the level of participation the
                                      hotel has with this rate plan, e.g,
                                      Mandatory, Elective.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="policyOverride" type="xsd:boolean" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Indicates whether the rate plan
                                      cancel/guarantee policies override those
                                      at the Hotel level.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="rateCategory" type="cmn:StringLength1to4Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Indicates the rate category, e.g.,
                                      Entitled, Other</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="ratePlanCategories" type="dst:RatePlanCategoriesType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">A list of rate plan categories to which this rate plan belongs.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="ratePlanCode" type="cmn:RatePlanCodeType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="ratePlanFees" type="dst:FeesType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">A collection of Fees.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="ratePlanType" type="dst:RatePlanKindType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Defines the type of Rate Plan, e.g.,
                                      Choice, Local.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="requiredMinimumAge" type="cmn:Numeric1to99Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Defines the minimum age required to
                                      qualify for this rate plan.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="roomTypes" type="dst:RoomTypesType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The list of room types associated with
                                      this rate plan.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="sellingLimit" type="cmn:Numeric1to999Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">When present, defines a limit on the
                                      number of rooms that can be sold daily.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="sellingLimitBucketCode" type="cmn:StringLength1to8Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">When present, indicates the shared selling
                                      bucket (group) this rate plan is
                                      associated with. The shared selling bucket
                                      defines the selling limit for all its
                                      associated rate plans.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="separateRoomAndTax" type="xsd:boolean" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Indicator to a PMS that room and tax
                                      should be on separate folio from
                                      incidental charges.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="shoppingCategories" type="dst:ShoppingCategoriesType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Shopping categories associated with this
                                      rate plan.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="suppressRate" type="xsd:boolean" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Indicates whether rate amounts must be
                                      suppressed.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="taxExempt" type="xsd:boolean" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Indicates whether rate plan is tax exempt.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="taxInclusive" type="xsd:boolean" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Indicates whether rate plan is tax
                                      inclusive.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="baseRatePlanCode" type="cmn:RatePlanCodeType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The rate plan this rate plan is derived
                                      from.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="adjustedAmount" type="cmn:MoneyType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The amount which should be added to the
                                      base rate plan to determine the price of
                                      this derived rate plan. Positive values
                                      indicate mark-up, negative values indicate
                                      discount.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="adjustedPercentage" type="cmn:PercentType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The percentage off (negative) or percentage
                                      markup (positive) the base rate plan amount
                                      used to determine the price of this derived
                                      rate plan.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="floorAmount" type="cmn:MoneyType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The lowest amount for which this derived
                                      rate plan should be sold.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="ceilingAmount" type="cmn:MoneyType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The highest amount for which this derived
                                      rate plan should be sold.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="HotelRatePlansType">
    <xsd:sequence>
      <xsd:element name="hotelRatePlan" type="dst:HotelRatePlanType" minOccurs="0" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="HotelStayTotalAmountType">
    <xsd:complexContent>
      <xsd:extension base="cmn:AmountType">
        <xsd:sequence>
          <xsd:element name="loyaltyRedemptionAmount" type="dst:LoyaltyRedemptionAmountType" minOccurs="0" maxOccurs="1"/>
        </xsd:sequence>
        <xsd:attribute name="voucherUsed" use="optional">
          <xsd:annotation>
            <xsd:documentation xml:lang="en">True if a voucher was used for the reservation.</xsd:documentation>
          </xsd:annotation>
        </xsd:attribute>
        <xsd:attribute name="loyaltyRedemptionUsed" use="optional">
          <xsd:annotation>
            <xsd:documentation xml:lang="en">True if a loyalty redemption was used for the
                                       reservation.</xsd:documentation>
          </xsd:annotation>
        </xsd:attribute>
      </xsd:extension>
    </xsd:complexContent>
  </xsd:complexType>
  <xsd:complexType name="LOSType">
    <xsd:sequence>
      <xsd:element name="losPattern" type="cmn:StringLength1to32Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">This may be used when MinMaxMessageType is
                                      FullPatternLOS to identify the open and
                                      closed status by LOS (e.g., if
                                      LengthsOfStay@FixedPatternLength="5" then
                                      FullPatternLOS="YYNYY" or
                                      FullPatternLOS="11011").</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="openStatusIndicator" type="xsd:boolean" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Indicates if the length of stay is open or
                                      closed when MinMaxMessageType is
                                      FullPatternLOS if true then open and if
                                      false then closed.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="time" type="xsd:integer" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Used in conjunction with the
                                      MinMaxMessageType and the TimeUnit to
                                      define the length of stay requirements.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="timeUnit" type="cmn:TimeUnitType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">A time unit used to apply this status
                                      message to other inventory, and with more
                                      granularity than daily. Values: Year,
                                      Month, Week, Day, Hour, Minute, Second.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="minMaxMessageKind" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">An enumerated type used to define how the
                                      minimum and maximum LOS is applied.
                                      Values: Set Minimum LOS, Remove Minimum
                                      LOS, Set Maximum LOS, Remove Maximum LOS,
                                      Set Forward Minimum Stay, Remove Forward
                                      Minimum Stay, Set Forward Maximum Stay,
                                      Remove Forward Maximum Stay.</xsd:documentation>
        </xsd:annotation>
        <xsd:simpleType>
          <xsd:restriction base="xsd:string">
            <xsd:enumeration value="SetMinLOS">
              <xsd:annotation>
                <xsd:documentation xml:lang="en">Used to set the minimum length of stay
                                         (LOS).</xsd:documentation>
              </xsd:annotation>
            </xsd:enumeration>
            <xsd:enumeration value="RemoveMinLOS">
              <xsd:annotation>
                <xsd:documentation xml:lang="en">Used to remove the minimum length of
                                         stay (LOS).</xsd:documentation>
              </xsd:annotation>
            </xsd:enumeration>
            <xsd:enumeration value="SetMaxLOS">
              <xsd:annotation>
                <xsd:documentation xml:lang="en">Used to set the maximum length of stay
                                         (LOS).</xsd:documentation>
              </xsd:annotation>
            </xsd:enumeration>
            <xsd:enumeration value="RemoveMaxLOS">
              <xsd:annotation>
                <xsd:documentation xml:lang="en">Used to remove the maximum length of
                                         stay (LOS).</xsd:documentation>
              </xsd:annotation>
            </xsd:enumeration>
            <xsd:enumeration value="SetForwardMinStay"/>
            <xsd:enumeration value="RemoveForwardMinStay"/>
            <xsd:enumeration value="SetForwardMaxStay"/>
            <xsd:enumeration value="RemoveForwardMaxStay"/>
            <xsd:enumeration value="FixedLOS">
              <xsd:annotation>
                <xsd:documentation xml:lang="en">This indicates the required length of
                                         stay (LOS).</xsd:documentation>
              </xsd:annotation>
            </xsd:enumeration>
            <xsd:enumeration value="FullPatternLOS">
              <xsd:annotation>
                <xsd:documentation xml:lang="en">This indicates allowable length of stay
                                         (LOS). When used, there is an option to
                                         fully define the open and closed status
                                         with the attribute FullPatternLOS in
                                         the subelement LOS_Pattern.</xsd:documentation>
              </xsd:annotation>
            </xsd:enumeration>
            <xsd:enumeration value="MinLOS">
              <xsd:annotation>
                <xsd:documentation xml:lang="en">Used to specify the minimum length of
                                         stay.</xsd:documentation>
              </xsd:annotation>
            </xsd:enumeration>
            <xsd:enumeration value="MaxLOS">
              <xsd:annotation>
                <xsd:documentation xml:lang="en">Used to specify the maximum length of
                                         stay.</xsd:documentation>
              </xsd:annotation>
            </xsd:enumeration>
          </xsd:restriction>
        </xsd:simpleType>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="LOSsType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A collection of LengthOfStay.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:annotation>
        <xsd:documentation xml:lang="en">A collection of patterns defining allowable
                                     lengths of stay (LOS).</xsd:documentation>
      </xsd:annotation>
      <xsd:element name="los" type="dst:LOSType" minOccurs="0" maxOccurs="unbounded"/>
      <xsd:element name="arrivalDateBased" type="xsd:boolean" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">True indicates that LOS is based on
                                      arrival date. False indicates that LOS is
                                      based on stay date.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="LoyaltyRedemptionAmountType">
    <xsd:sequence>
      <xsd:element ref="cmn:loyaltyProgramId" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="amount" type="cmn:NonNegativeDecimal" minOccurs="1" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="MultiAvailabilityType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Represents a set of hotels having availability.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="hotel" minOccurs="0" maxOccurs="unbounded">
        <xsd:complexType>
          <xsd:sequence>
            <xsd:element ref="cmn:hotelReference" minOccurs="1" maxOccurs="1"/>
            <xsd:element name="checkInOutDate" type="cmn:DateSpanType" minOccurs="1" maxOccurs="1"/>
            <xsd:element ref="cmn:numberOfGuests" minOccurs="0" maxOccurs="1"/>
            <xsd:element ref="dst:roomRateRanges" minOccurs="0" maxOccurs="1"/>
            <xsd:element name="availabilityStatus" type="dst:RateIndicatorType" minOccurs="0" maxOccurs="1"/>
          </xsd:sequence>
        </xsd:complexType>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="NotificationRequestType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Describes how guests or other interested
                                    parties are to be notified for certain events.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="recipient" type="cmn:PersonContactType" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="notificationMethod" type="cmn:NotificationMethodType" minOccurs="1" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="OTACodesType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A collection of OTA code and code list table
                                    values.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="code" type="cmn:OTACodeType" minOccurs="0" maxOccurs="unbounded">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">OTA code and its associated table, for
                                      example, "100.HAC", "198.RMA".</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="PointRedemptionTierType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Defines a specific points redemption period
                                    comprising the date span and the associated
                                    points requirement.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="period" type="cmn:DateSpanType" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="tier" type="xsd:integer" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="points" type="xsd:integer" minOccurs="1" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="PointRedemptionTiersType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A collection of point redemption tiers.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="tier" type="dst:PointRedemptionTierType" minOccurs="0" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="PseudoCityCodesType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A collection of pseudo city codes</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="PseudoCityCode" type="dst:PseudoCityCodeType" minOccurs="1" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="PricingAvailabilityType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Represents the room pricing for a given hotel.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="checkInOutDate" type="cmn:DateSpanType" minOccurs="1" maxOccurs="1"/>
      <xsd:element ref="dst:ratePlan" minOccurs="0" maxOccurs="1"/>
      <xsd:element ref="dst:roomType" minOccurs="0" maxOccurs="1"/>
      <xsd:element ref="cmn:numberOfGuests" minOccurs="0" maxOccurs="1"/>
      <xsd:element ref="dst:roomRate" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="cancelPolicies" type="dst:CancelPoliciesType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="guaranteeOptions" type="dst:GuaranteesType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="totalAmount" type="dst:HotelStayTotalAmountType" minOccurs="0" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="RateAccessSetType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A set of rate access entities.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="rateAccess" type="dst:RateAccessType" minOccurs="0" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="RateAccessType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Describes a rate access entity.</xsd:documentation>
    </xsd:annotation>
    <xsd:attribute name="code" type="dst:RatePlanAccessCodeType" use="required"/>
    <xsd:attribute name="longCode" type="dst:RatePlanAccessCodeType" use="optional"/>
    <xsd:attribute name="partner" type="dst:DistributionPartnerCodeType" use="required"/>
  </xsd:complexType>
  <xsd:complexType name="RateByNumberOfGuestsType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A collection of Base charges by number of
                                    guests.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="rateByGuest" minOccurs="1" maxOccurs="unbounded">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Base charge for a given number of guests
                                      for a given age qualifying code.</xsd:documentation>
        </xsd:annotation>
        <xsd:complexType>
          <xsd:complexContent>
            <xsd:extension base="cmn:AmountType">
              <xsd:sequence>
                <xsd:element name="numberOfGuestsDescription" type="xsd:string" minOccurs="0" maxOccurs="1">
                  <xsd:annotation>
                    <xsd:documentation xml:lang="en">Description of number of guests and
                                           the associated age group (ex 2
                                           Adults).</xsd:documentation>
                  </xsd:annotation>
                </xsd:element>
                <xsd:element ref="cmn:numberOfGuests" minOccurs="1" maxOccurs="1">
                  <xsd:annotation>
                    <xsd:documentation xml:lang="en">The number of guests associated with
                                           this base charge.</xsd:documentation>
                  </xsd:annotation>
                </xsd:element>
              </xsd:sequence>
              <xsd:attributeGroup ref="dst:AgeQualifyingGroup"/>
            </xsd:extension>
          </xsd:complexContent>
        </xsd:complexType>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="RatePlanAccessAssignmentsType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A collection of rate plan access assignments.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element ref="dst:ratePlanAccessAssignment" minOccurs="1" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="RatePlanAccessAssignmentType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Describes the assignment of a rate plan access
                                    code to an entity.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="ratePlanAccessCode" type="dst:RatePlanAccessCodeType" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="assignee" type="cmn:StringLength1to64Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Name of the entity that has been assigned the
                                     access code.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="assigneeAccountId" type="cmn:AccountIdType" minOccurs="0" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="RatePlanCategoriesType">
    <xsd:sequence>
      <xsd:element ref="dst:ratePlanCategory" minOccurs="0" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="RatePlanCategoryType">
    <xsd:sequence>
      <xsd:element name="category" type="cmn:StringLength1to16Type" minOccurs="1" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="RatePlanCodesType">
    <xsd:sequence>
      <xsd:element ref="cmn:ratePlanCode" minOccurs="0" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="RatePlanUsageTermsType">
    <xsd:sequence>
      <xsd:element name="ratePlanUsageTerm" type="dst:RatePlanUsageTermType" minOccurs="1" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="RatePlanUsageTermType">
    <xsd:sequence>
      <xsd:element name="contractId" type="cmn:StringLength1to16Type" minOccurs="0" maxOccurs="1"/>
      <xsd:element ref="cmn:ratePlanCode" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="effectiveDateRange" type="cmn:DateSpanType" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="allowGuaranteeOverride" type="xsd:boolean" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="additionalDiscountPercent" type="cmn:PercentType" minOccurs="0" maxOccurs="1">
        <!--TODO remove in CDM 7-->
        <xsd:annotation>
          <xsd:documentation xml:lang="en">*** DEPRECATED ***
                                      This element is not to be used since the discounts
                                      must be dictated by the rate plan.
                                      
                                      An additional discount to apply to the rate
                                      after the rack discount has been applied.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="commissionable" type="xsd:boolean" minOccurs="0" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="RateType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Defines the details of a rate.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="additionalCharges" type="dst:AdditionalChargesType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="additionalGuestRates" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">A collection of charges that apply to
                                      additional occupants, guests or service
                                      users (over and above the rate's MaxGuest
                                      Applicable).</xsd:documentation>
        </xsd:annotation>
        <xsd:complexType>
          <xsd:sequence>
            <xsd:element ref="dst:additionalGuestRate" minOccurs="1" maxOccurs="1">
              <xsd:annotation>
                <xsd:documentation xml:lang="en">Collection of incremental charges per
                                         age qualifying code for additional
                                         guests. Amount charged for additional
                                         occupant is with respect to age group
                                         of the base guests.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
          </xsd:sequence>
        </xsd:complexType>
      </xsd:element>
      <xsd:element name="commissionable" type="xsd:boolean" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="dateRange" type="cmn:DateSpanType" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="daysOfWeekRateValid" type="dst:DayOfWeekPatternType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Allows for specifying the days of the week
                                      that this rate is valid.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="fees" type="dst:FeesType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="minLOS" type="dst:LengthOfStayType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The minimum length of stay required by
                                      this rate plan.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="maxLOS" type="dst:LengthOfStayType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The maximum length of stay allowed by this
                                      rate plan.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="loyaltyRedemptionAmount" type="dst:LoyaltyRedemptionAmountType" minOccurs="0" maxOccurs="1"/>
      <xsd:element ref="dst:rateByNumberOfGuests" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">A collection of Base charges by number of
                                      guests.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="stayOverDay" type="cmn:DayOfWeekType" minOccurs="0" maxOccurs="7">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Indicates a specific day on which the
                                      guest must stay over in order to be
                                      eligible for the quoted rate plan.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="totalAmount" type="cmn:AmountType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Total price for the room rate, for
                                      example, 3 nights at $100 per night for a
                                      King room would total $300</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
    <xsd:attribute name="rateTier" type="dst:RateTierType" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">Hotel systems often have different tiers
                                     for a given rate plan; this attribute is
                                     used to designate a specific tier within
                                     the rate plan (e.g. high, medium, low).</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
  </xsd:complexType>
  <xsd:complexType name="ReservationAgentType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Describes the person who booking a reservation.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="id" type="cmn:StringLength1to64Type" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="name" type="cmn:PersonNameType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="dutyCode" type="cmn:StringLength1to16Type" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="companyName" type="cmn:StringLength1to64Type" minOccurs="0" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="RestrictionStatusType">
    <xsd:sequence>
      <xsd:annotation>
        <xsd:documentation xml:lang="en">Describes the status of a restriction on a
                                     room and/or rate.</xsd:documentation>
      </xsd:annotation>
      <xsd:element name="restriction" type="dst:RestrictionType" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="status" type="dst:StatusType" minOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The availability status of the room.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="RoomAmenityPreferenceType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A room amenity preference to be used when
                                    searching for rooms. For example, on a
                                    RoomAvailability search, only consider rooms
                                    that include a widescreen TV and wireless
                                    internet.</xsd:documentation>
    </xsd:annotation>
    <xsd:complexContent>
      <xsd:extension base="dst:AmenityPreferenceType">
        <xsd:attribute name="quantity" type="cmn:Numeric1to99Type" use="optional"/>
      </xsd:extension>
    </xsd:complexContent>
  </xsd:complexType>
  <xsd:complexType name="RoomAmenityPreferencesType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A collection of room amenity preferences.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="amenity" type="dst:RoomAmenityPreferenceType" minOccurs="0" maxOccurs="unbounded"/>
    </xsd:sequence>
    <xsd:attribute name="verbose" type="xsd:boolean" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">When true, return all details for a room amenity.</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
  </xsd:complexType>
  <xsd:complexType name="RoomAmenitiesType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A collection of room amentities with
                                    optional summary text.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="description" type="xsd:string" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Summary description of room amenities.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="roomAmenity" type="dst:RoomAmenityType" minOccurs="0" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="RoomAmenityType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Represents a room level amenity, for
                                    example, HDTV, coffee maker.</xsd:documentation>
    </xsd:annotation>
    <xsd:complexContent>
      <xsd:extension base="dst:AmenityType">
        <xsd:attribute name="quantity" use="optional" type="cmn:Numeric1to99Type"/>
      </xsd:extension>
    </xsd:complexContent>
  </xsd:complexType>
  <xsd:complexType name="RoomRateCalendarType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Room Rate Calendar</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element ref="cmn:hotelId" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The hotel id for this rate calendar.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element ref="cmn:dateSpan" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The date span of the rate calendar.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element ref="cmn:currencyCode" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The currency code of the amount values in this rate calendar.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element ref="dst:ratePlans" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">A collection of hotel rate plans.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element ref="dst:roomTypes" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">A collection of hotel room types.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="days" minOccurs="1" maxOccurs="1">
        <xsd:complexType>
          <xsd:sequence>
            <xsd:element name="day" minOccurs="1" maxOccurs="unbounded">
              <xsd:annotation>
                <xsd:documentation xml:lang="en">Each day element represents a date/rate plan/room type combination.</xsd:documentation>
              </xsd:annotation>
              <xsd:complexType>
                <xsd:sequence>
                  <xsd:element name="rate" minOccurs="1" maxOccurs="unbounded">
                    <xsd:annotation>
                      <xsd:documentation xml:lang="en">Represents a rate for a specific day and occupancy.</xsd:documentation>
                    </xsd:annotation>
                    <xsd:complexType>
                      <xsd:attribute name="kind" type="dst:RateCalendarRateKindType" use="required">
                        <xsd:annotation>
                          <xsd:documentation xml:lang="en">Classifies this calendar day rate entry.</xsd:documentation>
                        </xsd:annotation>
                      </xsd:attribute>
                      <xsd:attribute name="occupancy" type="xsd:nonNegativeInteger" use="optional">
                        <xsd:annotation>
                          <xsd:documentation xml:lang="en">Describes the occupancy for this rate.</xsd:documentation>
                        </xsd:annotation>
                      </xsd:attribute>
                      <xsd:attribute name="amount" type="xsd:decimal" use="required">
                        <xsd:annotation>
                          <xsd:documentation xml:lang="en">Describes the room rate amount.</xsd:documentation>
                        </xsd:annotation>
                      </xsd:attribute>
                      <xsd:attribute name="taxIncluded" type="xsd:boolean" use="required">
                        <xsd:annotation>
                          <xsd:documentation xml:lang="en">Indicates whether taxes are included in the room rate.</xsd:documentation>
                        </xsd:annotation>
                      </xsd:attribute>
                      <xsd:attribute name="taxAmount" type="xsd:decimal" use="optional">
                        <xsd:annotation>
                          <xsd:documentation xml:lang="en">The tax amount for the room rate.</xsd:documentation>
                        </xsd:annotation>
                      </xsd:attribute>
                    </xsd:complexType>
                  </xsd:element>
                  <xsd:element name="amenityCharge" minOccurs="1" maxOccurs="unbounded">
                    <xsd:annotation>
                      <xsd:documentation xml:lang="en">Represents an amenity charge.</xsd:documentation>
                    </xsd:annotation>
                    <xsd:complexType>
                      <xsd:attribute name="amenityCode" type="dst:AmenityCodeType" use="required">
                        <xsd:annotation>
                          <xsd:documentation xml:lang="en">The amenity code, e.g. CRIB or RLWY</xsd:documentation>
                        </xsd:annotation>
                      </xsd:attribute>
                      <xsd:attribute name="amount" type="xsd:decimal" use="required">
                        <xsd:annotation>
                          <xsd:documentation xml:lang="en">The daily cost of the amenity.</xsd:documentation>
                        </xsd:annotation>
                      </xsd:attribute>
                      <xsd:attribute name="taxIncluded" type="xsd:boolean" use="required">
                        <xsd:annotation>
                          <xsd:documentation xml:lang="en">Indicates whether taxes are included in the amenity amount.</xsd:documentation>
                        </xsd:annotation>
                      </xsd:attribute>
                      <xsd:attribute name="taxAmount" type="xsd:decimal" use="optional">
                        <xsd:annotation>
                          <xsd:documentation xml:lang="en">The tax amount for the amenity.</xsd:documentation>
                        </xsd:annotation>
                      </xsd:attribute>
                    </xsd:complexType>
                  </xsd:element>
                </xsd:sequence>
                <xsd:attribute name="date" type="xsd:date" use="required">
                  <xsd:annotation>
                    <xsd:documentation xml:lang="en">The date for this day in the rate calendar.</xsd:documentation>
                  </xsd:annotation>
                </xsd:attribute>
                <xsd:attribute name="roomTypeCode" type="cmn:StringLength1to32Type" use="required">
                  <xsd:annotation>
                    <xsd:documentation xml:lang="en">The room type code.</xsd:documentation>
                  </xsd:annotation>
                </xsd:attribute>
                <xsd:attribute name="ratePlanCode" type="cmn:StringLength1to32Type" use="required">
                  <xsd:annotation>
                    <xsd:documentation xml:lang="en">The rate plan code.</xsd:documentation>
                  </xsd:annotation>
                </xsd:attribute>
                <xsd:attribute name="availableRooms" type="xsd:nonNegativeInteger" use="required">
                  <xsd:annotation>
                    <xsd:documentation xml:lang="en">The number of available rooms.</xsd:documentation>
                  </xsd:annotation>
                </xsd:attribute>
                <xsd:attribute name="closed" type="xsd:boolean" use="optional">
                  <xsd:annotation>
                    <xsd:documentation xml:lang="en">Set to true if the hotel does not allow any stays for this date.</xsd:documentation>
                  </xsd:annotation>
                </xsd:attribute>
                <xsd:attribute name="closedToArrival" type="xsd:boolean" use="optional">
                  <xsd:annotation>
                    <xsd:documentation xml:lang="en">Set to true if the hotel does not allow arrival for this date.</xsd:documentation>
                  </xsd:annotation>
                </xsd:attribute>
                <xsd:attribute name="blackout" type="xsd:boolean" use="optional">
                  <xsd:annotation>
                    <xsd:documentation xml:lang="en">Set to true if there is no availability for the given rate plan.</xsd:documentation>
                  </xsd:annotation>
                </xsd:attribute>
                <xsd:attribute name="minimumLengthOfStay" type="xsd:nonNegativeInteger" use="optional">
                  <xsd:annotation>
                    <xsd:documentation xml:lang="en">The minimum length of stay for arrival on this date.</xsd:documentation>
                  </xsd:annotation>
                </xsd:attribute>
              </xsd:complexType>
            </xsd:element>
          </xsd:sequence>
        </xsd:complexType>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="RoomRateRangesType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A collection of room rate ranges.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="roomRateRange" type="dst:RoomRateRangeType" minOccurs="0" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="RoomRateRangeType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A collection of room rates.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="minRoomRate" type="dst:RoomRateType" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="maxRoomRate" type="dst:RoomRateType" minOccurs="1" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="RoomRatesType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A collection of room rates.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="roomRate" type="dst:RoomRateType" minOccurs="1" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="RoomRateType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">The RoomRateType is used to associate room
                                    types and rates.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="availabilityStatus" type="dst:RateIndicatorType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Indicates whether RoomRate has
                                      availablity; "AvailableForSale",
                                      "NoAvailability", "Exclusive", 
                                      "InsufficientPoints"</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="bookingCode" type="dst:BookingCodeType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Identifies a bookable product.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="invBlockCode" type="cmn:StringLength1to32Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Code that identifies an inventory block.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="numberOfRooms" type="xsd:integer" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The number of rooms to book.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="numberOfAvailableRooms" type="xsd:integer" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The number of rooms available to book.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element ref="cmn:numberOfGuests" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="rates" minOccurs="0" maxOccurs="1">
        <xsd:complexType>
          <xsd:sequence>
            <xsd:element name="rate" type="dst:RateType" maxOccurs="unbounded">
              <xsd:annotation>
                <xsd:documentation xml:lang="en">An individual rate, which is a
                                         collection of amounts by guest,
                                         additional guests, fees, collection of
                                         related guarantee, cancel and payment
                                         policies, a description and the unique
                                         id to identify the rate. Rate
                                         restrictions can be sent along with the
                                         rate as attributes of this rate. The
                                         indivual rate can also be qualified by
                                         the inventory information
                                         (InventoryGroup attribute group).</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
          </xsd:sequence>
        </xsd:complexType>
      </xsd:element>
      <xsd:element ref="dst:ratePlanCode" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Specfic system rate plan code</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element ref="dst:ratePlanCategory" minOccurs="0" maxOccurs="1">
        <!--TODO remove in CDM 7-->
        <xsd:annotation>
          <xsd:documentation xml:lang="en">*** DEPRECATED *** Specfic system rate plan category type</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element ref="dst:ratePlanCategories" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">A list of rate plan categories to which this rate plan belongs.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="roomRateDescription" type="cmn:StringLength1to255Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Description of the room rate.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="roomTypeCode" type="dst:RoomTypeCodeType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Room type code, e.g., 'K', 'QQ'.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element ref="cmn:roomTypeId" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Specfic system room type code</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="totalAmount" type="cmn:AmountType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Total price for the room rate, for
                                      example, 3 nights at $100 per night for a
                                      King room would total $300</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="averageNightlyRate" type="cmn:AmountType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Average nightly rate for the room</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="nightlyRate" type="cmn:AmountType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Non-averaged nightly rate for the room</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="totalLoyaltyRedemptionAmount" type="dst:LoyaltyRedemptionAmountType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="averageNightlyLoyaltyRedemption" type="dst:LoyaltyRedemptionAmountType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Average nightly loyalty redemption amount for the room</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="validDateRange" type="cmn:DateSpanType" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">This time span is for the entire roomrate
                                      stay. This is different from the RateType
                                      dateRange because there could be multiple
                                      rates over the span of the stay. The total
                                      of all dates in the rates should include
                                      every day in this date span.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
    <xsd:attribute name="rateMode" type="dst:RateModeType" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">A string value to indiacate the returned rate
    								 is of 'highlow' or 'average' rate mode.</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
  </xsd:complexType>
  <xsd:complexType name="RoomTypeSummaryType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Defines a type of room (eg. location,
                                    configuration, view).</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="id" type="cmn:RoomTypeIdType" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Room identifier.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="code" type="dst:RoomTypeCodeType">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Room type code identifier, e.g. 'NHQQ',
                                      'K', 'DD'.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="shortName" type="cmn:StringLength1to16Type" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The hotel defined abbreviation for a Room
                                      type, e.g. 'NHQQ', 'K', 'DD', 'FAMILY'.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="encodedRoomFeatureString" type="cmn:StringLength1to32Type" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Encoded string derived from key room
                                      features (e.g. 'DTT' = one double and two
                                      twin beds, 'SQ' = smoking queen)</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="smoking" type="xsd:boolean" default="false" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Smoking indicator. Default value is false.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="accessibility" type="dst:RoomAccessibilityType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="numberOfRooms" type="cmn:Numeric1to999Type" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Total number of this room type.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="numberOfBeds" type="cmn:Numeric1to999Type" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Total number of beds in this room type.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="maximumOccupancy" type="cmn:Numeric1to999Type" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Maximum occupancy count for this room type.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="amenities" type="dst:RoomAmenitiesType" minOccurs="0" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="RoomTypesType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A collection of room types.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="roomType" type="dst:RoomTypeType" minOccurs="1" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="RoomTypeCodeType">
    <xsd:sequence>
      <xsd:element name="code" type="cmn:StringLength1to8Type">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Room type code identifier, e.g. 'NHQQ',
                                      'K', 'DD'.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="RoomTypeType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Defines a type of room (eg. location,
                                    configuration, view).</xsd:documentation>
    </xsd:annotation>
    <xsd:complexContent>
      <xsd:extension base="dst:RoomTypeSummaryType">
        <xsd:sequence>
          <xsd:element name="customDescription" type="cmn:StringLength1to255Type" minOccurs="0">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">Customizable description of this room
                                        type.</xsd:documentation>
            </xsd:annotation>
          </xsd:element>
          <xsd:element name="description" type="xsd:string" minOccurs="0">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">Standard description of this room type.</xsd:documentation>
            </xsd:annotation>
          </xsd:element>
          <xsd:element name="beds" type="dst:BedsType" minOccurs="0">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">Indicates the type of bed(s) found in
                                        the room.</xsd:documentation>
            </xsd:annotation>
          </xsd:element>
          <xsd:element name="efficiency" type="xsd:boolean" default="false" minOccurs="0">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">Efficiencies configured indicator.
                                        Default value is false.</xsd:documentation>
            </xsd:annotation>
          </xsd:element>
          <xsd:element name="suite" type="xsd:boolean" default="false" minOccurs="0">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">Room is a suite. Default value is false.</xsd:documentation>
            </xsd:annotation>
          </xsd:element>
          <xsd:element name="extraBed" type="xsd:boolean" default="false" minOccurs="0">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">Room contains an extra bed. Default
                                        value is false.</xsd:documentation>
            </xsd:annotation>
          </xsd:element>
          <xsd:element name="upgraded" type="xsd:boolean" default="false" minOccurs="0">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">Room has been upgraded. Default value is
                                        false.</xsd:documentation>
            </xsd:annotation>
          </xsd:element>
          <xsd:element name="promotional" type="xsd:boolean" default="false" minOccurs="0">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">Room is under promotion. Default value
                                        is false.</xsd:documentation>
            </xsd:annotation>
          </xsd:element>
          <xsd:element name="brandSpecificRoomTypeDescriptor" type="dst:BrandSpecificRoomDescriptorType" minOccurs="0" maxOccurs="1"/>
          <xsd:element name="sizeMeasurement" type="xsd:string" minOccurs="0">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">Textual description of room dimensions.</xsd:documentation>
            </xsd:annotation>
          </xsd:element>
          <xsd:element name="gdsSellable" type="xsd:boolean" default="false" minOccurs="0">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">Room is sellable in the GDS. Default
                                        value is false. *** DEPRECATED *** This
                                        element is deprecated since it doesn't
                                        exist to define a room type but instead
                                        is used to filter room types. This
                                        element will be removed once a room type
                                        filtering service is available.</xsd:documentation>
            </xsd:annotation>
          </xsd:element>
        </xsd:sequence>
        <xsd:attribute name="gdsSequence" type="xsd:nonNegativeInteger" use="optional">
          <xsd:annotation>
            <xsd:documentation xml:lang="en">GDS sequencing value.</xsd:documentation>
          </xsd:annotation>
        </xsd:attribute>
      </xsd:extension>
    </xsd:complexContent>
  </xsd:complexType>
  <xsd:complexType name="RoomStayType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Describes a stay (proposed, reserved or completed)
                                    at a specific hotel.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="checkInOutDate" type="cmn:DateSpanType" minOccurs="1" maxOccurs="1"/>
      <xsd:element ref="dst:ratePlan" minOccurs="0" maxOccurs="1"/>
      <xsd:element ref="dst:roomType" minOccurs="0" maxOccurs="1"/>
      <xsd:element ref="cmn:numberOfGuests" minOccurs="0" maxOccurs="1"/>
      <xsd:element ref="dst:roomRate" minOccurs="0" maxOccurs="1">
        <!--TODO remove in CDM 7-->
        <xsd:annotation>
          <xsd:documentation xml:lang="en">*** DEPRECATED ***
                                      Use roomRates instead.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element ref="dst:roomRates" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="totalLoyaltyRedemptionAmount" type="spt:LoyaltyRedemptionType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="totalAmount" type="dst:HotelStayTotalAmountType" minOccurs="0" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="RoomViewType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Represents room views, for example, beach
                                    front, lake, pool.</xsd:documentation>
    </xsd:annotation>
    <xsd:complexContent>
      <xsd:extension base="dst:AmenityType"/>
    </xsd:complexContent>
  </xsd:complexType>
  <xsd:complexType name="SalesContactsType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A set of sales contacts</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="primaryContact" type="dst:SalesContactType" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="otherContact" type="dst:SalesContactType" minOccurs="0" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="SalesContactType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Describes a person who has been engaged by
                                    the sales staff</xsd:documentation>
    </xsd:annotation>
    <xsd:complexContent>
      <xsd:extension base="cmn:PersonContactType">
        <xsd:sequence>
          <xsd:element name="title" type="cmn:StringLength1to64Type" minOccurs="0" maxOccurs="1">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">Job title or functioal title of the
                                        contact</xsd:documentation>
            </xsd:annotation>
          </xsd:element>
          <xsd:element name="organization" minOccurs="0" maxOccurs="1">
            <xsd:complexType>
              <xsd:sequence>
                <xsd:element name="name" type="cmn:StringLength1to64Type" minOccurs="1" maxOccurs="1"/>
                <xsd:element name="website" type="cmn:UrlType" minOccurs="0" maxOccurs="1"/>
              </xsd:sequence>
            </xsd:complexType>
          </xsd:element>
          <xsd:element name="additionalInfo" type="xsd:string" minOccurs="0" maxOccurs="1"/>
        </xsd:sequence>
      </xsd:extension>
    </xsd:complexContent>
  </xsd:complexType>
  <xsd:complexType name="ShoppingCategoryType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A shopping category used for rate plan
                                    association.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="code" type="cmn:StringLength1to8Type" minOccurs="1" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="ShoppingCategoriesType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A collection of shopping categories.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="shoppingCategory" type="dst:ShoppingCategoryType" minOccurs="1" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="SingleHotelAvailabilityType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Represents room availablity for a given hotel.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element ref="cmn:hotelId" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="checkInOutDate" type="cmn:DateSpanType" minOccurs="1" maxOccurs="1"/>
      <xsd:element ref="dst:ratePlans" minOccurs="0" maxOccurs="1"/>
      <xsd:element ref="dst:roomTypes" minOccurs="0" maxOccurs="1"/>
      <xsd:element ref="cmn:numberOfGuests" minOccurs="0" maxOccurs="1"/>
      <xsd:element ref="dst:roomRates" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="availabilityStatus" type="dst:RateIndicatorType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="cancelPolicies" type="dst:CancelPoliciesType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="guaranteeOptions" type="dst:GuaranteesType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="totalAmount" type="dst:HotelStayTotalAmountType" minOccurs="0" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="SplitCommissionDistributionListType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A list of distributions for a split
                                    commission.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="distribution" type="dst:SplitCommissionDistributionType" minOccurs="1" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="SplitCommissionDistributionType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Specifies the distribution of a split
                                    commission with another travel agent or
                                    account.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="recipient" minOccurs="1" maxOccurs="1">
        <xsd:complexType>
          <xsd:choice>
            <xsd:element ref="cmn:accountId" minOccurs="1" maxOccurs="1"/>
            <xsd:element ref="cmn:travelAgentId" minOccurs="1" maxOccurs="1"/>
          </xsd:choice>
        </xsd:complexType>
      </xsd:element>
      <xsd:element name="percentage" type="cmn:PercentType" minOccurs="1" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="SplitCommissionType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Describes an amount that is payable as part
                                    of a sales agreement to multiple recipients.</xsd:documentation>
    </xsd:annotation>
    <xsd:complexContent>
      <xsd:extension base="dst:CommissionType">
        <xsd:sequence>
          <xsd:element name="distributionList" type="dst:SplitCommissionDistributionListType" minOccurs="0" maxOccurs="1"/>
        </xsd:sequence>
      </xsd:extension>
    </xsd:complexContent>
  </xsd:complexType>
  <xsd:simpleType name="AcceptedPaymentFormCodeType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A code representing a form of payment.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to4Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="AcceptedPaymentFormKindType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Classifies a payment method (e.g., LoyaltyRedemption,
                                    GiftCard, PaymentCard, Cash, Voucher, Coupon, Invoice).</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to16Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="AmenityCodeType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">The reference code for an amenity.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to16Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="ArrivalTransportationType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Type of transport used</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:string">
      <xsd:enumeration value="Air"/>
      <xsd:enumeration value="Rail"/>
      <xsd:enumeration value="Bus"/>
      <xsd:enumeration value="Boat"/>
      <xsd:enumeration value="Private"/>
      <xsd:enumeration value="Auto"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="BookingCodeType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Identifies a bookable product (room type and
                                    rate plan).</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to16Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="BookingLimitMessageKindType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">An enumerated type defining the function of
                                    the booking limit message. Values:
                                    RemoveLimit, SetLimit, AdjustLimit.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to16Type">
      <xsd:enumeration value="RemoveLimit"/>
      <xsd:enumeration value="SetLimit"/>
      <xsd:enumeration value="AdjustLimit"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="BrandSpecificRoomDescriptorType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A word or phrase that is used to describe a
                                    room type in a way that is specific to how a
                                    brand wants to market the room type (e.g.,
                                    'Business Room', 'Rodeway Choice Room',
                                    'Clarion Class Leisure Room').</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to32Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="CancellationRefundAmountType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Used to specify the cancellation amount.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to32Type">
      <xsd:enumeration value="FirstNightDeposit">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Amount to be applied as a deposit for the
                                      first night.</xsd:documentation>
        </xsd:annotation>
      </xsd:enumeration>
      <xsd:enumeration value="LastNightDepost">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Amount to be applied as a deposit for the
                                      last night.</xsd:documentation>
        </xsd:annotation>
      </xsd:enumeration>
      <xsd:enumeration value="FirstAndLastNightDeposit">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Amount to be applied as a deposit for the
                                      first and last nights.</xsd:documentation>
        </xsd:annotation>
      </xsd:enumeration>
      <xsd:enumeration value="FirstNightPayment">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Amount to be applied as payment for the
                                      first night.</xsd:documentation>
        </xsd:annotation>
      </xsd:enumeration>
      <xsd:enumeration value="LastNightPayment">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Amount to be applied as payment for the
                                      last night.</xsd:documentation>
        </xsd:annotation>
      </xsd:enumeration>
      <xsd:enumeration value="FirstAndLastNightPayment">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Amount to be applied as payment for the
                                      first and last nights.</xsd:documentation>
        </xsd:annotation>
      </xsd:enumeration>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="DayOfWeekPatternType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">This represents the days of the week that
                                    the associated item is available. The range
                                    is from Mon - Sun. A 'Y' means the item is
                                    available and a 'N' means it is not
                                    available. (e.g., "NNNNYYY" means the item
                                    is only available on Friday, Saturday, and
                                    Sunday.)</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:string">
      <xsd:pattern value="[YN][YN][YN][YN][YN][YN][YN]"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="DistributionChannelKindType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Classifies distribution channels (e.g., GDS, OTA,
                                    Intermediate, Hotel, CallCenter, Website, Mobile).</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to16Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="DistributionPartnerCodeType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A 2-character code representing a distribution
                                    partner. This is the airline code (e.g., AA, DL, US),
                                    a GDS code (e.g., 1A, 1G) or an OTA code (e.g., DS).</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:string">
      <xsd:pattern value="[A-Za-z0-9]{2}"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="DistributionPartnerKindType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A classifier of a distribution partner
                                    (e.g., Airline, GDS, OTA, Intermediate).</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to16Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="EmployeeDiscountRateLoadLevelType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Indicates the rate load level for
                                    employee discount rates such as SED and
                                    LFF. Possible values include:
                                    "Based on ADR", "Lowest Rate",
                                    "Medium Level Rate", "Highest Rate".</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to32Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="FeeTaxCodeType">
    <xsd:restriction base="xsd:string">
      <xsd:enumeration value="Bed Tax"/>
      <xsd:enumeration value="Occupancy Tax"/>
      <xsd:enumeration value="Package Fee"/>
      <xsd:enumeration value="Resort Fee"/>
      <xsd:enumeration value="Sales Tax"/>
      <xsd:enumeration value="Service Charge"/>
      <xsd:enumeration value="Total Tax"/>
      <xsd:enumeration value="State Tax"/>
      <xsd:enumeration value="Surcharge"/>
      <xsd:enumeration value="Tourism Tax"/>
      <xsd:enumeration value="VAT/GST Tax"/>
      <xsd:enumeration value="City Hotel Fee"/>
      <xsd:enumeration value="Standard"/>
      <xsd:enumeration value="Room Tax"/>
      <xsd:enumeration value="Early Checkout Fee"/>
      <xsd:enumeration value="City Tax"/>
      <xsd:enumeration value="Country Tax"/>
      <xsd:enumeration value="Banquet Service Fee"/>
      <xsd:enumeration value="Local Fee"/>
      <xsd:enumeration value="Crib Fee"/>
      <xsd:enumeration value="Rollaway Fee"/>
      <xsd:enumeration value="County Tax"/>
      <xsd:enumeration value="Pet Fee"/>
      <xsd:enumeration value="Federal Tax"/>
      <xsd:enumeration value="Food and Beverage Tax"/>
      <xsd:enumeration value="Lodging Tax"/>
      <xsd:enumeration value="Maintenance Fee"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="GuestAgeCategoryType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Classifies the age of a guest (e.g., Adult, Infant,
                                    Child, Senior). This is similar to the OTA age
                                    qualifying code (AQC).</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to16Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="HotelStatusType">
    <xsd:restriction base="xsd:string">
      <xsd:enumeration value="New"/>
      <xsd:enumeration value="Active"/>
      <xsd:enumeration value="Inactive"/>
      <xsd:enumeration value="Terminated"/>
      <xsd:enumeration value="Suspended"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="LengthOfStayType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Used for basic LOS values.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:nonNegativeInteger"/>
  </xsd:simpleType>
  <xsd:simpleType name="PseudoCityCodeType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A code used to identify a travel agent location.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to32Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="RateManagementStrategyType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Indicates the rate management strategy used
                                    for a hotel (e.g., BAR, STANDARD).</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to32Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="RateModeType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A string that indicates the type of rates to be returned
   									in the RoomRateRanges. Possible values are 'highlow' and
   									'average. 'highlow' returns non-averaged min/max rates
   									and 'average' provides averaged min/max rates.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to16Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="RatePlanAccessCodeType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A code used to gain access to a rate plan.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to16Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="RateCalendarRateKindType">
    <xsd:annotation>
      <xsd:documentation>Classifies a rate calendar rate (e.g, StandardOccupancy,
                      ExtraPerson).</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to32Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="RateIndicatorType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">An enumerated type indicating special
                                    conditions with the rate. Derived from OTA.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to32Type">
      <xsd:enumeration value="ChangeDuringStay"/>
      <xsd:enumeration value="MultipleNights"/>
      <xsd:enumeration value="Exclusive">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Availability is limited based on guest
                                      qualification criteria e.g. AAA member or
                                      Government Employee</xsd:documentation>
        </xsd:annotation>
      </xsd:enumeration>
      <xsd:enumeration value="OnRequest"/>
      <xsd:enumeration value="LimitedAvailability"/>
      <xsd:enumeration value="AvailableForSale"/>
      <xsd:enumeration value="ClosedOut"/>
      <xsd:enumeration value="OtherAvailable"/>
      <xsd:enumeration value="UnableToProcess">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Indicates an issue that precluded the
                                      ability to provide the information.</xsd:documentation>
        </xsd:annotation>
      </xsd:enumeration>
      <xsd:enumeration value="NoAvailability"/>
      <xsd:enumeration value="RoomTypeClosed"/>
      <xsd:enumeration value="RatePlanClosed"/>
      <xsd:enumeration value="LOS_Restricted"/>
      <xsd:enumeration value="Restricted">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Availability is limited based on
                                      distribution channel qualification
                                      criteria (e.g., Expedia or Sabre).</xsd:documentation>
        </xsd:annotation>
      </xsd:enumeration>
      <xsd:enumeration value="DoesNotExist">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The rate plan does not exist.</xsd:documentation>
        </xsd:annotation>
      </xsd:enumeration>
      <xsd:enumeration value="InsufficientPoints"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="RatePlanKindType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Identifies a Rate Plan Type.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to4Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="RateTierType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">The tier that the rate falls into.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to16Type">
      <xsd:enumeration value="High"/>
      <xsd:enumeration value="Medium"/>
      <xsd:enumeration value="Low"/>
      <xsd:enumeration value="Standard"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="RestrictionType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Type of status change.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to16Type">
      <xsd:enumeration value="Master"/>
      <xsd:enumeration value="Arrival"/>
      <xsd:enumeration value="Departure"/>
      <xsd:enumeration value="NonGuarantee"/>
      <xsd:enumeration value="TravelAgent"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="RoomAccessibilityType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Type of disabled access provided by a room
                                    (e.g., 'Non-accessible', 'Mobility
                                    Accessible', 'Hearing Accessible', 'Mobility
                                    and Hearing Accessible').</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to32Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="StatusType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Identifies the availability status of an
                                    item.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to32Type">
      <xsd:enumeration value="Open">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Inventory is available for sale.</xsd:documentation>
        </xsd:annotation>
      </xsd:enumeration>
      <xsd:enumeration value="Close">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Inventory is not available for sale.</xsd:documentation>
        </xsd:annotation>
      </xsd:enumeration>
      <xsd:enumeration value="ClosedOnArrival">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Inventory is not available for sale to
                                      arriving guests.</xsd:documentation>
        </xsd:annotation>
      </xsd:enumeration>
      <xsd:enumeration value="OpenWithMinimumLengthOfStay">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Roomtype is open but only if the stay
                                      equals or exceeds a min length of stay.</xsd:documentation>
        </xsd:annotation>
      </xsd:enumeration>
      <xsd:enumeration value="ClosedOnArrivalOnRequest">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Inventory may not be available for sale to
                                      arriving guests.</xsd:documentation>
        </xsd:annotation>
      </xsd:enumeration>
      <xsd:enumeration value="OnRequest">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Inventory may be available.</xsd:documentation>
        </xsd:annotation>
      </xsd:enumeration>
      <xsd:enumeration value="RemoveClosedOnly">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Remove Close restriction while keeping
                                      other restrictions in place.</xsd:documentation>
        </xsd:annotation>
      </xsd:enumeration>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:attributeGroup name="AgeQualifyingGroup">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Age group of occupants for which this rate
                                    is valid.</xsd:documentation>
    </xsd:annotation>
    <xsd:attribute name="minAge" type="cmn:Numeric1to999Type" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">MinAge: The minimum age to qualify for
                                     AgeQualifyingCode.</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
    <xsd:attribute name="maxAge" type="cmn:Numeric1to999Type" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">Max Age: The maximum age to qualify for
                                     AgeQualifyingCode.</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
    <xsd:attribute name="ageCategory" type="dst:GuestAgeCategoryType" use="optional"/>
  </xsd:attributeGroup>
</xsd:schema>]]></con:content>
        <con:type>http://www.w3.org/2001/XMLSchema</con:type>
      </con:part>
      <con:part>
        <con:url>http://esb.services.ext.pci.qa.chotel.com:80/HotelDistributionService/v6?SCHEMA%2FCdm_Shared_v6%2Fxsd%2Fsupport%2FPayment</con:url>
        <con:content><![CDATA[<!--Document: The Payment schema contains schema types
          used to create and manage payment information.

Date: 01-05-2011
Last Updated: 11-19-2014
Authors: Chris Judson, Kirk Damron, Andrew Baker, Daniel Gonzalez, Niall Broderick-->
<xsd:schema targetNamespace="http://www.choicehotels.com/schema/v6/support/cdm" elementFormDefault="qualified" attributeFormDefault="unqualified" xml:lang="en" xmlns:spt="http://www.choicehotels.com/schema/v6/support/cdm" xmlns:cmn="http://www.choicehotels.com/schema/v6/common/cdm" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <xsd:import namespace="http://www.choicehotels.com/schema/v6/common/cdm" schemaLocation="http://esb.services.ext.pci.qa.chotel.com:80/HotelDistributionService/v6?SCHEMA%2FCdm_Shared_v6%2Fxsd%2Fcommon%2FCommonTypes"/>
  <xsd:element name="cashValueCoupon" type="spt:CashValueCouponType"/>
  <xsd:element name="cashValueCouponId" type="spt:CashValueCouponIdType"/>
  <xsd:element name="creditCancellation" type="spt:CreditCancellationType"/>
  <xsd:element name="loyaltyRedemption" type="spt:LoyaltyRedemptionType"/>
  <xsd:element name="paymentAmount" type="spt:PaymentAmountType"/>
  <xsd:element name="paymentCancellation" type="spt:PaymentCancellationType"/>
  <xsd:element name="paymentCard" type="spt:PaymentCardType"/>
  <xsd:element name="paymentCardAuthorization" type="spt:PaymentCardAuthorizationType"/>
  <xsd:element name="paymentCardCharge" type="spt:PaymentCardChargeType"/>
  <xsd:element name="paymentCardInquiry" type="spt:PaymentCardInquiryType"/>
  <xsd:element name="paymentCardIssuance" type="spt:PaymentCardIssuanceType"/>
  <xsd:element name="paymentCardIssuanceConfiguration" type="spt:PaymentCardIssuanceConfigurationType"/>
  <xsd:element name="paymentCardNumberPrefixRange" type="spt:PaymentCardNumberPrefixRangeType"/>
  <xsd:element name="paymentCardNumberPrefixRanges" type="spt:PaymentCardNumberPrefixRangesType"/>
  <xsd:element name="paymentCardList" type="spt:PaymentCardListType"/>
  <xsd:element name="paymentCardNumberList" type="spt:PaymentCardNumberListType"/>
  <xsd:element name="paymentCardTransaction" type="spt:PaymentCardTransactionType"/>
  <xsd:element name="paymentDetokenizeAuditEntry" type="spt:PaymentDetokenizeAuditEntryType"/>
  <xsd:element name="paymentForm" type="spt:PaymentFormType"/>
  <xsd:element name="payments" type="spt:PaymentsType"/>
  <xsd:element name="paymentCardTransactionDescriptiveInfo" type="spt:PaymentCardTransactionDescriptiveInfoType"/>
  <xsd:element name="merchantTransactionAuthorization" type="spt:MerchantTransactionAuthorizationType"/>
  <xsd:element name="voucher" type="spt:VoucherType"/>
  <xsd:complexType name="CashValueCouponIdType">
    <xsd:sequence>
      <xsd:element name="id" type="xsd:positiveInteger" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation>Unique identifier for a cash value coupon.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="CashValueCouponType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A Cash Value Coupon (CVC) is issued by Guest
                                    Relations as compensation resulting from the
                                    resolution of a guest complaint.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element ref="spt:cashValueCouponId"/>
      <xsd:element name="denomination" type="cmn:CurrencyAmountType" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation>The face value of the coupon.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="issueDate" type="xsd:date" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation>Date the coupon was issued.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="expireDate" type="xsd:date" maxOccurs="1" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation>Date the coupon expired or was made invalid.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="consumeDate" type="xsd:date" maxOccurs="1" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation>Date the coupon was consumed.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="CreditCancellationType">
    <xsd:sequence>
      <xsd:element name="transactionId" type="spt:PaymentTransactionIdType" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="timeStamp" type="xsd:dateTime" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="amount" type="cmn:CurrencyAmountType" minOccurs="0" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="LoyaltyRedemptionType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Describes the essentials needed to consume value from a loyalty
                                    account.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element ref="cmn:loyaltyAccountId" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Identifies the loyalty account from which the amount is to be
                                      consumed.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="amount" type="cmn:NonNegativeDecimal" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Amount to be consumed.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="deltaAmount" type="xsd:decimal" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Difference between amount redeemed in this transaction and 
                                      the amount redeemed in the most recent previous transaction.
                                      Let A[current] = amount of the current transaction and
                                      let A[prev] = amount of the previous transaction then
                                      delta = A[current] - A[prev].
                                      
                                      Example 1: A member books a one night stay at 8000 points
                                      per night for a total of 8000 points. Then, sometime later
                                      adds another night to the stay for a total of 16000 points.
                                      The delta is A[current] - A[prev] = 16000 - 8000 = 8000 points.
                                      
                                      Example 2: A member orders three gift cards for 10000 points
                                      each for a total of 30000 points. Then, changes his mind
                                      (prior to fulfillment) and removes two gift cards from his
                                      order for a total of 10000 points. The delta is
                                      10000 - 30000 = -20000 points.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="loyaltyValuePurchased" type="spt:LoyaltyValuePurchasedType" minOccurs="0" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="LoyaltyValuePurchasedType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Describes a transaction to purchase a loyalty asset.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="amount" type="cmn:NonNegativeDecimal" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Amount of loyalty value purchased.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="purchasePrice" type="cmn:AmountType" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Purchase price of the loyalty value</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
    <xsd:attribute name="transactionId" type="spt:PaymentTransactionIdType" use="required">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">The payment transaction identifier for this purchase.</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
  </xsd:complexType>
  <xsd:complexType name="MerchantTransactionAuthorizationType">
    <xsd:annotation>
      <xsd:documentation>The credentials used to signify a transaction has been certified by
                      someone with authority on the merchant side. A common use-case is
                      for a supervisor to approve a refund so that fraud or misuse can be
                      avoided.</xsd:documentation>
    </xsd:annotation>
    <xsd:complexContent>
      <xsd:extension base="cmn:UserCredentialsType"/>
    </xsd:complexContent>
  </xsd:complexType>
  <xsd:complexType name="MerchantTransactionType">
    <xsd:annotation>
      <xsd:documentation>Describes a transaction to purchase items from a merchant.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="merchantTransactionId" type="spt:MerchantTransactionIdType" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="timeStamp" type="xsd:dateTime" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="loyaltyAccountId" type="cmn:LoyaltyAccountIdType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="purchasedProducts" type="spt:PurchasedProductsType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="merchantTransactionKind" type="spt:MerchantTransactionKindType" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="referenceId" type="cmn:StringLength1to64Type" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="businessUnit" type="cmn:StringLength1to64Type" minOccurs="0" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="PaymentAmountType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Describes the amount of a payment.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="totalAmount" type="cmn:CurrencyAmountType" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="amountComposition" minOccurs="0" maxOccurs="1">
        <xsd:complexType>
          <xsd:annotation>
            <xsd:documentation xml:lang="en">Describes the individual items that make
                                       up the total amount of a payment
                                       transaction (e.g., tax, tip, fee).</xsd:documentation>
          </xsd:annotation>
          <xsd:sequence>
            <xsd:element name="component" minOccurs="1" maxOccurs="unbounded">
              <xsd:complexType>
                <xsd:sequence>
                  <xsd:element name="name" type="cmn:StringLength1to32Type" minOccurs="0" maxOccurs="1"/>
                  <xsd:element name="code" type="cmn:StringLength1to16Type" minOccurs="0" maxOccurs="1"/>
                  <xsd:element name="amount" type="cmn:CurrencyAmountType" minOccurs="1" maxOccurs="1"/>
                </xsd:sequence>
              </xsd:complexType>
            </xsd:element>
          </xsd:sequence>
        </xsd:complexType>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="PaymentCancellationType">
    <xsd:sequence>
      <xsd:element name="transactionId" type="spt:PaymentTransactionIdType" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="timeStamp" type="xsd:dateTime" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="amount" type="cmn:CurrencyAmountType" minOccurs="0" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="PaymentCardAuthorizationType">
    <xsd:sequence>
      <xsd:element name="paymentCard" type="spt:PaymentCardType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="authorizationId" type="spt:PaymentAuthorizationIdType" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="transactionId" type="spt:PaymentTransactionIdType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="timeStamp" type="xsd:dateTime" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="expiration" type="xsd:dateTime" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="amount" type="cmn:CurrencyAmountType" minOccurs="0" maxOccurs="1"/>
    </xsd:sequence>
    <xsd:attribute name="manualAuthorization" type="xsd:boolean" use="optional"/>
  </xsd:complexType>
  <xsd:complexType name="PaymentCardChargeType">
    <xsd:sequence>
      <xsd:element name="paymentCard" type="spt:PaymentCardType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="token" type="cmn:PaymentCardTokenType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="authorizationId" type="spt:PaymentAuthorizationIdType" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="transactionId" type="spt:PaymentTransactionIdType" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="timeStamp" type="xsd:dateTime" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="amount" type="cmn:CurrencyAmountType" minOccurs="1" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="PaymentCardCreditType">
    <xsd:sequence>
      <xsd:element name="paymentCard" type="spt:PaymentCardType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="token" type="cmn:PaymentCardTokenType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="authorizationId" type="spt:PaymentAuthorizationIdType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="transactionId" type="spt:PaymentTransactionIdType" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="timeStamp" type="xsd:dateTime" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="amount" type="cmn:CurrencyAmountType" minOccurs="1" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="PaymentCardIssuanceConfigurationType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">The set of payment card issuances used for
                                    validation of card numbers.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="paymentCardIssuance" type="spt:PaymentCardIssuanceType" minOccurs="0" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="PaymentCardIssuanceType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Describes a collection of payment cards
                                    issued by an entity.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="issuer" type="spt:PaymentCardIssuerType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="cardCode" type="cmn:PaymentCardCodeType" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="cobranded" type="xsd:boolean" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Card is issued under a co-branded marketing scheme.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="product" type="spt:PaymentCardProductType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="numberRanges" type="spt:PaymentCardNumberPrefixRangesType" minOccurs="1" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="PaymentCardNumberPrefixRangesType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A collection of payment card number prefix ranges.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="range" type="spt:PaymentCardNumberPrefixRangeType" minOccurs="1" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="PaymentCardNumberPrefixRangeType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A payment card number prefix range. This is typically 
                                    used for the IIN range. It could be a longer prefix
                                    to represent a specific number allocation for an
                                    issuer as in the case of a cobranded card.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="begin" type="spt:PaymentCardNumberPrefixType" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Lowest inclusive value of the prefix range.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="end" type="spt:PaymentCardNumberPrefixType" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Highest inclusive value of the prefix range.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="minLength" type="cmn:Numeric1to99Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Mininum length of the full card number.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="maxLength" type="cmn:Numeric1to99Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Maximum length of the full card number.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="checkAlgorithm" type="cmn:StringLength1to64Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Name of the algorithm used to validate a
                                      payment card number in this range.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="PaymentCardInquiryType">
    <xsd:sequence>
      <xsd:element name="processorId" type="spt:PaymentProcessorIdType" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="processorAccessToken" type="cmn:StringLength1to64Type" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="businessTransactionKind" type="spt:BusinessTransactionKindType" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="paymentCard" type="spt:PaymentCardType" minOccurs="1" maxOccurs="1"/>
      <xsd:element ref="spt:paymentCardTransactionDescriptiveInfo" minOccurs="0" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="PaymentCardIssuerType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Describes an entity that issues payment
                                    cards.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="name" type="cmn:StringLength1to32Type" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Name of bank issuing the card.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
    <xsd:attribute name="bankId" type="cmn:StringLength1to64Type" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">Code of bank issuing the card.</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
  </xsd:complexType>
  <xsd:complexType name="PaymentCardListType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A list of payment cards.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element ref="spt:paymentCard" minOccurs="0" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="PaymentCardType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Identification about a specific credit card.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="cardHolderName" type="cmn:StringLength1to64Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Name of the card holder.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="billingAddress" type="cmn:AddressType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Card holder's address used for additional
                                      authorization checks.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element ref="cmn:phone" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation>Card holder's telephone number used for additional
                        authorization checks.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="cardIssuer" type="spt:PaymentCardIssuerType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="cobranded" type="xsd:boolean" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Card is issued under a co-branded marketing scheme.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="product" type="spt:PaymentCardProductType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="cardCode" type="cmn:PaymentCardCodeType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="paymentCardNumber" type="cmn:PaymentCardNumberType" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="effectiveDate" type="cmn:MMYYDateType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Indicates the effective date of the card.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="expireDate" type="cmn:MMYYDateType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Indicates the cards expiration date.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="expireDateEncrypted" type="cmn:StringLength1to64Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The cards expiration date after it has
                                      been encrypted.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="securityCode" type="cmn:NumericStringLength1to8Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Verification digits printed on the card
                                      following the embossed number. This may
                                      also accommodate the customer
                                      identification/batch number (CID), card
                                      verification value (CVV2 ), card
                                      validation code number (CVC2) on credit
                                      card. DO NOT store this data anywhere, it
                                      is for transmit ONLY.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="trackData" type="cmn:StringLength1to255Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Data from the magnetic stripe. DO NOT
                                      store this data anywhere, it is for
                                      transmit ONLY.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
    <xsd:attribute name="paymentCardKind" type="spt:PaymentCardKindType" use="optional"/>
  </xsd:complexType>
  <xsd:complexType name="PaymentCardNumberListType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A list of payment card numbers.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element ref="cmn:paymentCardNumber" minOccurs="0" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="PaymentCardTransactionType">
    <xsd:sequence>
      <xsd:element name="processorId" type="spt:PaymentProcessorIdType" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="processorAccessToken" type="cmn:StringLength1to64Type" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="businessTransactionKind" type="spt:BusinessTransactionKindType" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="paymentCard" type="spt:PaymentCardType" minOccurs="0" maxOccurs="1"/>
      <xsd:element ref="spt:paymentAmount" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="authorization" type="spt:PaymentCardAuthorizationType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="transactionId" type="spt:PaymentTransactionIdType" minOccurs="0" maxOccurs="1"/>
      <xsd:element ref="spt:merchantTransactionAuthorization" minOccurs="0" maxOccurs="1"/>
      <xsd:element ref="spt:paymentCardTransactionDescriptiveInfo" minOccurs="0" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="PaymentDetokenizeAuditEntryType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Fields specific to the
			auditing of Detokenize requests.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="clientApplication" type="cmn:StringLength1to64Type" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation>The application calling the service.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="clientApplicationNetworkAddress" type="cmn:IPAddressType" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation>The IP address of the machine running the
					clientApplication.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="endUserName" type="cmn:UsernameType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation>The username of the person requesting the credit
					card number from the application.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="endUserNetworkAddress" type="cmn:IPAddressType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation>The IP address of the machine calling the
					clientApplication.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="tokens" type="spt:PaymentCardNumberListType" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation>Tokens to be detokenized.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="PaymentFormType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Ways of providing funds and guarantees for
                                    travel by the individual.</xsd:documentation>
    </xsd:annotation>
    <xsd:choice minOccurs="0">
      <xsd:element ref="spt:paymentCard">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Details of a debit or credit card.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element ref="spt:cashValueCouponId">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Identifier of a cash value coupon.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element ref="spt:voucher">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Details of a paper or electronic document
                                      indicating prepayment.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element ref="spt:loyaltyRedemption">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Used to indicate payment with loyalty
                                      points.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="cash">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Used to indicate payment in cash.</xsd:documentation>
        </xsd:annotation>
        <xsd:complexType>
          <xsd:attribute name="cashIndicator" type="xsd:boolean" use="optional">
            <xsd:annotation>
              <xsd:documentation xml:lang="en">If true, this indicates cash is being
                                        used.</xsd:documentation>
            </xsd:annotation>
          </xsd:attribute>
        </xsd:complexType>
      </xsd:element>
    </xsd:choice>
    <xsd:attribute name="paymentTransactionTypeCode" type="spt:PaymentTransactionTypeCodeType" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">This is used to indicate either a charge,
                                     reserve (deposit) or refund.</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
    <xsd:attribute name="guaranteeIndicator" type="xsd:boolean" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">When true, indicates this is exclsively a
                                     guarantee. When false, indicates it is a
                                     payment (which may imply guarantee). The
                                     implication when true is that no funds will
                                     be consumed (e.g., credit card will not be
                                     charged).</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
    <xsd:attribute name="guaranteeKindCode" type="cmn:GuaranteeKindCodeType" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">Used to specify the method of guarantee.</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
    <xsd:attribute name="guaranteeId" type="cmn:StringLength1to64Type" use="optional">
      <xsd:annotation>
        <xsd:documentation xml:lang="en">Provides the identifier as specified by the
                                     GuaranteeTypeCode (e.g., Corporate ID or
                                     IATA number).</xsd:documentation>
      </xsd:annotation>
    </xsd:attribute>
    <xsd:attribute name="paymentProcessorId" type="spt:PaymentProcessorIdType" use="optional"/>
    <xsd:attribute name="paymentAuthorizationId" type="spt:PaymentAuthorizationIdType" use="optional"/>
  </xsd:complexType>
  <xsd:complexType name="PaymentsType">
    <xsd:sequence>
      <xsd:element name="payment" type="spt:PaymentType" minOccurs="1" maxOccurs="unbounded">
        <xsd:annotation>
          <xsd:documentation>Collection of payments which supports having multiple
                        payment forms each having different amounts.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="PaymentType">
    <xsd:sequence>
      <xsd:element ref="spt:paymentForm" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="paymentAmount" type="cmn:CurrencyAmountType" minOccurs="1" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation>Monetary amount of the payment. 
                        NOTE: If the payment is a loyalty redemption the amount of points,
                        miles, etc. is not reflected here and instead a placeholder value
                        such as 25.00USD or 0.00USD is used.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="PaymentCardTransactionDescriptiveInfoType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Describes some of the payment transaction
                                    details so the payment may be distingushed
                                    from other transactions. This information
                                    may appear on a cardholder statement or a
                                    guest folio and it may be useful for
                                    auditing purposes.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="businessDate" type="xsd:date" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Business date of the transaction. This
                                      date could differ from the actual date
                                      (e.g., previous day if the night audit
                                      process has not yet been executed).</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="merchantId" type="cmn:StringLength1to64Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Merchant identity for the purpose of bank
                                      processing.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="merchantTransactionId" type="spt:MerchantTransactionIdType" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Unique identifier assigned by the merchant
                                      for a specific payment transaction.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="cardPresented" type="xsd:boolean" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">If true, the payment card was presented
                                      at some point during the stay.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="locationId" type="cmn:StringLength1to64Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Identifier assigned by the merchant for
                                      the business location (e.g., hotel, store)
                                      where the transaction was initiated.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="terminalId" type="cmn:StringLength1to64Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Identifier of the point of sale
                                         terminal where the transaction was
                                         initiated.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="userId" type="cmn:StringLength1to64Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Identifier of the user who initiated
                                      the transaction.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="terminalInfo" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Describes the terminal used to initiate
                                      the transaction.</xsd:documentation>
        </xsd:annotation>
        <xsd:complexType>
          <xsd:sequence>
            <xsd:element name="vendorName" type="cmn:StringLength1to32Type" minOccurs="0" maxOccurs="1"/>
            <xsd:element name="productName" type="cmn:StringLength1to32Type" minOccurs="0" maxOccurs="1"/>
            <xsd:element name="hardwareVersion" type="cmn:StringLength1to16Type" minOccurs="0" maxOccurs="1"/>
            <xsd:element name="softwareVersion" type="cmn:StringLength1to16Type" minOccurs="0" maxOccurs="1"/>
          </xsd:sequence>
        </xsd:complexType>
      </xsd:element>
      <xsd:element name="accountNumber" type="cmn:StringLength1to64Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Number assigned by the merchant to group
                                      transactions into a logical unit (e.g., a
                                      guest account number that is used to track
                                      the transactions of a specific guest across
                                      time).</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="referenceId" type="cmn:StringLength1to64Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Number assigned by the merchant to
                                      correlate with an entity in the domain
                                      of the merchant. The typical use for this
                                      is to record an identifier that is known
                                      to the customer (e.g., reservation
                                      confirmation number).</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="ledgerAccount" type="cmn:StringLength1to64Type" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Reference into the accounting system used by the
                                      merchant. The common use-case for this is to tie
                                      the payment transaction to a specific account for
                                      audit and reconciliation purposes.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="hotelTransactionInfo" minOccurs="0" maxOccurs="1">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Describes some hotel-specific payment
                                      transaction details.</xsd:documentation>
        </xsd:annotation>
        <xsd:complexType>
          <xsd:sequence>
            <xsd:element name="arrivalDate" type="xsd:date" minOccurs="0" maxOccurs="1">
              <xsd:annotation>
                <xsd:documentation xml:lang="en">Guest arrival date.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="lengthOfStay" type="xsd:nonNegativeInteger" minOccurs="0" maxOccurs="1">
              <xsd:annotation>
                <xsd:documentation xml:lang="en">Estimated number of days of guest stay.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
            <xsd:element name="guaranteedReservationNoShow" type="xsd:boolean" minOccurs="0" maxOccurs="1">
              <xsd:annotation>
                <xsd:documentation xml:lang="en">If true, the payment is an invocation
                                         of the guarantee/cancel policy of the
                                         hotel.</xsd:documentation>
              </xsd:annotation>
            </xsd:element>
          </xsd:sequence>
        </xsd:complexType>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="ProductType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Describes product that may be sold by a merchant.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="id" type="cmn:StringLength1to32Type" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="name" type="cmn:StringLength1to32Type" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="description" type="cmn:StringLength1to255Type" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="options" type="cmn:AttributeFamilyType" minOccurs="0" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="PurchasedProductsType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A collection of purchased products.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="purchasedProduct" type="spt:PurchasedProductType" minOccurs="1" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="PurchasedProductType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Describes the conditions of the purchase of a specific
                                    product.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="product" type="spt:ProductType" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="quantity" type="cmn:NumericStringLength1to3Type" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="price" type="cmn:CurrencyAmountType" minOccurs="1" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="PurchaseSearchCriteriaType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Criteria for locating and filtering purchases.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="purchaseId" type="spt:PurchaseIdType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="startDate" type="xsd:dateTime" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="endDate" type="xsd:dateTime" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="paymentTransactionId" type="spt:PaymentTransactionIdType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="merchantTransactionId" type="spt:MerchantTransactionIdType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="loyaltyAccountId" type="cmn:LoyaltyAccountIdType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="customerName" type="cmn:PersonNameType" minOccurs="0" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="PurchasesType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A collection of purchases.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="purchase" type="spt:PurchaseType" minOccurs="0" maxOccurs="unbounded"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="PurchaseType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Describes a purchase from a merchant using a payment
                                    card.</xsd:documentation>
    </xsd:annotation>
    <xsd:sequence>
      <xsd:element name="id" type="spt:PurchaseIdType" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="paymentCardTransaction" type="spt:PaymentCardTransactionType" minOccurs="1" maxOccurs="1"/>
      <xsd:element name="merchantTransaction" type="spt:MerchantTransactionType" minOccurs="0" maxOccurs="1"/>
      <xsd:element name="reversingPaymentCardTransaction" type="spt:PaymentCardTransactionType" minOccurs="0" maxOccurs="1"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="VoucherType">
    <xsd:sequence>
      <xsd:element name="effectiveDate" type="xsd:date">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The effective date of the voucher.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="expirationDate" type="xsd:date">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">The expiry date of the voucher.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="seriesCode" type="cmn:StringLength1to32Type">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Identification of a series of coupons or vouchers identified
                                      by serial number(s).</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="identifier" type="cmn:StringLength1to64Type" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Unique identifier of the electronic voucher.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="billingNumber" type="cmn:StringLength1to64Type" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Reference of the billing account which handles the payment
                                      transaction.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="supplierIdentifier" type="cmn:StringLength1to64Type" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Unique identifier of the electronic voucher, created by the
                                      supplier.</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
      <xsd:element name="valueType" type="cmn:StringLength1to32Type" minOccurs="0">
        <xsd:annotation>
          <xsd:documentation xml:lang="en">Defines the type of voucher (e.g., full credit or partial
                                      credit).</xsd:documentation>
        </xsd:annotation>
      </xsd:element>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:simpleType name="BusinessTransactionKindType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Generic business transaction type associated
                                    with a payment (e.g., ReservationGuarantee,
                                    ReservationPrepayment, FolioCashout,
                                    GiftCardPurchase, LoyaltyPointsPurchase)</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to32Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="MerchantTransactionIdType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Unique identifier assigned by the merchant
                                    for a specific payment transaction.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to64Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="MerchantTransactionKindType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Classifies a merchant transaction.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to64Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="PaymentAuthorizationIdType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Identifier for a payment authorization. This
                                    is assigned by the payment processor.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to64Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="PaymentCardIssuerIdentificationNumberType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A number used to identifiy an issuer of
                                    payment cards conforming to ISO/IEC 7812
                                    (aka IIN or BIN).</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:integer">
      <xsd:minInclusive value="0"/>
      <xsd:maxInclusive value="999999"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="PaymentCardKindType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Specifies the kind of payment card.
                                    i.e. Classic, Virtual, or Ghost.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to16Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="PaymentCardNumberPrefixType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">A number used to identifiy an issuance of cards. This
                                    may be the IIN or a longer number as in the case of
                                    a cobranded issuance.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="xsd:integer">
      <xsd:minInclusive value="0"/>
      <xsd:maxInclusive value="9999999999"/>
    </xsd:restriction>
  </xsd:simpleType>
  <xsd:simpleType name="PaymentCardProductType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Specifies the card product (e.g., Gold, Silver,
                                    Platinum, Black, Signature,
                                    ChoicePrivileges Signature VISA).</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to64Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="PaymentProcessorIdType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Identifier for a payment processor
                                    (e.g., Shift4, RealEx, Chase).</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to64Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="PaymentTransactionIdType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Identifier for a payment transaction. This
                                    is assigned by the payment processor.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to64Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="PaymentTransactionTypeCodeType">
    <xsd:annotation xml:lang="en">
      <xsd:documentation>A code used to describe a payment transaction (e.g., Charge,
                      Reserve, Refund).</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to32Type"/>
  </xsd:simpleType>
  <xsd:simpleType name="PurchaseIdType">
    <xsd:annotation>
      <xsd:documentation xml:lang="en">Identifier for a purchase.</xsd:documentation>
    </xsd:annotation>
    <xsd:restriction base="cmn:StringLength1to64Type"/>
  </xsd:simpleType>
</xsd:schema>]]></con:content>
        <con:type>http://www.w3.org/2001/XMLSchema</con:type>
      </con:part>
      <con:part>
        <con:url>http://esb.services.ext.pci.qa.chotel.com:80/HotelDistributionService/v6?SCHEMA%2FCdm_Shared_v6%2Fxsd%2Fcommon%2FCommonMessages</con:url>
        <con:content><![CDATA[<!--Document: The CommonMessages schema contains XSD message types that
          are used by multiple WSDLs. These types are defined here
          to maximize reuse and avoid redundency.

Date: 06-28-2012
Last Updated: 10-18-2012
Authors: Kirk Damron-->
<xsd:schema targetNamespace="http://www.choicehotels.com/schema/v6/common/msg" elementFormDefault="qualified" attributeFormDefault="unqualified" xml:lang="en" xmlns:cmg="http://www.choicehotels.com/schema/v6/common/msg" xmlns:cmn="http://www.choicehotels.com/schema/v6/common/cdm" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <xsd:import namespace="http://www.choicehotels.com/schema/v6/common/cdm" schemaLocation="http://esb.services.ext.pci.qa.chotel.com:80/HotelDistributionService/v6?SCHEMA%2FCdm_Shared_v6%2Fxsd%2Fcommon%2FCommonTypes"/>
  <xsd:element name="describe" type="cmg:DescribeRequestType"/>
  <xsd:element name="describeResponse" type="cmg:DescribeResponseType"/>
  <xsd:complexType name="DescribeRequestMessageType">
    <xsd:sequence>
      <xsd:element ref="cmn:requestMessageHeader"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="DescribeRequestType">
    <xsd:sequence>
      <xsd:element name="request" type="cmg:DescribeRequestMessageType"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="DescribeResponseMessageType">
    <xsd:sequence>
      <xsd:element ref="cmn:responseMessageHeader"/>
      <xsd:element ref="cmn:serviceDescriptiveInfo"/>
    </xsd:sequence>
  </xsd:complexType>
  <xsd:complexType name="DescribeResponseType">
    <xsd:sequence>
      <xsd:element name="response" type="cmg:DescribeResponseMessageType"/>
    </xsd:sequence>
  </xsd:complexType>
</xsd:schema>]]></con:content>
        <con:type>http://www.w3.org/2001/XMLSchema</con:type>
      </con:part>
    </con:definitionCache>
    <con:endpoints>
      <con:endpoint>${#Project#HDS Endpoint}</con:endpoint>
      <con:endpoint>http://esb.services.ext.pci.qa.chotel.com:80/HotelDistributionService/v6</con:endpoint>
    </con:endpoints>
    <con:environmentSpec>
      <con:entry environmentId="85ab9fa6-0169-4d73-8d01-a914c335f57b">
        <con:authProfile>Inherit From Parent</con:authProfile>
      </con:entry>
      <con:entry environmentId="7aa79c75-0aae-4877-991a-4831f886d4cc">
        <con:authProfile>Inherit From Parent</con:authProfile>
      </con:entry>
      <con:entry environmentId="4616e1b3-bc00-4528-a7d0-4d215fb2de82">
        <con:authProfile>Inherit From Parent</con:authProfile>
      </con:entry>
      <con:entry environmentId="4101a08c-af1b-41bb-9ac2-f42539ea0156">
        <con:authProfile>Inherit From Parent</con:authProfile>
      </con:entry>
    </con:environmentSpec>
    <con:operation id="dae0dd08-5950-4b4f-880d-a3940b9e4a98" isOneWay="false" action="describe" name="describe" bindingOperationName="describe" type="Request-Response" inputName="" receivesAttachments="false" sendsAttachments="false">
      <con:settings id="f0e4b811-f1ab-4160-b632-469fe7694a91">
        <con:setting id="0b0fda72-25a5-4d5a-9dbe-1fb576ea42ccfileName">describe</con:setting>
      </con:settings>
      <con:environmentSpec>
        <con:entry environmentId="85ab9fa6-0169-4d73-8d01-a914c335f57b">
          <con:authProfile>Inherit From Parent</con:authProfile>
        </con:entry>
        <con:entry environmentId="7aa79c75-0aae-4877-991a-4831f886d4cc">
          <con:authProfile>Inherit From Parent</con:authProfile>
        </con:entry>
        <con:entry environmentId="4616e1b3-bc00-4528-a7d0-4d215fb2de82">
          <con:authProfile>Inherit From Parent</con:authProfile>
        </con:entry>
        <con:entry environmentId="4101a08c-af1b-41bb-9ac2-f42539ea0156">
          <con:authProfile>Inherit From Parent</con:authProfile>
        </con:entry>
      </con:environmentSpec>
    </con:operation>
    <con:operation id="2e794386-ff1f-4b36-9b4a-06b17689b9f0" isOneWay="false" action="getHotel" name="getHotel" bindingOperationName="getHotel" type="Request-Response" inputName="" receivesAttachments="false" sendsAttachments="false" anonymous="optional">
      <con:settings id="42d3cf77-8935-4e3e-bf3b-b4ea7bb86c6c">
        <con:setting id="e883c3cc-8cc8-4ac0-a5fd-55a2e905d3d1fileName">getHotel</con:setting>
      </con:settings>
      <con:call id="76bdf63b-ae67-4c65-a8c8-d01ee8a5ad1d" name="Request 1">
        <con:settings/>
        <con:encoding>UTF-8</con:encoding>
        <con:endpoint>${#Project#HDS Endpoint}</con:endpoint>
        <con:request><![CDATA[<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:msg="http://www.choicehotels.com/schema/v6/dist/msg" xmlns:cdm="http://www.choicehotels.com/schema/v6/common/cdm">\r
   <soapenv:Header/>\r
   <soapenv:Body>\r
      <msg:getHotel>\r
         <msg:request>\r
            <cdm:requestMessageHeader version="?" sequenceNumber="?">\r
               <!--Optional:-->\r
               <cdm:echoToken>?</cdm:echoToken>\r
               <cdm:timeStamp>?</cdm:timeStamp>\r
               <!--Optional:-->\r
               <cdm:duplicate>false</cdm:duplicate>\r
               <!--Optional:-->\r
               <cdm:trackingId>?</cdm:trackingId>\r
               <!--Optional:-->\r
               <cdm:contextId>?</cdm:contextId>\r
               <!--Optional:-->\r
               <cdm:locale>\r
                  <cdm:language>?</cdm:language>\r
                  <!--Optional:-->\r
                  <cdm:country>?</cdm:country>\r
                  <!--Optional:-->\r
                  <cdm:variant>?</cdm:variant>\r
               </cdm:locale>\r
               <!--Optional:-->\r
               <cdm:organizationId>?</cdm:organizationId>\r
               <!--Optional:-->\r
               <cdm:clientIP>?</cdm:clientIP>\r
               <!--Optional:-->\r
               <cdm:clientAppName>?</cdm:clientAppName>\r
            </cdm:requestMessageHeader>\r
            <cdm:hotelId>\r
               <!--Optional:-->\r
               <cdm:id>?</cdm:id>\r
               <!--Optional:-->\r
               <cdm:uuid>?</cdm:uuid>\r
               <!--Optional:-->\r
               <cdm:altId>?</cdm:altId>\r
            </cdm:hotelId>\r
         </msg:request>\r
      </msg:getHotel>\r
   </soapenv:Body>\r
</soapenv:Envelope>]]></con:request>
        <con:credentials>
          <con:selectedAuthProfile>No Authorization</con:selectedAuthProfile>
          <con:authType>No Authorization</con:authType>
        </con:credentials>
        <con:jmsConfig JMSDeliveryMode="PERSISTENT"/>
        <con:wsaConfig mustUnderstand="NONE" version="200508" action="getHotel"/>
        <con:wsrmConfig version="1.2"/>
      </con:call>
      <con:environmentSpec>
        <con:entry environmentId="85ab9fa6-0169-4d73-8d01-a914c335f57b">
          <con:authProfile>Inherit From Parent</con:authProfile>
        </con:entry>
        <con:entry environmentId="7aa79c75-0aae-4877-991a-4831f886d4cc">
          <con:authProfile>Inherit From Parent</con:authProfile>
        </con:entry>
        <con:entry environmentId="4616e1b3-bc00-4528-a7d0-4d215fb2de82">
          <con:authProfile>Inherit From Parent</con:authProfile>
        </con:entry>
        <con:entry environmentId="4101a08c-af1b-41bb-9ac2-f42539ea0156">
          <con:authProfile>Inherit From Parent</con:authProfile>
        </con:entry>
      </con:environmentSpec>
    </con:operation>
    <con:operation id="cf69d0a9-c5a9-4e20-8fe8-92209265b4fb" isOneWay="false" action="getHotelSummary" name="getHotelSummary" bindingOperationName="getHotelSummary" type="Request-Response" inputName="" receivesAttachments="false" sendsAttachments="false">
      <con:settings id="f634e656-5278-4433-bc82-9c98c36ba99c">
        <con:setting id="caa52189-7036-44d4-b729-e3f347aa2219fileName">getHotelSummary</con:setting>
      </con:settings>
      <con:environmentSpec>
        <con:entry environmentId="85ab9fa6-0169-4d73-8d01-a914c335f57b">
          <con:authProfile>Inherit From Parent</con:authProfile>
        </con:entry>
        <con:entry environmentId="7aa79c75-0aae-4877-991a-4831f886d4cc">
          <con:authProfile>Inherit From Parent</con:authProfile>
        </con:entry>
        <con:entry environmentId="4616e1b3-bc00-4528-a7d0-4d215fb2de82">
          <con:authProfile>Inherit From Parent</con:authProfile>
        </con:entry>
        <con:entry environmentId="4101a08c-af1b-41bb-9ac2-f42539ea0156">
          <con:authProfile>Inherit From Parent</con:authProfile>
        </con:entry>
      </con:environmentSpec>
    </con:operation>
    <con:operation id="e4e5137a-781e-43dd-842e-e85c8c547dc3" isOneWay="false" action="searchHotel" name="searchHotel" bindingOperationName="searchHotel" type="Request-Response" inputName="" receivesAttachments="false" sendsAttachments="false">
      <con:settings id="1ceaa8d4-eeda-4736-ad7e-2c95d9f9ba23">
        <con:setting id="03a0b86d-1b2e-4774-8c0e-94d2dba15591fileName">searchHotel</con:setting>
      </con:settings>
      <con:environmentSpec>
        <con:entry environmentId="85ab9fa6-0169-4d73-8d01-a914c335f57b">
          <con:authProfile>Inherit From Parent</con:authProfile>
        </con:entry>
        <con:entry environmentId="7aa79c75-0aae-4877-991a-4831f886d4cc">
          <con:authProfile>Inherit From Parent</con:authProfile>
        </con:entry>
        <con:entry environmentId="4616e1b3-bc00-4528-a7d0-4d215fb2de82">
          <con:authProfile>Inherit From Parent</con:authProfile>
        </con:entry>
        <con:entry environmentId="4101a08c-af1b-41bb-9ac2-f42539ea0156">
          <con:authProfile>Inherit From Parent</con:authProfile>
        </con:entry>
      </con:environmentSpec>
    </con:operation>
  </con:interface>
  <con:testSuite id="e21f150d-99e1-4014-a936-c36b0b80e485" name="SUPER_ENRICHED_PROPERTY">
    <con:settings id="683a9da6-123d-4046-a5e2-a7d2602138ab"/>
    <con:runType>SEQUENTIAL</con:runType>
    <con:testCase id="4b45f96b-b42b-4fc7-a1cd-5ad3245c01ef" discardOkResults="false" failOnError="true" failTestCaseOnErrors="true" keepSession="false" name="postKafka-SUPER_ENRICHED_PROPERTY" searchProperties="true" timeout="0">
      <con:settings/>
      <con:testStep type="restrequest" name="POST - SUPER_ENRICHED_PROPERTY message" id="6c7b7b5e-11e4-4102-96d7-51c50efc5e00">
        <con:settings/>
        <con:config service="testDataAPI" resourcePath="/api/kafka/topic/{topicName}/message" methodName="Method 1" xsi:type="con:RestRequestStep" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
          <con:restRequest name="POST - SUPER_ENRICHED_PROPERTY message" id="c9326f50-56e3-408e-8df8-bdcaa3767896" mediaType="application/json" postQueryString="false">
            <con:settings>
              <con:setting id="com.eviware.soapui.impl.wsdl.WsdlRequest@request-headers">&lt;xml-fragment/></con:setting>
            </con:settings>
            <con:endpoint>http://testdataapi-testops-chi-qa.sharedev.cloud.chotel.com</con:endpoint>
            <con:request>{
    "brokerUrl" : "z360-kafka-qa.frandev.cloud.chotel.com:9092",
    
    "value" :"{\"messageTimestamp\":\"2025-03-06T14:23:24.93Z\",\"eventMessageType\":\"SUPER_ENRICHED_PROPERTY_CONTRACT_STATUS_CHANGE\",\"transactionUUID\":\"${#Project#trackingID}\",\"replayEventId\":83023,\"propertyUUID\":\"a033u00000tjwpCAAQ\",\"lastModifiedDatetime\":\"2025-03-06T14:14:06.000Z\",\"deleted\":false,\"propertyCode\":\"${#Project#propertyCode}\",\"externalPropertyCode\":null,\"secondaryExternalPropertyCode\":null,\"propertyEmailAddress\":\"CAK13@stayatchoice.com\",\"innboxPropertyEmail\":\"CAK13@stayatchoice.com\",\"createdDatetime\":\"2022-10-12T18:51:00.000Z\",\"name\":\"CAK13 Rohnert Park\",\"fullName\":\"Comfort Inn\",\"hotelAddress\":{\"addressLine1\":\"5040 Redwood Drive\",\"addressLine2\":null,\"addressLine3\":null,\"city\":\"Rohnert Park\",\"stateOrProvinceCode\":\"US-CA\",\"postalCode\":\"94928\",\"county\":null,\"countryCode\":\"US\"},\"mailingAddress\":{\"addressLine1\":\"5040 Redwood Drive\",\"addressLine2\":null,\"city\":\"Rohnert Park\",\"stateOrProvinceCode\":\"US-CA\",\"postalCode\":\"94928\",\"countryCode\":\"US\"},\"geoLocation\":{\"locationMethod\":\"MAP\",\"locationVerifiedFlag\":true,\"geoCodeLatitude\":38.36452,\"geoCodeLongitude\":-122.71395},\"propertyManagementCompanyUUID\":null,\"propertyManagementCompanyCode\":null,\"propertyManagementCompanyName\":null,\"controllingOfficeUUID\":null,\"controllingOfficeCode\":null,\"controllingOfficeName\":null,\"masterFranchisorUUID\":null,\"masterFranchisorCode\":null,\"masterFranchisorName\":null,\"franchisePrimaryContactAccountUUID\":null,\"franchisePrimaryContactAccountName\":null,\"buildingCapacity\":{\"floors\":3,\"guestRooms\":125,\"meetingRooms\":0},\"buildingAmenities\":{\"liquorOnPremises\":false,\"foodAndBeverage\":false,\"lounges\":null,\"outdoorPools\":1,\"indoorPools\":null,\"fitnessCenter\":true,\"laundryCenter\":false,\"corridorType\":\"Exterior\"},\"localAmenities\":{\"militaryBase\":null,\"medicalFacilities\":null,\"arenas\":null,\"universities\":null,\"otherAmenities\":null},\"hotelManagement\":{\"generalManagerName\":\"Amber Bowser\",\"additionalGeneralManagerEmail\":null,\"salesManagerName\":null},\"travelAgentCommission\":{\"percentage\":10.0,\"enabled\":true},\"locationCode\":\"C\",\"operationalLocationCode\":\"D\",\"firstOpenDate\":\"2023-06-23\",\"yearBuilt\":\"1990\",\"reportingLocationCode\":\"D\",\"fax\":\"(707) 584-8180\",\"phone\":\"(707) 584-8180\",\"STRMarketCode\":\"61300\",\"STRTractCode\":\"61302\",\"STRLocationCode\":\"SUB\",\"reservationStatus\":\"S\",\"status\":\"Pending\",\"effectiveContract\":{\"contractUUID\":\"a0GPB0000028X0r2AE\",\"legalSecName\":null,\"lastModifiedDatetime\":\"2025-03-06T14:23:20.000Z\",\"deleted\":false,\"contractId\":\"0000046061\",\"name\":\"CAK13-FR-HO-EXEC-0000046061\",\"applicationDate\":\"2025-03-06\",\"applicationType\":\"CONV\",\"averageDailyRate\":null,\"affiliationFee\":0.0,\"areaDirectorResourceUUID\":\"a313u000000SIUSAA4\",\"billableRooms\":125,\"cambriaCommissionType\":null,\"contractStatus\":\"EXEC\",\"contractSubStatus\":\"Execution Reconciliation Complete\",\"effectiveContractFlag\":false,\"effectiveDate\":\"2025-03-06\",\"salesVPResourceUUID\":\"a313u000000SIHVAA4\",\"salesVPResourceName\":\"Anthony Goldstein\",\"opening\":{\"expectedOpeningDate\":\"2025-04-30\",\"openingUUID\":\"a0fPB000000yhIDYAY\"},\"effectiveCommencementDate\":null,\"effectiveTerminationDate\":null,\"executedBillableRoomCount\":125,\"firstOutDateTermPoint\":11,\"legalSecondaryName\":null,\"licenseeRepContactUUID\":\"0033u00001wbdyiAAA\",\"licenseeRepContactName\":\"Ankit Panchal\",\"previousContractId\":null,\"possession\":false,\"salesRvpResourceUUID\":\"a31PB00000012nlYAA\",\"salesRvpResourceName\":\"Shivesh Tewari\",\"servicesRvpResourceUUID\":\"a313u000000SIIzAAO\",\"servicesRvpResourceName\":\"Byron Bean\",\"strategicDeal\":false,\"terminatedAsOtherContractIsOpen\":false,\"terminationReason\":null,\"terminationReasonDescription\":null,\"votingApprovedOnDatetime\":null,\"votingInitatedByUserUUID\":null,\"votingInitiatedDatetime\":null,\"votingProcessLevel\":null,\"votingStatus\":null,\"brand\":{\"brandUUID\":\"a0F3u000005hCTnEAM\",\"chainId\":\"U\",\"brandCode\":\"FR\",\"brandName\":\"RocketFuel\"},\"customerUUID\":\"a0IPB0000018vrl2AA\",\"customerId\":\"CAK13-03\",\"dealUUID\":\"006PB00000IcjoNYAR\",\"product\":{\"productUUID\":\"a0Q3u00000D3xy8EAB\",\"choiceClassId\":\"H\",\"productCode\":\"HO\",\"productName\":\"Hotel\"},\"propertyUUID\":\"a033u00000tjwpCAAQ\",\"propertyCode\":\"${#Project#propertyCode}\",\"dualBrandContractUUID\":null,\"dualBrandContractId\":null,\"contractTerminatedDatetime\":null,\"effectiveExecutionDate\":\"2025-03-05\",\"leveragedRepo\":false,\"dfdResourceName\":\"Shivesh Tewari\",\"dfdResourceUUID\":\"a31PB00000012nlYAA\",\"nextOutDate\":null,\"regionSalesUUID\":\"0123u000000FQxnAAG\",\"regionServicesUUID\":\"0123u000000FQxnAAG\",\"regionIOCUUID\":\"0123u000000FQxnAAG\",\"regions\":[{\"regionUUID\":\"a3IPB000000NTsX2AW\",\"regionLastModifiedDatetime\":\"2020-07-18T05:30:48.000Z\",\"deleted\":false,\"regionName\":\"12\",\"regionDescription\":\"HI,CA,NV,AZ\",\"regionType\":\"IOC\",\"regionActiveFlag\":true,\"superRegionUUID\":\"a3c3u0000006ZwbAAE\",\"superRegionLastModifiedDatetime\":\"2020-07-18T05:16:28.000Z\",\"superRegionDeleted\":false,\"superRegionName\":\"CHOC\",\"superRegionDescription\":\"QUALITY, COMFORT,CLARION,SLEEP\",\"superRegionType\":\"IOC\",\"superRegionActiveFlag\":true},{\"regionUUID\":\"a3IPB000000NTu92AG\",\"regionLastModifiedDatetime\":\"2024-12-19T02:49:11.000Z\",\"deleted\":false,\"regionName\":\"110\",\"regionDescription\":\"CI-CX-SL: CA, NV, HI\",\"regionType\":\"SALES\",\"regionActiveFlag\":true,\"superRegionUUID\":\"a3c3u0000006ZwQAAU\",\"superRegionLastModifiedDatetime\":\"2020-07-18T05:16:28.000Z\",\"superRegionDeleted\":false,\"superRegionName\":\"SEL5\",\"superRegionDescription\":\"SALES REGION - SIGNATURE WEST\",\"superRegionType\":\"SALES\",\"superRegionActiveFlag\":true},{\"regionUUID\":\"a3IPB000000NTvl2AG\",\"regionLastModifiedDatetime\":\"2020-12-16T22:42:30.000Z\",\"deleted\":false,\"regionName\":\"510\",\"regionDescription\":\"CA - BAY AREA\",\"regionType\":\"SERVICES\",\"regionActiveFlag\":true,\"superRegionUUID\":\"a3c3u0000006ZwyAAE\",\"superRegionLastModifiedDatetime\":\"2020-07-18T05:16:28.000Z\",\"superRegionDeleted\":false,\"superRegionName\":\"SVRB\",\"superRegionDescription\":\"SERVICE REGION 2\",\"superRegionType\":\"SERVICES\",\"superRegionActiveFlag\":true}]},\"propertyManagementSystemName\":\"\",\"pointOfSaleDescription\":\"\",\"rateManagementSystemName\":\"\",\"crsIntegrationName\":\"\",\"channelManagerName\":\"\",\"vanityWebsiteURL\":\"\",\"isBookingcomDirectConnected\":false,\"isExpediacomDirectConnected\":false,\"isChoiceBookingWidgetConnected\":false,\"choiceRMLevelName\":\"\",\"isChoiceRMTrial\":false,\"choiceRMStartDate\":null,\"choiceRMEndDate\":null,\"revenueManagementSystemName\":\"\",\"rmsStartDate\":null,\"rmReportingSolutionName\":\"\",\"choiceRevenueManagerResourceUUID\":\"\",\"isChoiceRevenueManagerThePropertyRevenueManager\":false}"
}</con:request>
            <con:originalUri>http://testdataapi-testops-chi-qa.sharedev.cloud.chotel.com/api/kafka/topic/z360-prop-api-sys-v2-qa/message</con:originalUri>
            <con:assertion type="Valid HTTP Status Codes" id="d5e78e7c-54c8-46ff-b095-14ea71edeacf" name="Valid HTTP Status Codes">
              <con:settings/>
              <con:configuration>
                <codes>200</codes>
              </con:configuration>
            </con:assertion>
            <con:assertion type="GroovyScriptAssertion" id="19f8d137-bd89-403c-b7e3-197da505b18e" name="Script Assertion - propertyCode">
              <con:configuration>
                <scriptText>import groovy.json.JsonSlurper

// JSON string
String jsonString = context.expand( '${POST - SUPER_ENRICHED_PROPERTY message#RawRequest#$[\'value\']}' )

// Parse JSON string
def jsonSlurper = new JsonSlurper()
def data = jsonSlurper.parseText(jsonString)
log.info data
// Get propertyCode value
def propertyCode = data.propertyCode
log.info propertyCode
// Set propertyCode value to project level
context.testCase.testSuite.project.setPropertyValue('propertyNew', propertyCode)</scriptText>
              </con:configuration>
            </con:assertion>
            <con:credentials>
              <con:selectedAuthProfile>No Authorization</con:selectedAuthProfile>
              <con:authType>No Authorization</con:authType>
            </con:credentials>
            <con:jmsConfig JMSDeliveryMode="PERSISTENT"/>
            <con:parameters>
              <con:entry key="topicName" value="z360-prop-api-sys-v2-qa"/>
            </con:parameters>
          </con:restRequest>
        </con:config>
      </con:testStep>
      <con:testStep type="request" id="282d61e4-36bd-41f1-ae77-3efa8a93984f" name="getHotel(HDS) -  Validate holet created">
        <con:settings/>
        <con:config xsi:type="con:RequestStep" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
          <con:interface>HotelDistributionSoapBinding</con:interface>
          <con:operation>getHotel</con:operation>
          <con:request name="getHotel(HDS) -  Validate holet created" id="6ed8539b-bbe7-421e-9057-81d59ddaac25">
            <con:settings>
              <con:setting id="com.eviware.soapui.impl.wsdl.WsdlRequest@request-headers">&lt;xml-fragment/></con:setting>
            </con:settings>
            <con:encoding>UTF-8</con:encoding>
            <con:endpoint>${#Project#HDSENDPOINT}</con:endpoint>
            <con:request><![CDATA[<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:msg="http://www.choicehotels.com/schema/v6/dist/msg" xmlns:cdm="http://www.choicehotels.com/schema/v6/common/cdm">
   <soapenv:Header/>
   <soapenv:Body>
      <msg:getHotel>
         <msg:request>
            <cdm:requestMessageHeader version="1" sequenceNumber="1">
               <cdm:timeStamp>${#Project#timeStamp}</cdm:timeStamp>
            </cdm:requestMessageHeader>
            <cdm:hotelId>
               
            <cdm:id>${#Project#propertyNew}</cdm:id></cdm:hotelId>
         </msg:request>
      </msg:getHotel>
      <msg1:getHotel xmlns:msg1="http://www.choicehotels.com/schema/v6/dist/msg"/>
   </soapenv:Body>
</soapenv:Envelope>]]></con:request>
            <con:assertion type="Valid HTTP Status Codes" id="45a2ec3d-c423-4209-8489-c6212faf7ffb" name="Valid HTTP Status Codes">
              <con:settings/>
              <con:configuration>
                <codes>200</codes>
              </con:configuration>
            </con:assertion>
            <con:assertion type="SOAP Fault Assertion" id="ebdd61e3-08d3-4bd4-be65-1460945d14da" name="Not SOAP Fault"/>
            <con:assertion type="XPath Match" id="69ccd0a6-ec92-4c75-b5a0-127a99fde1fa" name="Match content of [cmn:line1]">
              <con:configuration>
                <path>declare namespace dst='http://www.choicehotels.com/schema/v6/dist/cdm';
declare namespace ns6='http://www.choicehotels.com/schema/v6/dist/msg';
//ns6:getHotelResponse[1]/ns6:response[1]/dst:hotelDistribution[1]/dst:buildingCapacitySummary[1]/dst:guestRooms[1]</path>
                <content>125</content>
                <allowWildcards>false</allowWildcards>
                <ignoreNamspaceDifferences>false</ignoreNamspaceDifferences>
                <ignoreComments>false</ignoreComments>
              </con:configuration>
            </con:assertion>
            <con:assertion type="XPath Match" id="9f90e2fa-1fab-484a-a9fa-1327e11fbf54" name="XPath Match - hotel code">
              <con:configuration>
                <path>declare namespace ns2='http://www.choicehotels.com/schema/v6/dist/cdm';
declare namespace ns0='http://www.choicehotels.com/schema/v6/dist/msg';
declare namespace ns1='http://www.choicehotels.com/schema/v6/common/cdm';
//ns0:getHotelResponse[1]/ns0:response[1]/ns2:hotelDistribution[1]/ns1:hotelReference[1]/ns1:hotelId[1]/ns1:id[1]</path>
                <content>${#Project#propertyNew}</content>
                <allowWildcards>false</allowWildcards>
                <ignoreNamspaceDifferences>false</ignoreNamspaceDifferences>
                <ignoreComments>false</ignoreComments>
              </con:configuration>
            </con:assertion>
            <con:credentials>
              <con:selectedAuthProfile>No Authorization</con:selectedAuthProfile>
              <con:authType>No Authorization</con:authType>
            </con:credentials>
            <con:jmsConfig JMSDeliveryMode="PERSISTENT"/>
            <con:wsaConfig action="getHotel" mustUnderstand="NONE" version="200508"/>
            <con:wsrmConfig version="1.2"/>
            <con:environmentSpec>
              <con:entry environmentId="85ab9fa6-0169-4d73-8d01-a914c335f57b">
                <con:authProfile>Inherit From Parent</con:authProfile>
              </con:entry>
              <con:entry environmentId="7aa79c75-0aae-4877-991a-4831f886d4cc">
                <con:authProfile>Inherit From Parent</con:authProfile>
              </con:entry>
              <con:entry environmentId="4616e1b3-bc00-4528-a7d0-4d215fb2de82">
                <con:authProfile>Inherit From Parent</con:authProfile>
              </con:entry>
              <con:entry environmentId="4101a08c-af1b-41bb-9ac2-f42539ea0156">
                <con:authProfile>Inherit From Parent</con:authProfile>
              </con:entry>
              <con:entry environmentId="ca1b0d5d-339b-41fb-abf5-34b9e768e4de">
                <con:authProfile>No Authorization</con:authProfile>
              </con:entry>
              <con:entry environmentId="679a36cf-96b3-4460-9a93-f7c45a64006b">
                <con:authProfile>No Authorization</con:authProfile>
              </con:entry>
            </con:environmentSpec>
          </con:request>
        </con:config>
      </con:testStep>
      <con:properties/>
      <con:reportParameters/>
    </con:testCase>
    <con:properties/>
    <con:reportParameters/>
  </con:testSuite>
  <con:testSuite id="bb4e256a-960a-447d-9501-6303e769d852" name="PROPERTY_CHANGES_ALL">
    <con:settings id="683a9da6-123d-4046-a5e2-a7d2602138ab"/>
    <con:runType>SEQUENTIAL</con:runType>
    <con:testCase id="d717f700-1ae8-4600-81c9-86fbd3b1c101" discardOkResults="false" failOnError="true" failTestCaseOnErrors="true" keepSession="false" name="postKafka-PROPERTY_CHANGES_ALL NEW proprty" searchProperties="true" timeout="0">
      <con:settings/>
      <con:testStep type="restrequest" name="POST - PROPERTY_CHANGES_ALL message" id="1df015c0-d037-40c1-95fd-fe84a0fee1d4">
        <con:settings/>
        <con:config service="testDataAPI" resourcePath="/api/kafka/topic/{topicName}/message" methodName="Method 1" xsi:type="con:RestRequestStep" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
          <con:restRequest name="POST - PROPERTY_CHANGES_ALL message" id="c9326f50-56e3-408e-8df8-bdcaa3767896" mediaType="application/json" postQueryString="false">
            <con:settings>
              <con:setting id="com.eviware.soapui.impl.wsdl.WsdlRequest@request-headers">&lt;xml-fragment/></con:setting>
            </con:settings>
            <con:endpoint>http://testdataapi-testops-chi-qa.sharedev.cloud.chotel.com</con:endpoint>
            <con:request>{
    "brokerUrl" : "z360-kafka-qa.frandev.cloud.chotel.com:9092",
    "key" : "${#Project#propertyNew}",
    "value" :"{\"messageTimestamp\":\"2025-01-24T21:18:03.801Z\",\"eventMessageType\":\"PROPERTY_CHANGES_ALL\",\"transactionUUID\":\"${#Project#trackingID}\",\"eventReplayId\":1840444,\"propertyUUID\":\"a03PB0000091CrZYAU\",\"propertyCode\":\"${#Project#propertyNew}\",\"name\":\"WI122 Salt Lake City\",\"fullName\":\"Park Inn by Radisson, by Radisson, Salt Lake City Airport\",\"createdDatetime\":\"2024-03-15T17:07:43.000Z\",\"lastModifiedDatetime\":\"2025-01-24T21:18:00.000Z\",\"deleted\":false,\"propertyEmailAddress\":\"PD_UT320@parkinnamericas.com\",\"innboxPropertyEmail\":\"WI122@stayatchoice.com\",\"externalPropertyCode\":\"\",\"secondaryExternalPropertyCode\":\"\",\"hotelAddress\":{\"addressLine1\":\"${#Project#addr} North W Temple Street\",\"addressLine2\":\"\",\"addressLine3\":\"\",\"city\":\"Salt Lake City\",\"stateOrProvinceCode\":\"US-UT\",\"postalCode\":\"84116\",\"county\":\"\",\"countryCode\":\"US\"},\"mailingAddress\":{\"addressLine1\":\"${#Project#addr} North W Temple Street\",\"addressLine2\":\"\",\"city\":\"Salt Lake City\",\"stateOrProvinceCode\":\"US-UT\",\"postalCode\":\"${#Project#pin}\",\"countryCode\":\"US\"},\"geoLocation\":{\"locationMethod\":\"MAP\",\"locationVerifiedFlag\":false,\"geoCodeLatitude\":${#Project#latln}.772322,\"geoCodeLongitude\":-${#Project#latln}.948188},\"propertyManagementCompanyUUID\":\"001PB00000CZUabYAH\",\"propertyManagementCompanyCode\":\"GLX\",\"propertyManagementCompanyName\":\"Galaxy Hotels Group\",\"controllingOfficeUUID\":\"001PB00000CZUqjYAH\",\"controllingOfficeCode\":\"GLXCO\",\"controllingOfficeName\":\"Galaxy Hotels Group (CO)\",\"masterFranchisorUUID\":null,\"masterFranchisorCode\":null,\"masterFranchisorName\":null,\"franchisePrimaryContactAccountUUID\":null,\"franchisePrimaryContactAccountName\":null,\"buildingCapacity\":{\"floors\":1,\"guestRooms\":104,\"meetingRooms\":null},\"buildingAmenities\":{\"liquorOnPremises\":false,\"foodAndBeverage\":false,\"lounges\":null,\"outdoorPools\":null,\"indoorPools\":null,\"fitnessCenter\":false,\"laundryCenter\":false,\"corridorType\":\"Exterior\"},\"localAmenities\":{\"militaryBase\":null,\"medicalFacilities\":null,\"arenas\":null,\"universities\":null,\"otherAmenities\":null},\"hotelManagement\":{\"generalManagerName\":\"Katie Gallegos\",\"additionalGeneralManagerEmail\":\"\",\"salesManagerName\":\"\"},\"travelAgentCommission\":{\"percentage\":10.0,\"enabled\":true},\"locationCode\":\"\",\"operationalLocationCode\":\"D\",\"firstOpenDate\":\"2024-07-26\",\"yearBuilt\":\"1978\",\"reportingLocationCode\":\"D\",\"fax\":null,\"phone\":\"(385) 355-3345\",\"STRMarketCode\":\"490100\",\"STRTractCode\":\"490102\",\"STRLocationCode\":\"ARPT\",\"reservationStatus\":\"\",\"status\":\"Pending\",\"effectiveContract\":{\"contractUUID\":\"a0GPB0000013Jn72AE\",\"effectiveContractFlag\":true,\"contractId\":\"0000044744\",\"contractStatus\":\"TERM\",\"contractSubStatus\":\"\",\"effectiveTerminationDate\":\"2025-01-24\",\"legalSecName\":\"by Radisson, Salt Lake City Airport\"},\"propertyManagementSystemName\":\"\",\"pointOfSaleDescription\":\"\",\"rateManagementSystemName\":\"\",\"crsIntegrationName\":\"\",\"channelManagerName\":\"\",\"vanityWebsiteURL\":\"\",\"isBookingcomDirectConnected\":false,\"isExpediacomDirectConnected\":false,\"isChoiceBookingWidgetConnected\":false,\"choiceRMLevelName\":\"\",\"isChoiceRMTrial\":false,\"choiceRMStartDate\":null,\"choiceRMEndDate\":null,\"revenueManagementSystemName\":\"\",\"rmsStartDate\":null,\"rmReportingSolutionName\":\"\",\"choiceRevenueManagerResourceUUID\":\"\",\"isChoiceRevenueManagerThePropertyRevenueManager\":false}"
}</con:request>
            <con:originalUri>http://testdataapi-testops-chi-qa.sharedev.cloud.chotel.com/api/kafka/topic/z360-prop-api-sys-v2-qa/message</con:originalUri>
            <con:assertion type="Valid HTTP Status Codes" id="d5e78e7c-54c8-46ff-b095-14ea71edeacf" name="Valid HTTP Status Codes">
              <con:settings/>
              <con:configuration>
                <codes>200</codes>
              </con:configuration>
            </con:assertion>
            <con:assertion type="GroovyScriptAssertion" id="39bcee60-571f-42f1-89da-0d40eb39aa04" name="Script Assertion">
              <con:configuration>
                <scriptText>def rawRequest = messageExchange.getRequestContent()
def jsonSlurper = new groovy.json.JsonSlurper()
def outerJson = jsonSlurper.parseText(rawRequest)
def valueJsonStr = outerJson.value

// Unescape if necessary
if (valueJsonStr instanceof String &amp;&amp; !valueJsonStr.startsWith("{")) {
    valueJsonStr = groovy.json.StringEscapeUtils.unescapeJava(valueJsonStr)
}

def valueJson = jsonSlurper.parseText(valueJsonStr)

// Extract from nested objects
def geoCodeLongitude = valueJson.geoLocation?.geoCodeLongitude
def geoCodeLatitude  = valueJson.geoLocation?.geoCodeLatitude
def addressLine1     = valueJson.hotelAddress?.addressLine1
def postalCode       = valueJson.hotelAddress?.postalCode

// Log for debug
log.info "geoCodeLongitude: ${geoCodeLongitude}"
log.info "geoCodeLatitude: ${geoCodeLatitude}"
log.info "addressLine1: ${addressLine1}"
log.info "postalCode: ${postalCode}"

// Set as properties
def project = context.getTestCase().getTestSuite().getProject()
project.setPropertyValue("geoCodeLongitude", geoCodeLongitude?.toString() ?: "")
project.setPropertyValue("geoCodeLatitude", geoCodeLatitude?.toString() ?: "")
project.setPropertyValue("addressLine1", addressLine1 ?: "")
project.setPropertyValue("postalCode", postalCode ?: "")</scriptText>
              </con:configuration>
            </con:assertion>
            <con:credentials>
              <con:selectedAuthProfile>No Authorization</con:selectedAuthProfile>
              <con:authType>No Authorization</con:authType>
            </con:credentials>
            <con:jmsConfig JMSDeliveryMode="PERSISTENT"/>
            <con:parameters>
              <con:entry key="topicName" value="z360-prop-api-sys-v2-qa"/>
            </con:parameters>
          </con:restRequest>
        </con:config>
      </con:testStep>
      <con:testStep type="request" id="0a1f0911-4c02-40ac-bb3c-2de10f2e0e44" name="getHotel(HDS) -  Validate hotel created">
        <con:settings/>
        <con:config xsi:type="con:RequestStep" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
          <con:interface>HotelDistributionSoapBinding</con:interface>
          <con:operation>getHotel</con:operation>
          <con:request name="getHotel(HDS) -  Validate hotel created" id="6ed8539b-bbe7-421e-9057-81d59ddaac25">
            <con:settings>
              <con:setting id="com.eviware.soapui.impl.wsdl.WsdlRequest@request-headers">&lt;xml-fragment/></con:setting>
            </con:settings>
            <con:encoding>UTF-8</con:encoding>
            <con:endpoint>${#Project#HDSENDPOINT}</con:endpoint>
            <con:request><![CDATA[<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:msg="http://www.choicehotels.com/schema/v6/dist/msg" xmlns:cdm="http://www.choicehotels.com/schema/v6/common/cdm">
   <soapenv:Header/>
   <soapenv:Body>
      <msg:getHotel>
         <msg:request>
            <cdm:requestMessageHeader version="1" sequenceNumber="1">
               <cdm:timeStamp>${#Project#timeStamp}</cdm:timeStamp>
            </cdm:requestMessageHeader>
            <cdm:hotelId>
               
            <cdm:id>${#Project#propertyNew}</cdm:id></cdm:hotelId>
         </msg:request>
      </msg:getHotel>
      <msg1:getHotel xmlns:msg1="http://www.choicehotels.com/schema/v6/dist/msg"/>
   </soapenv:Body>
</soapenv:Envelope>]]></con:request>
            <con:assertion type="Valid HTTP Status Codes" id="45a2ec3d-c423-4209-8489-c6212faf7ffb" name="Valid HTTP Status Codes">
              <con:settings/>
              <con:configuration>
                <codes>200</codes>
              </con:configuration>
            </con:assertion>
            <con:assertion type="SOAP Fault Assertion" id="ebdd61e3-08d3-4bd4-be65-1460945d14da" name="Not SOAP Fault"/>
            <con:assertion type="XPath Match" id="69ccd0a6-ec92-4c75-b5a0-127a99fde1fa" name="Match content of [cmn:line1]">
              <con:configuration>
                <path>declare namespace dst='http://www.choicehotels.com/schema/v6/dist/cdm';
declare namespace ns6='http://www.choicehotels.com/schema/v6/dist/msg';
//ns6:getHotelResponse[1]/ns6:response[1]/dst:hotelDistribution[1]/dst:buildingCapacitySummary[1]/dst:guestRooms[1]</path>
                <content>104</content>
                <allowWildcards>false</allowWildcards>
                <ignoreNamspaceDifferences>false</ignoreNamspaceDifferences>
                <ignoreComments>false</ignoreComments>
              </con:configuration>
            </con:assertion>
            <con:assertion type="XPath Match" id="9f90e2fa-1fab-484a-a9fa-1327e11fbf54" name="XPath Match - hotel code">
              <con:configuration>
                <path>declare namespace ns2='http://www.choicehotels.com/schema/v6/dist/cdm';
declare namespace ns0='http://www.choicehotels.com/schema/v6/dist/msg';
declare namespace ns1='http://www.choicehotels.com/schema/v6/common/cdm';
//ns0:getHotelResponse[1]/ns0:response[1]/ns2:hotelDistribution[1]/ns1:hotelReference[1]/ns1:hotelId[1]/ns1:id[1]</path>
                <content>${#Project#propertyNew}</content>
                <allowWildcards>false</allowWildcards>
                <ignoreNamspaceDifferences>false</ignoreNamspaceDifferences>
                <ignoreComments>false</ignoreComments>
              </con:configuration>
            </con:assertion>
            <con:assertion type="GroovyScriptAssertion" id="5fe391d3-9c39-483d-902e-6adb91c7d63f" name="Script Assertion">
              <con:configuration>
                <scriptText>// Groovy script assertion for ReadyAPI test step "getHotel(HDS) - Validate hotel created"
// This script compares longitude, latitude, line1, and postalCode from the response with corresponding expected properties

// Parse the response as XML
def groovyUtils = new com.eviware.soapui.support.GroovyUtils(context)
def responseXml = new XmlSlurper().parseText(context.response)

// Extract actual values from the response
def point = responseXml.'**'.find { it.name() == 'point' }
def businessAddress = responseXml.'**'.find { it.name() == 'businessAddress' }

def actualLongitude = point.@longitude.toString()
def actualLatitude = point.@latitude.toString()
def actualLine1 = businessAddress.'line1'.text()
def actualPostalCode = businessAddress.'postalCode'.text()

// Fetch expected values from test case properties (or test step properties as appropriate)
def expectedLongitude = context.expand('${#Project#geoCodeLongitude}')
def expectedLatitude = context.expand('${#Project#geoCodeLatitude}')
def expectedLine1 = context.expand('${#Project#addressLine1}')
def expectedPostalCode = context.expand('${#Project#postalCode}')

// Assertion checks
assert actualLongitude == expectedLongitude : "Longitude does not match. Expected: ${expectedLongitude}, Actual: ${actualLongitude}"
assert actualLatitude == expectedLatitude : "Latitude does not match. Expected: ${expectedLatitude}, Actual: ${actualLatitude}"
assert actualLine1 == expectedLine1 : "Line1 does not match. Expected: ${expectedLine1}, Actual: ${actualLine1}"
assert actualPostalCode == expectedPostalCode : "PostalCode does not match. Expected: ${expectedPostalCode}, Actual: ${actualPostalCode}"</scriptText>
              </con:configuration>
            </con:assertion>
            <con:credentials>
              <con:selectedAuthProfile>No Authorization</con:selectedAuthProfile>
              <con:authType>No Authorization</con:authType>
            </con:credentials>
            <con:jmsConfig JMSDeliveryMode="PERSISTENT"/>
            <con:wsaConfig action="getHotel" mustUnderstand="NONE" version="200508"/>
            <con:wsrmConfig version="1.2"/>
            <con:environmentSpec>
              <con:entry environmentId="85ab9fa6-0169-4d73-8d01-a914c335f57b">
                <con:authProfile>Inherit From Parent</con:authProfile>
              </con:entry>
              <con:entry environmentId="7aa79c75-0aae-4877-991a-4831f886d4cc">
                <con:authProfile>Inherit From Parent</con:authProfile>
              </con:entry>
              <con:entry environmentId="4616e1b3-bc00-4528-a7d0-4d215fb2de82">
                <con:authProfile>Inherit From Parent</con:authProfile>
              </con:entry>
              <con:entry environmentId="4101a08c-af1b-41bb-9ac2-f42539ea0156">
                <con:authProfile>Inherit From Parent</con:authProfile>
              </con:entry>
              <con:entry environmentId="ca1b0d5d-339b-41fb-abf5-34b9e768e4de">
                <con:authProfile>No Authorization</con:authProfile>
              </con:entry>
              <con:entry environmentId="679a36cf-96b3-4460-9a93-f7c45a64006b">
                <con:authProfile>No Authorization</con:authProfile>
              </con:entry>
            </con:environmentSpec>
          </con:request>
        </con:config>
      </con:testStep>
      <con:properties>
        <con:property>
          <con:name>geoCodeLongitude</con:name>
          <con:value>-78.9481882</con:value>
        </con:property>
        <con:property>
          <con:name>geoCodeLatitude</con:name>
          <con:value>96.7723221</con:value>
        </con:property>
        <con:property>
          <con:name>addressLine1</con:name>
          <con:value>76 North W Temple Street</con:value>
        </con:property>
        <con:property>
          <con:name>postalCode</con:name>
          <con:value>84116</con:value>
        </con:property>
      </con:properties>
      <con:reportParameters/>
    </con:testCase>
    <con:testCase id="746c8dfd-5bd8-435c-b451-ad1349ad8c53" discardOkResults="false" failOnError="true" failTestCaseOnErrors="true" keepSession="false" name="postKafka-PROPERTY_CHANGES_ALL TERMINATED proprty" searchProperties="true" timeout="0">
      <con:settings/>
      <con:testStep type="request" id="cc5e962d-8f9e-4b74-a319-93dbc5b56dff" name="getHotel(HDS) -  search terminated prop">
        <con:settings/>
        <con:config xsi:type="con:RequestStep" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
          <con:interface>HotelDistributionSoapBinding</con:interface>
          <con:operation>getHotel</con:operation>
          <con:request name="getHotel(HDS) -  search terminated prop" id="6ed8539b-bbe7-421e-9057-81d59ddaac25">
            <con:settings>
              <con:setting id="com.eviware.soapui.impl.wsdl.WsdlRequest@request-headers">&lt;xml-fragment/></con:setting>
            </con:settings>
            <con:encoding>UTF-8</con:encoding>
            <con:endpoint>${#Project#HDSENDPOINT}</con:endpoint>
            <con:request><![CDATA[<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:msg="http://www.choicehotels.com/schema/v6/dist/msg" xmlns:cdm="http://www.choicehotels.com/schema/v6/common/cdm">
   <soapenv:Header/>
   <soapenv:Body>
      <msg:getHotel>
         <msg:request>
            <cdm:requestMessageHeader version="1" sequenceNumber="1">
               <cdm:timeStamp>${#Project#timeStamp}</cdm:timeStamp>
            </cdm:requestMessageHeader>
            <cdm:hotelId>
               
            <cdm:id>AL013</cdm:id></cdm:hotelId>
         </msg:request>
      </msg:getHotel>
      <msg1:getHotel xmlns:msg1="http://www.choicehotels.com/schema/v6/dist/msg"/>
   </soapenv:Body>
</soapenv:Envelope>]]></con:request>
            <con:assertion type="Valid HTTP Status Codes" id="45a2ec3d-c423-4209-8489-c6212faf7ffb" name="Valid HTTP Status Codes">
              <con:settings/>
              <con:configuration>
                <codes>200</codes>
              </con:configuration>
            </con:assertion>
            <con:assertion type="SOAP Fault Assertion" id="ebdd61e3-08d3-4bd4-be65-1460945d14da" name="Not SOAP Fault"/>
            <con:assertion type="XPath Match" id="69ccd0a6-ec92-4c75-b5a0-127a99fde1fa" name="Match content of [cmn:line1]">
              <con:configuration>
                <path>declare namespace dst='http://www.choicehotels.com/schema/v6/dist/cdm';
declare namespace ns6='http://www.choicehotels.com/schema/v6/dist/msg';
//ns6:getHotelResponse[1]/ns6:response[1]/dst:hotelDistribution[1]/dst:buildingCapacitySummary[1]/dst:guestRooms[1]</path>
                <content>125</content>
                <allowWildcards>false</allowWildcards>
                <ignoreNamspaceDifferences>false</ignoreNamspaceDifferences>
                <ignoreComments>false</ignoreComments>
              </con:configuration>
            </con:assertion>
            <con:assertion type="XPath Match" id="9f90e2fa-1fab-484a-a9fa-1327e11fbf54" name="XPath Match - hotel code">
              <con:configuration>
                <path>declare namespace ns2='http://www.choicehotels.com/schema/v6/dist/cdm';
declare namespace ns0='http://www.choicehotels.com/schema/v6/dist/msg';
declare namespace ns1='http://www.choicehotels.com/schema/v6/common/cdm';
//ns0:getHotelResponse[1]/ns0:response[1]/ns2:hotelDistribution[1]/ns1:hotelReference[1]/ns1:hotelId[1]/ns1:id[1]</path>
                <content>${#Project#propertyNew}</content>
                <allowWildcards>false</allowWildcards>
                <ignoreNamspaceDifferences>false</ignoreNamspaceDifferences>
                <ignoreComments>false</ignoreComments>
              </con:configuration>
            </con:assertion>
            <con:assertion type="GroovyScriptAssertion" id="f3ec929a-92b3-4d2e-a99b-9bb8d5d323cc" name="Script Assertion">
              <con:configuration>
                <scriptText>import com.eviware.soapui.support.XmlHolder

// Get the raw response content
   def responseContent = messageExchange.response.contentAsString
   def responseXml = new XmlHolder(responseContent)
   def hotelStatus = responseXml.getNodeValue("//hotelStatus")
   def hotelId = responseXml.getNodeValue("//id")
   // ReadyAPI project reference
def project = context.testCase.testSuite.project
// Validate and store the hotel ID if status is "Suspended"
if (hotelStatus == 'Suspended') {
    project.setPropertyValue('suspendedHotelId', hotelId)
    log.info "Hotel status is 'Suspended'. Stored Hotel ID: ${hotelId}"
} else {
    log.info "Hotel status is not 'Suspended'."
}</scriptText>
              </con:configuration>
            </con:assertion>
            <con:credentials>
              <con:selectedAuthProfile>No Authorization</con:selectedAuthProfile>
              <con:authType>No Authorization</con:authType>
            </con:credentials>
            <con:jmsConfig JMSDeliveryMode="PERSISTENT"/>
            <con:wsaConfig action="getHotel" mustUnderstand="NONE" version="200508"/>
            <con:wsrmConfig version="1.2"/>
            <con:environmentSpec>
              <con:entry environmentId="85ab9fa6-0169-4d73-8d01-a914c335f57b">
                <con:authProfile>Inherit From Parent</con:authProfile>
              </con:entry>
              <con:entry environmentId="7aa79c75-0aae-4877-991a-4831f886d4cc">
                <con:authProfile>Inherit From Parent</con:authProfile>
              </con:entry>
              <con:entry environmentId="4616e1b3-bc00-4528-a7d0-4d215fb2de82">
                <con:authProfile>Inherit From Parent</con:authProfile>
              </con:entry>
              <con:entry environmentId="4101a08c-af1b-41bb-9ac2-f42539ea0156">
                <con:authProfile>Inherit From Parent</con:authProfile>
              </con:entry>
              <con:entry environmentId="ca1b0d5d-339b-41fb-abf5-34b9e768e4de">
                <con:authProfile>No Authorization</con:authProfile>
              </con:entry>
              <con:entry environmentId="679a36cf-96b3-4460-9a93-f7c45a64006b">
                <con:authProfile>No Authorization</con:authProfile>
              </con:entry>
            </con:environmentSpec>
          </con:request>
        </con:config>
      </con:testStep>
      <con:testStep type="restrequest" name="POST - PROPERTY_CHANGES_ALL message" id="3be1526c-f2c5-4220-a52b-6d31b2685802">
        <con:settings/>
        <con:config service="testDataAPI" resourcePath="/api/kafka/topic/{topicName}/message" methodName="Method 1" xsi:type="con:RestRequestStep" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
          <con:restRequest name="POST - PROPERTY_CHANGES_ALL message" id="c9326f50-56e3-408e-8df8-bdcaa3767896" mediaType="application/json" postQueryString="false">
            <con:settings>
              <con:setting id="com.eviware.soapui.impl.wsdl.WsdlRequest@request-headers">&lt;xml-fragment/></con:setting>
            </con:settings>
            <con:endpoint>http://testdataapi-testops-chi-qa.sharedev.cloud.chotel.com</con:endpoint>
            <con:request>{
    "brokerUrl" : "z360-kafka-qa.frandev.cloud.chotel.com:9092",
    "key" : "${#Project#propertyNew}",
    "value" :"{\"messageTimestamp\":\"2025-01-24T21:18:03.801Z\",\"eventMessageType\":\"PROPERTY_CHANGES_ALL\",\"transactionUUID\":\"${#Project#trackingID}\",\"eventReplayId\":1840444,\"propertyUUID\":\"a03PB0000091CrZYAU\",\"propertyCode\":\"${#Project#propertyNew}\",\"name\":\"WI122 Salt Lake City\",\"fullName\":\"Park Inn by Radisson, by Radisson, Salt Lake City Airport\",\"createdDatetime\":\"2024-03-15T17:07:43.000Z\",\"lastModifiedDatetime\":\"2025-01-24T21:18:00.000Z\",\"deleted\":false,\"propertyEmailAddress\":\"PD_UT320@parkinnamericas.com\",\"innboxPropertyEmail\":\"WI122@stayatchoice.com\",\"externalPropertyCode\":\"\",\"secondaryExternalPropertyCode\":\"\",\"hotelAddress\":{\"addressLine1\":\"${#Project#addr} North W Temple Street\",\"addressLine2\":\"\",\"addressLine3\":\"\",\"city\":\"Salt Lake City\",\"stateOrProvinceCode\":\"US-UT\",\"postalCode\":\"84116\",\"county\":\"\",\"countryCode\":\"US\"},\"mailingAddress\":{\"addressLine1\":\"1990 North W Temple Street\",\"addressLine2\":\"\",\"city\":\"Salt Lake City\",\"stateOrProvinceCode\":\"US-UT\",\"postalCode\":\"84116\",\"countryCode\":\"US\"},\"geoLocation\":{\"locationMethod\":\"MAP\",\"locationVerifiedFlag\":false,\"geoCodeLatitude\":40.7723221,\"geoCodeLongitude\":-111.9481882},\"propertyManagementCompanyUUID\":\"001PB00000CZUabYAH\",\"propertyManagementCompanyCode\":\"GLX\",\"propertyManagementCompanyName\":\"Galaxy Hotels Group\",\"controllingOfficeUUID\":\"001PB00000CZUqjYAH\",\"controllingOfficeCode\":\"GLXCO\",\"controllingOfficeName\":\"Galaxy Hotels Group (CO)\",\"masterFranchisorUUID\":null,\"masterFranchisorCode\":null,\"masterFranchisorName\":null,\"franchisePrimaryContactAccountUUID\":null,\"franchisePrimaryContactAccountName\":null,\"buildingCapacity\":{\"floors\":1,\"guestRooms\":104,\"meetingRooms\":null},\"buildingAmenities\":{\"liquorOnPremises\":false,\"foodAndBeverage\":false,\"lounges\":null,\"outdoorPools\":null,\"indoorPools\":null,\"fitnessCenter\":false,\"laundryCenter\":false,\"corridorType\":\"Exterior\"},\"localAmenities\":{\"militaryBase\":null,\"medicalFacilities\":null,\"arenas\":null,\"universities\":null,\"otherAmenities\":null},\"hotelManagement\":{\"generalManagerName\":\"Katie Gallegos\",\"additionalGeneralManagerEmail\":\"\",\"salesManagerName\":\"\"},\"travelAgentCommission\":{\"percentage\":10.0,\"enabled\":true},\"locationCode\":\"\",\"operationalLocationCode\":\"D\",\"firstOpenDate\":\"2024-07-26\",\"yearBuilt\":\"1978\",\"reportingLocationCode\":\"D\",\"fax\":null,\"phone\":\"(385) 355-3345\",\"STRMarketCode\":\"490100\",\"STRTractCode\":\"490102\",\"STRLocationCode\":\"ARPT\",\"reservationStatus\":\"\",\"status\":\"Pending\",\"effectiveContract\":{\"contractUUID\":\"a0GPB0000013Jn72AE\",\"effectiveContractFlag\":true,\"contractId\":\"0000044744\",\"contractStatus\":\"TERM\",\"contractSubStatus\":\"\",\"effectiveTerminationDate\":\"2025-01-24\",\"legalSecName\":\"by Radisson, Salt Lake City Airport\"},\"propertyManagementSystemName\":\"\",\"pointOfSaleDescription\":\"\",\"rateManagementSystemName\":\"\",\"crsIntegrationName\":\"\",\"channelManagerName\":\"\",\"vanityWebsiteURL\":\"\",\"isBookingcomDirectConnected\":false,\"isExpediacomDirectConnected\":false,\"isChoiceBookingWidgetConnected\":false,\"choiceRMLevelName\":\"\",\"isChoiceRMTrial\":false,\"choiceRMStartDate\":null,\"choiceRMEndDate\":null,\"revenueManagementSystemName\":\"\",\"rmsStartDate\":null,\"rmReportingSolutionName\":\"\",\"choiceRevenueManagerResourceUUID\":\"\",\"isChoiceRevenueManagerThePropertyRevenueManager\":false}"
}</con:request>
            <con:originalUri>http://testdataapi-testops-chi-qa.sharedev.cloud.chotel.com/api/kafka/topic/z360-prop-api-sys-v2-qa/message</con:originalUri>
            <con:assertion type="Valid HTTP Status Codes" id="d5e78e7c-54c8-46ff-b095-14ea71edeacf" name="Valid HTTP Status Codes">
              <con:settings/>
              <con:configuration>
                <codes>200</codes>
              </con:configuration>
            </con:assertion>
            <con:assertion type="Response SLA Assertion" id="b601c82b-7b90-425a-951f-cffaa1d0a0a0" name="Response SLA">
              <con:configuration>
                <SLA>200</SLA>
              </con:configuration>
            </con:assertion>
            <con:assertion type="GroovyScriptAssertion" id="39bcee60-571f-42f1-89da-0d40eb39aa04" name="Script Assertion">
              <con:configuration>
                <scriptText>import groovy.json.JsonSlurper

// JSON string
String jsonString = context.expand( '${POST - SUPER_ENRICHED_PROPERTY message#RawRequest#$[\'value\']}' )

// Parse JSON string
def jsonSlurper = new JsonSlurper()
def data = jsonSlurper.parseText(jsonString)
log.info data
// Get propertyCode value
def propertyCode = data.propertyCode
log.info propertyCode
// Set propertyCode value to project level
context.testCase.testSuite.project.setPropertyValue('propertyNew', propertyCode)</scriptText>
              </con:configuration>
            </con:assertion>
            <con:credentials>
              <con:selectedAuthProfile>No Authorization</con:selectedAuthProfile>
              <con:authType>No Authorization</con:authType>
            </con:credentials>
            <con:jmsConfig JMSDeliveryMode="PERSISTENT"/>
            <con:parameters>
              <con:entry key="topicName" value="z360-prop-api-sys-v2-qa"/>
            </con:parameters>
          </con:restRequest>
        </con:config>
      </con:testStep>
      <con:testStep type="request" id="646a2643-5e3a-4892-9bde-da9dcdf34ad8" name="getHotel(HDS) -  Validate holet created">
        <con:settings/>
        <con:config xsi:type="con:RequestStep" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
          <con:interface>HotelDistributionSoapBinding</con:interface>
          <con:operation>getHotel</con:operation>
          <con:request name="getHotel(HDS) -  Validate holet created" id="6ed8539b-bbe7-421e-9057-81d59ddaac25">
            <con:settings>
              <con:setting id="com.eviware.soapui.impl.wsdl.WsdlRequest@request-headers">&lt;xml-fragment/></con:setting>
            </con:settings>
            <con:encoding>UTF-8</con:encoding>
            <con:endpoint>${#Project#HDSENDPOINT}</con:endpoint>
            <con:request><![CDATA[<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:msg="http://www.choicehotels.com/schema/v6/dist/msg" xmlns:cdm="http://www.choicehotels.com/schema/v6/common/cdm">
   <soapenv:Header/>
   <soapenv:Body>
      <msg:getHotel>
         <msg:request>
            <cdm:requestMessageHeader version="1" sequenceNumber="1">
               <cdm:timeStamp>${#Project#timeStamp}</cdm:timeStamp>
            </cdm:requestMessageHeader>
            <cdm:hotelId>
               
            <cdm:id>${#Project#propertyNew}</cdm:id></cdm:hotelId>
         </msg:request>
      </msg:getHotel>
      <msg1:getHotel xmlns:msg1="http://www.choicehotels.com/schema/v6/dist/msg"/>
   </soapenv:Body>
</soapenv:Envelope>]]></con:request>
            <con:assertion type="Valid HTTP Status Codes" id="45a2ec3d-c423-4209-8489-c6212faf7ffb" name="Valid HTTP Status Codes">
              <con:settings/>
              <con:configuration>
                <codes>200</codes>
              </con:configuration>
            </con:assertion>
            <con:assertion type="SOAP Fault Assertion" id="ebdd61e3-08d3-4bd4-be65-1460945d14da" name="Not SOAP Fault"/>
            <con:assertion type="XPath Match" id="69ccd0a6-ec92-4c75-b5a0-127a99fde1fa" name="Match content of [cmn:line1]">
              <con:configuration>
                <path>declare namespace dst='http://www.choicehotels.com/schema/v6/dist/cdm';
declare namespace ns6='http://www.choicehotels.com/schema/v6/dist/msg';
//ns6:getHotelResponse[1]/ns6:response[1]/dst:hotelDistribution[1]/dst:buildingCapacitySummary[1]/dst:guestRooms[1]</path>
                <content>125</content>
                <allowWildcards>false</allowWildcards>
                <ignoreNamspaceDifferences>false</ignoreNamspaceDifferences>
                <ignoreComments>false</ignoreComments>
              </con:configuration>
            </con:assertion>
            <con:assertion type="XPath Match" id="9f90e2fa-1fab-484a-a9fa-1327e11fbf54" name="XPath Match - hotel code">
              <con:configuration>
                <path>declare namespace ns2='http://www.choicehotels.com/schema/v6/dist/cdm';
declare namespace ns0='http://www.choicehotels.com/schema/v6/dist/msg';
declare namespace ns1='http://www.choicehotels.com/schema/v6/common/cdm';
//ns0:getHotelResponse[1]/ns0:response[1]/ns2:hotelDistribution[1]/ns1:hotelReference[1]/ns1:hotelId[1]/ns1:id[1]</path>
                <content>${#Project#propertyNew}</content>
                <allowWildcards>false</allowWildcards>
                <ignoreNamspaceDifferences>false</ignoreNamspaceDifferences>
                <ignoreComments>false</ignoreComments>
              </con:configuration>
            </con:assertion>
            <con:credentials>
              <con:selectedAuthProfile>No Authorization</con:selectedAuthProfile>
              <con:authType>No Authorization</con:authType>
            </con:credentials>
            <con:jmsConfig JMSDeliveryMode="PERSISTENT"/>
            <con:wsaConfig action="getHotel" mustUnderstand="NONE" version="200508"/>
            <con:wsrmConfig version="1.2"/>
            <con:environmentSpec>
              <con:entry environmentId="85ab9fa6-0169-4d73-8d01-a914c335f57b">
                <con:authProfile>Inherit From Parent</con:authProfile>
              </con:entry>
              <con:entry environmentId="7aa79c75-0aae-4877-991a-4831f886d4cc">
                <con:authProfile>Inherit From Parent</con:authProfile>
              </con:entry>
              <con:entry environmentId="4616e1b3-bc00-4528-a7d0-4d215fb2de82">
                <con:authProfile>Inherit From Parent</con:authProfile>
              </con:entry>
              <con:entry environmentId="4101a08c-af1b-41bb-9ac2-f42539ea0156">
                <con:authProfile>Inherit From Parent</con:authProfile>
              </con:entry>
              <con:entry environmentId="ca1b0d5d-339b-41fb-abf5-34b9e768e4de">
                <con:authProfile>No Authorization</con:authProfile>
              </con:entry>
              <con:entry environmentId="679a36cf-96b3-4460-9a93-f7c45a64006b">
                <con:authProfile>No Authorization</con:authProfile>
              </con:entry>
            </con:environmentSpec>
          </con:request>
        </con:config>
      </con:testStep>
      <con:properties/>
      <con:reportParameters/>
    </con:testCase>
    <con:testCase id="c640b248-d962-4aea-8667-86100b999d9c" discardOkResults="false" failOnError="true" failTestCaseOnErrors="true" keepSession="false" name="postKafka-PROPERTY_CHANGES_ALL INACTIVE proprty" searchProperties="true" timeout="0">
      <con:settings/>
      <con:testStep type="restrequest" name="POST - PROPERTY_CHANGES_ALL message" id="65abeb03-da74-4460-b1c8-4e4fc2216243">
        <con:settings/>
        <con:config service="testDataAPI" resourcePath="/api/kafka/topic/{topicName}/message" methodName="Method 1" xsi:type="con:RestRequestStep" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
          <con:restRequest name="POST - PROPERTY_CHANGES_ALL message" id="c9326f50-56e3-408e-8df8-bdcaa3767896" mediaType="application/json" postQueryString="false">
            <con:settings>
              <con:setting id="com.eviware.soapui.impl.wsdl.WsdlRequest@request-headers">&lt;xml-fragment/></con:setting>
            </con:settings>
            <con:endpoint>http://testdataapi-testops-chi-qa.sharedev.cloud.chotel.com</con:endpoint>
            <con:request>{
    "brokerUrl" : "z360-kafka-qa.frandev.cloud.chotel.com:9092",
    "key" : "${#Project#propertyNew}",
    "value" :"{\"messageTimestamp\":\"2025-01-24T21:18:03.801Z\",\"eventMessageType\":\"PROPERTY_CHANGES_ALL\",\"transactionUUID\":\"${#Project#trackingID}\",\"eventReplayId\":1840444,\"propertyUUID\":\"a03PB0000091CrZYAU\",\"propertyCode\":\"${#Project#propertyNew}\",\"name\":\"WI122 Salt Lake City\",\"fullName\":\"Park Inn by Radisson, by Radisson, Salt Lake City Airport\",\"createdDatetime\":\"2024-03-15T17:07:43.000Z\",\"lastModifiedDatetime\":\"2025-01-24T21:18:00.000Z\",\"deleted\":false,\"propertyEmailAddress\":\"PD_UT320@parkinnamericas.com\",\"innboxPropertyEmail\":\"WI122@stayatchoice.com\",\"externalPropertyCode\":\"\",\"secondaryExternalPropertyCode\":\"\",\"hotelAddress\":{\"addressLine1\":\"${#Project#addr} North W Temple Street\",\"addressLine2\":\"\",\"addressLine3\":\"\",\"city\":\"Salt Lake City\",\"stateOrProvinceCode\":\"US-UT\",\"postalCode\":\"84116\",\"county\":\"\",\"countryCode\":\"US\"},\"mailingAddress\":{\"addressLine1\":\"1990 North W Temple Street\",\"addressLine2\":\"\",\"city\":\"Salt Lake City\",\"stateOrProvinceCode\":\"US-UT\",\"postalCode\":\"84116\",\"countryCode\":\"US\"},\"geoLocation\":{\"locationMethod\":\"MAP\",\"locationVerifiedFlag\":false,\"geoCodeLatitude\":40.7723221,\"geoCodeLongitude\":-111.9481882},\"propertyManagementCompanyUUID\":\"001PB00000CZUabYAH\",\"propertyManagementCompanyCode\":\"GLX\",\"propertyManagementCompanyName\":\"Galaxy Hotels Group\",\"controllingOfficeUUID\":\"001PB00000CZUqjYAH\",\"controllingOfficeCode\":\"GLXCO\",\"controllingOfficeName\":\"Galaxy Hotels Group (CO)\",\"masterFranchisorUUID\":null,\"masterFranchisorCode\":null,\"masterFranchisorName\":null,\"franchisePrimaryContactAccountUUID\":null,\"franchisePrimaryContactAccountName\":null,\"buildingCapacity\":{\"floors\":1,\"guestRooms\":104,\"meetingRooms\":null},\"buildingAmenities\":{\"liquorOnPremises\":false,\"foodAndBeverage\":false,\"lounges\":null,\"outdoorPools\":null,\"indoorPools\":null,\"fitnessCenter\":false,\"laundryCenter\":false,\"corridorType\":\"Exterior\"},\"localAmenities\":{\"militaryBase\":null,\"medicalFacilities\":null,\"arenas\":null,\"universities\":null,\"otherAmenities\":null},\"hotelManagement\":{\"generalManagerName\":\"Katie Gallegos\",\"additionalGeneralManagerEmail\":\"\",\"salesManagerName\":\"\"},\"travelAgentCommission\":{\"percentage\":10.0,\"enabled\":true},\"locationCode\":\"\",\"operationalLocationCode\":\"D\",\"firstOpenDate\":\"2024-07-26\",\"yearBuilt\":\"1978\",\"reportingLocationCode\":\"D\",\"fax\":null,\"phone\":\"(385) 355-3345\",\"STRMarketCode\":\"490100\",\"STRTractCode\":\"490102\",\"STRLocationCode\":\"ARPT\",\"reservationStatus\":\"\",\"status\":\"Pending\",\"effectiveContract\":{\"contractUUID\":\"a0GPB0000013Jn72AE\",\"effectiveContractFlag\":true,\"contractId\":\"0000044744\",\"contractStatus\":\"TERM\",\"contractSubStatus\":\"\",\"effectiveTerminationDate\":\"2025-01-24\",\"legalSecName\":\"by Radisson, Salt Lake City Airport\"},\"propertyManagementSystemName\":\"\",\"pointOfSaleDescription\":\"\",\"rateManagementSystemName\":\"\",\"crsIntegrationName\":\"\",\"channelManagerName\":\"\",\"vanityWebsiteURL\":\"\",\"isBookingcomDirectConnected\":false,\"isExpediacomDirectConnected\":false,\"isChoiceBookingWidgetConnected\":false,\"choiceRMLevelName\":\"\",\"isChoiceRMTrial\":false,\"choiceRMStartDate\":null,\"choiceRMEndDate\":null,\"revenueManagementSystemName\":\"\",\"rmsStartDate\":null,\"rmReportingSolutionName\":\"\",\"choiceRevenueManagerResourceUUID\":\"\",\"isChoiceRevenueManagerThePropertyRevenueManager\":false}"
}</con:request>
            <con:originalUri>http://testdataapi-testops-chi-qa.sharedev.cloud.chotel.com/api/kafka/topic/z360-prop-api-sys-v2-qa/message</con:originalUri>
            <con:assertion type="Valid HTTP Status Codes" id="d5e78e7c-54c8-46ff-b095-14ea71edeacf" name="Valid HTTP Status Codes">
              <con:settings/>
              <con:configuration>
                <codes>200</codes>
              </con:configuration>
            </con:assertion>
            <con:assertion type="Response SLA Assertion" id="b601c82b-7b90-425a-951f-cffaa1d0a0a0" name="Response SLA">
              <con:configuration>
                <SLA>200</SLA>
              </con:configuration>
            </con:assertion>
            <con:assertion type="GroovyScriptAssertion" id="39bcee60-571f-42f1-89da-0d40eb39aa04" name="Script Assertion">
              <con:configuration>
                <scriptText>import groovy.json.JsonSlurper

// JSON string
String jsonString = context.expand( '${POST - SUPER_ENRICHED_PROPERTY message#RawRequest#$[\'value\']}' )

// Parse JSON string
def jsonSlurper = new JsonSlurper()
def data = jsonSlurper.parseText(jsonString)
log.info data
// Get propertyCode value
def propertyCode = data.propertyCode
log.info propertyCode
// Set propertyCode value to project level
context.testCase.testSuite.project.setPropertyValue('propertyNew', propertyCode)</scriptText>
              </con:configuration>
            </con:assertion>
            <con:credentials>
              <con:selectedAuthProfile>No Authorization</con:selectedAuthProfile>
              <con:authType>No Authorization</con:authType>
            </con:credentials>
            <con:jmsConfig JMSDeliveryMode="PERSISTENT"/>
            <con:parameters>
              <con:entry key="topicName" value="z360-prop-api-sys-v2-qa"/>
            </con:parameters>
          </con:restRequest>
        </con:config>
      </con:testStep>
      <con:testStep type="request" id="ab08098e-4d43-40e1-9619-2760e1c14c37" name="getHotel(HDS) -  Validate holet created">
        <con:settings/>
        <con:config xsi:type="con:RequestStep" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
          <con:interface>HotelDistributionSoapBinding</con:interface>
          <con:operation>getHotel</con:operation>
          <con:request name="getHotel(HDS) -  Validate holet created" id="6ed8539b-bbe7-421e-9057-81d59ddaac25">
            <con:settings>
              <con:setting id="com.eviware.soapui.impl.wsdl.WsdlRequest@request-headers">&lt;xml-fragment/></con:setting>
            </con:settings>
            <con:encoding>UTF-8</con:encoding>
            <con:endpoint>${#Project#HDSENDPOINT}</con:endpoint>
            <con:request><![CDATA[<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:msg="http://www.choicehotels.com/schema/v6/dist/msg" xmlns:cdm="http://www.choicehotels.com/schema/v6/common/cdm">
   <soapenv:Header/>
   <soapenv:Body>
      <msg:getHotel>
         <msg:request>
            <cdm:requestMessageHeader version="1" sequenceNumber="1">
               <cdm:timeStamp>${#Project#timeStamp}</cdm:timeStamp>
            </cdm:requestMessageHeader>
            <cdm:hotelId>
               
            <cdm:id>${#Project#propertyNew}</cdm:id></cdm:hotelId>
         </msg:request>
      </msg:getHotel>
      <msg1:getHotel xmlns:msg1="http://www.choicehotels.com/schema/v6/dist/msg"/>
   </soapenv:Body>
</soapenv:Envelope>]]></con:request>
            <con:assertion type="Valid HTTP Status Codes" id="45a2ec3d-c423-4209-8489-c6212faf7ffb" name="Valid HTTP Status Codes">
              <con:settings/>
              <con:configuration>
                <codes>200</codes>
              </con:configuration>
            </con:assertion>
            <con:assertion type="SOAP Fault Assertion" id="ebdd61e3-08d3-4bd4-be65-1460945d14da" name="Not SOAP Fault"/>
            <con:assertion type="XPath Match" id="69ccd0a6-ec92-4c75-b5a0-127a99fde1fa" name="Match content of [cmn:line1]">
              <con:configuration>
                <path>declare namespace dst='http://www.choicehotels.com/schema/v6/dist/cdm';
declare namespace ns6='http://www.choicehotels.com/schema/v6/dist/msg';
//ns6:getHotelResponse[1]/ns6:response[1]/dst:hotelDistribution[1]/dst:buildingCapacitySummary[1]/dst:guestRooms[1]</path>
                <content>125</content>
                <allowWildcards>false</allowWildcards>
                <ignoreNamspaceDifferences>false</ignoreNamspaceDifferences>
                <ignoreComments>false</ignoreComments>
              </con:configuration>
            </con:assertion>
            <con:assertion type="XPath Match" id="9f90e2fa-1fab-484a-a9fa-1327e11fbf54" name="XPath Match - hotel code">
              <con:configuration>
                <path>declare namespace ns2='http://www.choicehotels.com/schema/v6/dist/cdm';
declare namespace ns0='http://www.choicehotels.com/schema/v6/dist/msg';
declare namespace ns1='http://www.choicehotels.com/schema/v6/common/cdm';
//ns0:getHotelResponse[1]/ns0:response[1]/ns2:hotelDistribution[1]/ns1:hotelReference[1]/ns1:hotelId[1]/ns1:id[1]</path>
                <content>${#Project#propertyNew}</content>
                <allowWildcards>false</allowWildcards>
                <ignoreNamspaceDifferences>false</ignoreNamspaceDifferences>
                <ignoreComments>false</ignoreComments>
              </con:configuration>
            </con:assertion>
            <con:credentials>
              <con:selectedAuthProfile>No Authorization</con:selectedAuthProfile>
              <con:authType>No Authorization</con:authType>
            </con:credentials>
            <con:jmsConfig JMSDeliveryMode="PERSISTENT"/>
            <con:wsaConfig action="getHotel" mustUnderstand="NONE" version="200508"/>
            <con:wsrmConfig version="1.2"/>
            <con:environmentSpec>
              <con:entry environmentId="85ab9fa6-0169-4d73-8d01-a914c335f57b">
                <con:authProfile>Inherit From Parent</con:authProfile>
              </con:entry>
              <con:entry environmentId="7aa79c75-0aae-4877-991a-4831f886d4cc">
                <con:authProfile>Inherit From Parent</con:authProfile>
              </con:entry>
              <con:entry environmentId="4616e1b3-bc00-4528-a7d0-4d215fb2de82">
                <con:authProfile>Inherit From Parent</con:authProfile>
              </con:entry>
              <con:entry environmentId="4101a08c-af1b-41bb-9ac2-f42539ea0156">
                <con:authProfile>Inherit From Parent</con:authProfile>
              </con:entry>
              <con:entry environmentId="ca1b0d5d-339b-41fb-abf5-34b9e768e4de">
                <con:authProfile>No Authorization</con:authProfile>
              </con:entry>
              <con:entry environmentId="679a36cf-96b3-4460-9a93-f7c45a64006b">
                <con:authProfile>No Authorization</con:authProfile>
              </con:entry>
            </con:environmentSpec>
          </con:request>
        </con:config>
      </con:testStep>
      <con:properties/>
      <con:reportParameters/>
    </con:testCase>
    <con:testCase id="88729365-1379-461d-a065-3841f1c768c2" discardOkResults="false" failOnError="true" failTestCaseOnErrors="true" keepSession="false" name="postKafka-PROPERTY_CHANGES_ALL ACTIVE proprty" searchProperties="true" timeout="0">
      <con:settings/>
      <con:testStep type="restrequest" name="POST - PROPERTY_CHANGES_ALL message" id="33ab9d70-1f22-47b3-a0ec-1bbd6b7fdebe">
        <con:settings/>
        <con:config service="testDataAPI" resourcePath="/api/kafka/topic/{topicName}/message" methodName="Method 1" xsi:type="con:RestRequestStep" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
          <con:restRequest name="POST - PROPERTY_CHANGES_ALL message" id="c9326f50-56e3-408e-8df8-bdcaa3767896" mediaType="application/json" postQueryString="false">
            <con:settings>
              <con:setting id="com.eviware.soapui.impl.wsdl.WsdlRequest@request-headers">&lt;xml-fragment/></con:setting>
            </con:settings>
            <con:endpoint>http://testdataapi-testops-chi-qa.sharedev.cloud.chotel.com</con:endpoint>
            <con:request>{
    "brokerUrl" : "z360-kafka-qa.frandev.cloud.chotel.com:9092",
    "key" : "${#Project#propertyNew}",
    "value" :"{\"messageTimestamp\":\"2025-01-24T21:18:03.801Z\",\"eventMessageType\":\"PROPERTY_CHANGES_ALL\",\"transactionUUID\":\"${#Project#trackingID}\",\"eventReplayId\":1840444,\"propertyUUID\":\"a03PB0000091CrZYAU\",\"propertyCode\":\"${#Project#propertyNew}\",\"name\":\"WI122 Salt Lake City\",\"fullName\":\"Park Inn by Radisson, by Radisson, Salt Lake City Airport\",\"createdDatetime\":\"2024-03-15T17:07:43.000Z\",\"lastModifiedDatetime\":\"2025-01-24T21:18:00.000Z\",\"deleted\":false,\"propertyEmailAddress\":\"PD_UT320@parkinnamericas.com\",\"innboxPropertyEmail\":\"WI122@stayatchoice.com\",\"externalPropertyCode\":\"\",\"secondaryExternalPropertyCode\":\"\",\"hotelAddress\":{\"addressLine1\":\"${#Project#addr} North W Temple Street\",\"addressLine2\":\"\",\"addressLine3\":\"\",\"city\":\"Salt Lake City\",\"stateOrProvinceCode\":\"US-UT\",\"postalCode\":\"84116\",\"county\":\"\",\"countryCode\":\"US\"},\"mailingAddress\":{\"addressLine1\":\"1990 North W Temple Street\",\"addressLine2\":\"\",\"city\":\"Salt Lake City\",\"stateOrProvinceCode\":\"US-UT\",\"postalCode\":\"84116\",\"countryCode\":\"US\"},\"geoLocation\":{\"locationMethod\":\"MAP\",\"locationVerifiedFlag\":false,\"geoCodeLatitude\":40.7723221,\"geoCodeLongitude\":-111.9481882},\"propertyManagementCompanyUUID\":\"001PB00000CZUabYAH\",\"propertyManagementCompanyCode\":\"GLX\",\"propertyManagementCompanyName\":\"Galaxy Hotels Group\",\"controllingOfficeUUID\":\"001PB00000CZUqjYAH\",\"controllingOfficeCode\":\"GLXCO\",\"controllingOfficeName\":\"Galaxy Hotels Group (CO)\",\"masterFranchisorUUID\":null,\"masterFranchisorCode\":null,\"masterFranchisorName\":null,\"franchisePrimaryContactAccountUUID\":null,\"franchisePrimaryContactAccountName\":null,\"buildingCapacity\":{\"floors\":1,\"guestRooms\":104,\"meetingRooms\":null},\"buildingAmenities\":{\"liquorOnPremises\":false,\"foodAndBeverage\":false,\"lounges\":null,\"outdoorPools\":null,\"indoorPools\":null,\"fitnessCenter\":false,\"laundryCenter\":false,\"corridorType\":\"Exterior\"},\"localAmenities\":{\"militaryBase\":null,\"medicalFacilities\":null,\"arenas\":null,\"universities\":null,\"otherAmenities\":null},\"hotelManagement\":{\"generalManagerName\":\"Katie Gallegos\",\"additionalGeneralManagerEmail\":\"\",\"salesManagerName\":\"\"},\"travelAgentCommission\":{\"percentage\":10.0,\"enabled\":true},\"locationCode\":\"\",\"operationalLocationCode\":\"D\",\"firstOpenDate\":\"2024-07-26\",\"yearBuilt\":\"1978\",\"reportingLocationCode\":\"D\",\"fax\":null,\"phone\":\"(385) 355-3345\",\"STRMarketCode\":\"490100\",\"STRTractCode\":\"490102\",\"STRLocationCode\":\"ARPT\",\"reservationStatus\":\"\",\"status\":\"Pending\",\"effectiveContract\":{\"contractUUID\":\"a0GPB0000013Jn72AE\",\"effectiveContractFlag\":true,\"contractId\":\"0000044744\",\"contractStatus\":\"TERM\",\"contractSubStatus\":\"\",\"effectiveTerminationDate\":\"2025-01-24\",\"legalSecName\":\"by Radisson, Salt Lake City Airport\"},\"propertyManagementSystemName\":\"\",\"pointOfSaleDescription\":\"\",\"rateManagementSystemName\":\"\",\"crsIntegrationName\":\"\",\"channelManagerName\":\"\",\"vanityWebsiteURL\":\"\",\"isBookingcomDirectConnected\":false,\"isExpediacomDirectConnected\":false,\"isChoiceBookingWidgetConnected\":false,\"choiceRMLevelName\":\"\",\"isChoiceRMTrial\":false,\"choiceRMStartDate\":null,\"choiceRMEndDate\":null,\"revenueManagementSystemName\":\"\",\"rmsStartDate\":null,\"rmReportingSolutionName\":\"\",\"choiceRevenueManagerResourceUUID\":\"\",\"isChoiceRevenueManagerThePropertyRevenueManager\":false}"
}</con:request>
            <con:originalUri>http://testdataapi-testops-chi-qa.sharedev.cloud.chotel.com/api/kafka/topic/z360-prop-api-sys-v2-qa/message</con:originalUri>
            <con:assertion type="Valid HTTP Status Codes" id="d5e78e7c-54c8-46ff-b095-14ea71edeacf" name="Valid HTTP Status Codes">
              <con:settings/>
              <con:configuration>
                <codes>200</codes>
              </con:configuration>
            </con:assertion>
            <con:assertion type="Response SLA Assertion" id="b601c82b-7b90-425a-951f-cffaa1d0a0a0" name="Response SLA">
              <con:configuration>
                <SLA>200</SLA>
              </con:configuration>
            </con:assertion>
            <con:assertion type="GroovyScriptAssertion" id="39bcee60-571f-42f1-89da-0d40eb39aa04" name="Script Assertion">
              <con:configuration>
                <scriptText>import groovy.json.JsonSlurper

// JSON string
String jsonString = context.expand( '${POST - SUPER_ENRICHED_PROPERTY message#RawRequest#$[\'value\']}' )

// Parse JSON string
def jsonSlurper = new JsonSlurper()
def data = jsonSlurper.parseText(jsonString)
log.info data
// Get propertyCode value
def propertyCode = data.propertyCode
log.info propertyCode
// Set propertyCode value to project level
context.testCase.testSuite.project.setPropertyValue('propertyNew', propertyCode)</scriptText>
              </con:configuration>
            </con:assertion>
            <con:credentials>
              <con:selectedAuthProfile>No Authorization</con:selectedAuthProfile>
              <con:authType>No Authorization</con:authType>
            </con:credentials>
            <con:jmsConfig JMSDeliveryMode="PERSISTENT"/>
            <con:parameters>
              <con:entry key="topicName" value="z360-prop-api-sys-v2-qa"/>
            </con:parameters>
          </con:restRequest>
        </con:config>
      </con:testStep>
      <con:testStep type="restrequest" name="POST - PROPERTY_CHANGES_ALL message 2" id="8b83b184-8fa3-4214-8f88-153e425c17e2">
        <con:settings/>
        <con:config service="testDataAPI" resourcePath="/api/kafka/topic/{topicName}/message" methodName="Method 1" xsi:type="con:RestRequestStep" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
          <con:restRequest name="POST - PROPERTY_CHANGES_ALL message 2" id="c9326f50-56e3-408e-8df8-bdcaa3767896" mediaType="application/json" postQueryString="false">
            <con:settings>
              <con:setting id="com.eviware.soapui.impl.wsdl.WsdlRequest@request-headers">&lt;xml-fragment/></con:setting>
            </con:settings>
            <con:endpoint>http://testdataapi-testops-chi-qa.sharedev.cloud.chotel.com</con:endpoint>
            <con:request>{
    "brokerUrl" : "z360-kafka-qa.frandev.cloud.chotel.com:9092",
    "key" : "${#Project#propertyNew}",
    "value" :"{\"messageTimestamp\":\"2025-01-24T21:18:03.801Z\",\"eventMessageType\":\"PROPERTY_CHANGES_ALL\",\"transactionUUID\":\"${#Project#trackingID}\",\"eventReplayId\":1840444,\"propertyUUID\":\"a03PB0000091CrZYAU\",\"propertyCode\":\"${#Project#propertyNew}\",\"name\":\"WI122 Salt Lake City\",\"fullName\":\"Park Inn by Radisson, by Radisson, Salt Lake City Airport\",\"createdDatetime\":\"2024-03-15T17:07:43.000Z\",\"lastModifiedDatetime\":\"2025-01-24T21:18:00.000Z\",\"deleted\":false,\"propertyEmailAddress\":\"PD_UT320@parkinnamericas.com\",\"innboxPropertyEmail\":\"WI122@stayatchoice.com\",\"externalPropertyCode\":\"\",\"secondaryExternalPropertyCode\":\"\",\"hotelAddress\":{\"addressLine1\":\"${#Project#addr} North W Temple Street\",\"addressLine2\":\"\",\"addressLine3\":\"\",\"city\":\"Salt Lake City\",\"stateOrProvinceCode\":\"US-UT\",\"postalCode\":\"84116\",\"county\":\"\",\"countryCode\":\"US\"},\"mailingAddress\":{\"addressLine1\":\"1990 North W Temple Street\",\"addressLine2\":\"\",\"city\":\"Salt Lake City\",\"stateOrProvinceCode\":\"US-UT\",\"postalCode\":\"84116\",\"countryCode\":\"US\"},\"geoLocation\":{\"locationMethod\":\"MAP\",\"locationVerifiedFlag\":false,\"geoCodeLatitude\":40.7723221,\"geoCodeLongitude\":-111.9481882},\"propertyManagementCompanyUUID\":\"001PB00000CZUabYAH\",\"propertyManagementCompanyCode\":\"GLX\",\"propertyManagementCompanyName\":\"Galaxy Hotels Group\",\"controllingOfficeUUID\":\"001PB00000CZUqjYAH\",\"controllingOfficeCode\":\"GLXCO\",\"controllingOfficeName\":\"Galaxy Hotels Group (CO)\",\"masterFranchisorUUID\":null,\"masterFranchisorCode\":null,\"masterFranchisorName\":null,\"franchisePrimaryContactAccountUUID\":null,\"franchisePrimaryContactAccountName\":null,\"buildingCapacity\":{\"floors\":1,\"guestRooms\":104,\"meetingRooms\":null},\"buildingAmenities\":{\"liquorOnPremises\":false,\"foodAndBeverage\":false,\"lounges\":null,\"outdoorPools\":null,\"indoorPools\":null,\"fitnessCenter\":false,\"laundryCenter\":false,\"corridorType\":\"Exterior\"},\"localAmenities\":{\"militaryBase\":null,\"medicalFacilities\":null,\"arenas\":null,\"universities\":null,\"otherAmenities\":null},\"hotelManagement\":{\"generalManagerName\":\"Katie Gallegos\",\"additionalGeneralManagerEmail\":\"\",\"salesManagerName\":\"\"},\"travelAgentCommission\":{\"percentage\":10.0,\"enabled\":true},\"locationCode\":\"\",\"operationalLocationCode\":\"D\",\"firstOpenDate\":\"2024-07-26\",\"yearBuilt\":\"1978\",\"reportingLocationCode\":\"D\",\"fax\":null,\"phone\":\"(385) 355-3345\",\"STRMarketCode\":\"490100\",\"STRTractCode\":\"490102\",\"STRLocationCode\":\"ARPT\",\"reservationStatus\":\"\",\"status\":\"Pending\",\"effectiveContract\":{\"contractUUID\":\"a0GPB0000013Jn72AE\",\"effectiveContractFlag\":true,\"contractId\":\"0000044744\",\"contractStatus\":\"TERM\",\"contractSubStatus\":\"\",\"effectiveTerminationDate\":\"2025-01-24\",\"legalSecName\":\"by Radisson, Salt Lake City Airport\"},\"propertyManagementSystemName\":\"\",\"pointOfSaleDescription\":\"\",\"rateManagementSystemName\":\"\",\"crsIntegrationName\":\"\",\"channelManagerName\":\"\",\"vanityWebsiteURL\":\"\",\"isBookingcomDirectConnected\":false,\"isExpediacomDirectConnected\":false,\"isChoiceBookingWidgetConnected\":false,\"choiceRMLevelName\":\"\",\"isChoiceRMTrial\":false,\"choiceRMStartDate\":null,\"choiceRMEndDate\":null,\"revenueManagementSystemName\":\"\",\"rmsStartDate\":null,\"rmReportingSolutionName\":\"\",\"choiceRevenueManagerResourceUUID\":\"\",\"isChoiceRevenueManagerThePropertyRevenueManager\":false}"
}</con:request>
            <con:originalUri>http://testdataapi-testops-chi-qa.sharedev.cloud.chotel.com/api/kafka/topic/z360-prop-api-sys-v2-qa/message</con:originalUri>
            <con:assertion type="Valid HTTP Status Codes" id="d5e78e7c-54c8-46ff-b095-14ea71edeacf" name="Valid HTTP Status Codes">
              <con:settings/>
              <con:configuration>
                <codes>200</codes>
              </con:configuration>
            </con:assertion>
            <con:assertion type="Response SLA Assertion" id="b601c82b-7b90-425a-951f-cffaa1d0a0a0" name="Response SLA">
              <con:configuration>
                <SLA>200</SLA>
              </con:configuration>
            </con:assertion>
            <con:assertion type="GroovyScriptAssertion" id="39bcee60-571f-42f1-89da-0d40eb39aa04" name="Script Assertion">
              <con:configuration>
                <scriptText>import groovy.json.JsonSlurper

// JSON string
String jsonString = context.expand( '${POST - SUPER_ENRICHED_PROPERTY message#RawRequest#$[\'value\']}' )

// Parse JSON string
def jsonSlurper = new JsonSlurper()
def data = jsonSlurper.parseText(jsonString)
log.info data
// Get propertyCode value
def propertyCode = data.propertyCode
log.info propertyCode
// Set propertyCode value to project level
context.testCase.testSuite.project.setPropertyValue('propertyNew', propertyCode)</scriptText>
              </con:configuration>
            </con:assertion>
            <con:credentials>
              <con:selectedAuthProfile>No Authorization</con:selectedAuthProfile>
              <con:authType>No Authorization</con:authType>
            </con:credentials>
            <con:jmsConfig JMSDeliveryMode="PERSISTENT"/>
            <con:parameters>
              <con:entry key="topicName" value="z360-prop-api-sys-v2-qa"/>
            </con:parameters>
          </con:restRequest>
        </con:config>
      </con:testStep>
      <con:properties/>
      <con:reportParameters/>
    </con:testCase>
    <con:testCase id="885127fe-aaa5-4c2e-bdca-d24a02d65653" discardOkResults="false" failOnError="true" failTestCaseOnErrors="true" keepSession="false" name="postKafka-PROPERTY_CHANGES_ALL SUSPENDED proprty" searchProperties="true" timeout="0">
      <con:settings/>
      <con:testStep type="restrequest" name="POST - PROPERTY_CHANGES_ALL message" id="ff75088d-58ca-4465-90aa-385f8b8a722c">
        <con:settings/>
        <con:config service="testDataAPI" resourcePath="/api/kafka/topic/{topicName}/message" methodName="Method 1" xsi:type="con:RestRequestStep" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
          <con:restRequest name="POST - PROPERTY_CHANGES_ALL message" id="c9326f50-56e3-408e-8df8-bdcaa3767896" mediaType="application/json" postQueryString="false">
            <con:settings>
              <con:setting id="com.eviware.soapui.impl.wsdl.WsdlRequest@request-headers">&lt;xml-fragment/></con:setting>
            </con:settings>
            <con:endpoint>http://testdataapi-testops-chi-qa.sharedev.cloud.chotel.com</con:endpoint>
            <con:request>{
    "brokerUrl" : "z360-kafka-qa.frandev.cloud.chotel.com:9092",
    "key" : "${#Project#propertyNew}",
    "value" :"{\"messageTimestamp\":\"2025-01-24T21:18:03.801Z\",\"eventMessageType\":\"PROPERTY_CHANGES_ALL\",\"transactionUUID\":\"${#Project#trackingID}\",\"eventReplayId\":1840444,\"propertyUUID\":\"a03PB0000091CrZYAU\",\"propertyCode\":\"${#Project#propertyNew}\",\"name\":\"WI122 Salt Lake City\",\"fullName\":\"Park Inn by Radisson, by Radisson, Salt Lake City Airport\",\"createdDatetime\":\"2024-03-15T17:07:43.000Z\",\"lastModifiedDatetime\":\"2025-01-24T21:18:00.000Z\",\"deleted\":false,\"propertyEmailAddress\":\"PD_UT320@parkinnamericas.com\",\"innboxPropertyEmail\":\"WI122@stayatchoice.com\",\"externalPropertyCode\":\"\",\"secondaryExternalPropertyCode\":\"\",\"hotelAddress\":{\"addressLine1\":\"${#Project#addr} North W Temple Street\",\"addressLine2\":\"\",\"addressLine3\":\"\",\"city\":\"Salt Lake City\",\"stateOrProvinceCode\":\"US-UT\",\"postalCode\":\"84116\",\"county\":\"\",\"countryCode\":\"US\"},\"mailingAddress\":{\"addressLine1\":\"1990 North W Temple Street\",\"addressLine2\":\"\",\"city\":\"Salt Lake City\",\"stateOrProvinceCode\":\"US-UT\",\"postalCode\":\"84116\",\"countryCode\":\"US\"},\"geoLocation\":{\"locationMethod\":\"MAP\",\"locationVerifiedFlag\":false,\"geoCodeLatitude\":40.7723221,\"geoCodeLongitude\":-111.9481882},\"propertyManagementCompanyUUID\":\"001PB00000CZUabYAH\",\"propertyManagementCompanyCode\":\"GLX\",\"propertyManagementCompanyName\":\"Galaxy Hotels Group\",\"controllingOfficeUUID\":\"001PB00000CZUqjYAH\",\"controllingOfficeCode\":\"GLXCO\",\"controllingOfficeName\":\"Galaxy Hotels Group (CO)\",\"masterFranchisorUUID\":null,\"masterFranchisorCode\":null,\"masterFranchisorName\":null,\"franchisePrimaryContactAccountUUID\":null,\"franchisePrimaryContactAccountName\":null,\"buildingCapacity\":{\"floors\":1,\"guestRooms\":104,\"meetingRooms\":null},\"buildingAmenities\":{\"liquorOnPremises\":false,\"foodAndBeverage\":false,\"lounges\":null,\"outdoorPools\":null,\"indoorPools\":null,\"fitnessCenter\":false,\"laundryCenter\":false,\"corridorType\":\"Exterior\"},\"localAmenities\":{\"militaryBase\":null,\"medicalFacilities\":null,\"arenas\":null,\"universities\":null,\"otherAmenities\":null},\"hotelManagement\":{\"generalManagerName\":\"Katie Gallegos\",\"additionalGeneralManagerEmail\":\"\",\"salesManagerName\":\"\"},\"travelAgentCommission\":{\"percentage\":10.0,\"enabled\":true},\"locationCode\":\"\",\"operationalLocationCode\":\"D\",\"firstOpenDate\":\"2024-07-26\",\"yearBuilt\":\"1978\",\"reportingLocationCode\":\"D\",\"fax\":null,\"phone\":\"(385) 355-3345\",\"STRMarketCode\":\"490100\",\"STRTractCode\":\"490102\",\"STRLocationCode\":\"ARPT\",\"reservationStatus\":\"\",\"status\":\"Pending\",\"effectiveContract\":{\"contractUUID\":\"a0GPB0000013Jn72AE\",\"effectiveContractFlag\":true,\"contractId\":\"0000044744\",\"contractStatus\":\"TERM\",\"contractSubStatus\":\"\",\"effectiveTerminationDate\":\"2025-01-24\",\"legalSecName\":\"by Radisson, Salt Lake City Airport\"},\"propertyManagementSystemName\":\"\",\"pointOfSaleDescription\":\"\",\"rateManagementSystemName\":\"\",\"crsIntegrationName\":\"\",\"channelManagerName\":\"\",\"vanityWebsiteURL\":\"\",\"isBookingcomDirectConnected\":false,\"isExpediacomDirectConnected\":false,\"isChoiceBookingWidgetConnected\":false,\"choiceRMLevelName\":\"\",\"isChoiceRMTrial\":false,\"choiceRMStartDate\":null,\"choiceRMEndDate\":null,\"revenueManagementSystemName\":\"\",\"rmsStartDate\":null,\"rmReportingSolutionName\":\"\",\"choiceRevenueManagerResourceUUID\":\"\",\"isChoiceRevenueManagerThePropertyRevenueManager\":false}"
}</con:request>
            <con:originalUri>http://testdataapi-testops-chi-qa.sharedev.cloud.chotel.com/api/kafka/topic/z360-prop-api-sys-v2-qa/message</con:originalUri>
            <con:assertion type="Valid HTTP Status Codes" id="d5e78e7c-54c8-46ff-b095-14ea71edeacf" name="Valid HTTP Status Codes">
              <con:settings/>
              <con:configuration>
                <codes>200</codes>
              </con:configuration>
            </con:assertion>
            <con:assertion type="Response SLA Assertion" id="b601c82b-7b90-425a-951f-cffaa1d0a0a0" name="Response SLA">
              <con:configuration>
                <SLA>200</SLA>
              </con:configuration>
            </con:assertion>
            <con:assertion type="GroovyScriptAssertion" id="39bcee60-571f-42f1-89da-0d40eb39aa04" name="Script Assertion">
              <con:configuration>
                <scriptText>import groovy.json.JsonSlurper

// JSON string
String jsonString = context.expand( '${POST - SUPER_ENRICHED_PROPERTY message#RawRequest#$[\'value\']}' )

// Parse JSON string
def jsonSlurper = new JsonSlurper()
def data = jsonSlurper.parseText(jsonString)
log.info data
// Get propertyCode value
def propertyCode = data.propertyCode
log.info propertyCode
// Set propertyCode value to project level
context.testCase.testSuite.project.setPropertyValue('propertyNew', propertyCode)</scriptText>
              </con:configuration>
            </con:assertion>
            <con:credentials>
              <con:selectedAuthProfile>No Authorization</con:selectedAuthProfile>
              <con:authType>No Authorization</con:authType>
            </con:credentials>
            <con:jmsConfig JMSDeliveryMode="PERSISTENT"/>
            <con:parameters>
              <con:entry key="topicName" value="z360-prop-api-sys-v2-qa"/>
            </con:parameters>
          </con:restRequest>
        </con:config>
      </con:testStep>
      <con:testStep type="request" id="a3b4815d-40b0-4634-9cc1-a38f30aeffd3" name="getHotel(HDS) -  Validate holet created">
        <con:settings/>
        <con:config xsi:type="con:RequestStep" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
          <con:interface>HotelDistributionSoapBinding</con:interface>
          <con:operation>getHotel</con:operation>
          <con:request name="getHotel(HDS) -  Validate holet created" id="6ed8539b-bbe7-421e-9057-81d59ddaac25">
            <con:settings>
              <con:setting id="com.eviware.soapui.impl.wsdl.WsdlRequest@request-headers">&lt;xml-fragment/></con:setting>
            </con:settings>
            <con:encoding>UTF-8</con:encoding>
            <con:endpoint>${#Project#HDSENDPOINT}</con:endpoint>
            <con:request><![CDATA[<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:msg="http://www.choicehotels.com/schema/v6/dist/msg" xmlns:cdm="http://www.choicehotels.com/schema/v6/common/cdm">
   <soapenv:Header/>
   <soapenv:Body>
      <msg:getHotel>
         <msg:request>
            <cdm:requestMessageHeader version="1" sequenceNumber="1">
               <cdm:timeStamp>${#Project#timeStamp}</cdm:timeStamp>
            </cdm:requestMessageHeader>
            <cdm:hotelId>
               
            <cdm:id>${#Project#propertyNew}</cdm:id></cdm:hotelId>
         </msg:request>
      </msg:getHotel>
      <msg1:getHotel xmlns:msg1="http://www.choicehotels.com/schema/v6/dist/msg"/>
   </soapenv:Body>
</soapenv:Envelope>]]></con:request>
            <con:assertion type="Valid HTTP Status Codes" id="45a2ec3d-c423-4209-8489-c6212faf7ffb" name="Valid HTTP Status Codes">
              <con:settings/>
              <con:configuration>
                <codes>200</codes>
              </con:configuration>
            </con:assertion>
            <con:assertion type="SOAP Fault Assertion" id="ebdd61e3-08d3-4bd4-be65-1460945d14da" name="Not SOAP Fault"/>
            <con:assertion type="XPath Match" id="69ccd0a6-ec92-4c75-b5a0-127a99fde1fa" name="Match content of [cmn:line1]">
              <con:configuration>
                <path>declare namespace dst='http://www.choicehotels.com/schema/v6/dist/cdm';
declare namespace ns6='http://www.choicehotels.com/schema/v6/dist/msg';
//ns6:getHotelResponse[1]/ns6:response[1]/dst:hotelDistribution[1]/dst:buildingCapacitySummary[1]/dst:guestRooms[1]</path>
                <content>125</content>
                <allowWildcards>false</allowWildcards>
                <ignoreNamspaceDifferences>false</ignoreNamspaceDifferences>
                <ignoreComments>false</ignoreComments>
              </con:configuration>
            </con:assertion>
            <con:assertion type="XPath Match" id="9f90e2fa-1fab-484a-a9fa-1327e11fbf54" name="XPath Match - hotel code">
              <con:configuration>
                <path>declare namespace ns2='http://www.choicehotels.com/schema/v6/dist/cdm';
declare namespace ns0='http://www.choicehotels.com/schema/v6/dist/msg';
declare namespace ns1='http://www.choicehotels.com/schema/v6/common/cdm';
//ns0:getHotelResponse[1]/ns0:response[1]/ns2:hotelDistribution[1]/ns1:hotelReference[1]/ns1:hotelId[1]/ns1:id[1]</path>
                <content>${#Project#propertyNew}</content>
                <allowWildcards>false</allowWildcards>
                <ignoreNamspaceDifferences>false</ignoreNamspaceDifferences>
                <ignoreComments>false</ignoreComments>
              </con:configuration>
            </con:assertion>
            <con:credentials>
              <con:selectedAuthProfile>No Authorization</con:selectedAuthProfile>
              <con:authType>No Authorization</con:authType>
            </con:credentials>
            <con:jmsConfig JMSDeliveryMode="PERSISTENT"/>
            <con:wsaConfig action="getHotel" mustUnderstand="NONE" version="200508"/>
            <con:wsrmConfig version="1.2"/>
            <con:environmentSpec>
              <con:entry environmentId="85ab9fa6-0169-4d73-8d01-a914c335f57b">
                <con:authProfile>Inherit From Parent</con:authProfile>
              </con:entry>
              <con:entry environmentId="7aa79c75-0aae-4877-991a-4831f886d4cc">
                <con:authProfile>Inherit From Parent</con:authProfile>
              </con:entry>
              <con:entry environmentId="4616e1b3-bc00-4528-a7d0-4d215fb2de82">
                <con:authProfile>Inherit From Parent</con:authProfile>
              </con:entry>
              <con:entry environmentId="4101a08c-af1b-41bb-9ac2-f42539ea0156">
                <con:authProfile>Inherit From Parent</con:authProfile>
              </con:entry>
              <con:entry environmentId="ca1b0d5d-339b-41fb-abf5-34b9e768e4de">
                <con:authProfile>No Authorization</con:authProfile>
              </con:entry>
              <con:entry environmentId="679a36cf-96b3-4460-9a93-f7c45a64006b">
                <con:authProfile>No Authorization</con:authProfile>
              </con:entry>
            </con:environmentSpec>
          </con:request>
        </con:config>
      </con:testStep>
      <con:properties/>
      <con:reportParameters/>
    </con:testCase>
    <con:properties/>
    <con:reportParameters/>
  </con:testSuite>
  <con:testSuite id="67f09989-be1b-412e-8288-67c3fb3eccdd" name="CONTRACT_CHANGES_ALL">
    <con:settings id="683a9da6-123d-4046-a5e2-a7d2602138ab"/>
    <con:runType>SEQUENTIAL</con:runType>
    <con:testCase id="d62f8cd5-8b03-47cd-aac4-e3869a6c1eed" discardOkResults="false" failOnError="true" failTestCaseOnErrors="true" keepSession="false" name="postKafka-CONTRACT_CHANGES_ALL NEW proprty" searchProperties="true" timeout="0">
      <con:settings/>
      <con:testStep type="restrequest" name="POST - CONTRACT_CHANGES_ALL message" id="7b6f87f3-e4d1-424c-9ea1-4b2c5041dff8">
        <con:settings/>
        <con:config service="testDataAPI" resourcePath="/api/kafka/topic/{topicName}/message" methodName="Method 1" xsi:type="con:RestRequestStep" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
          <con:restRequest name="POST - CONTRACT_CHANGES_ALL message" id="c9326f50-56e3-408e-8df8-bdcaa3767896" mediaType="application/json" postQueryString="false">
            <con:settings>
              <con:setting id="com.eviware.soapui.impl.wsdl.WsdlRequest@request-headers">&lt;xml-fragment/></con:setting>
            </con:settings>
            <con:endpoint>http://testdataapi-testops-chi-qa.sharedev.cloud.chotel.com</con:endpoint>
            <con:request>{
    "brokerUrl" : "z360-kafka-qa.frandev.cloud.chotel.com:9092",
    "key" : "${#Project#propertyNew}",
    "value" :"{\"messageTimestamp\":\"2025-01-24T21:18:03.801Z\",\"eventMessageType\":\"PROPERTY_CHANGES_ALL\",\"transactionUUID\":\"${#Project#trackingID}\",\"eventReplayId\":1840444,\"propertyUUID\":\"a03PB0000091CrZYAU\",\"propertyCode\":\"${#Project#propertyNew}\",\"name\":\"WI122 Salt Lake City\",\"fullName\":\"Park Inn by Radisson, by Radisson, Salt Lake City Airport\",\"createdDatetime\":\"2024-03-15T17:07:43.000Z\",\"lastModifiedDatetime\":\"2025-01-24T21:18:00.000Z\",\"deleted\":false,\"propertyEmailAddress\":\"PD_UT320@parkinnamericas.com\",\"innboxPropertyEmail\":\"WI122@stayatchoice.com\",\"externalPropertyCode\":\"\",\"secondaryExternalPropertyCode\":\"\",\"hotelAddress\":{\"addressLine1\":\"${#Project#addr} North W Temple Street\",\"addressLine2\":\"\",\"addressLine3\":\"\",\"city\":\"Salt Lake City\",\"stateOrProvinceCode\":\"US-UT\",\"postalCode\":\"84116\",\"county\":\"\",\"countryCode\":\"US\"},\"mailingAddress\":{\"addressLine1\":\"1990 North W Temple Street\",\"addressLine2\":\"\",\"city\":\"Salt Lake City\",\"stateOrProvinceCode\":\"US-UT\",\"postalCode\":\"84116\",\"countryCode\":\"US\"},\"geoLocation\":{\"locationMethod\":\"MAP\",\"locationVerifiedFlag\":false,\"geoCodeLatitude\":40.7723221,\"geoCodeLongitude\":-111.9481882},\"propertyManagementCompanyUUID\":\"001PB00000CZUabYAH\",\"propertyManagementCompanyCode\":\"GLX\",\"propertyManagementCompanyName\":\"Galaxy Hotels Group\",\"controllingOfficeUUID\":\"001PB00000CZUqjYAH\",\"controllingOfficeCode\":\"GLXCO\",\"controllingOfficeName\":\"Galaxy Hotels Group (CO)\",\"masterFranchisorUUID\":null,\"masterFranchisorCode\":null,\"masterFranchisorName\":null,\"franchisePrimaryContactAccountUUID\":null,\"franchisePrimaryContactAccountName\":null,\"buildingCapacity\":{\"floors\":1,\"guestRooms\":104,\"meetingRooms\":null},\"buildingAmenities\":{\"liquorOnPremises\":false,\"foodAndBeverage\":false,\"lounges\":null,\"outdoorPools\":null,\"indoorPools\":null,\"fitnessCenter\":false,\"laundryCenter\":false,\"corridorType\":\"Exterior\"},\"localAmenities\":{\"militaryBase\":null,\"medicalFacilities\":null,\"arenas\":null,\"universities\":null,\"otherAmenities\":null},\"hotelManagement\":{\"generalManagerName\":\"Katie Gallegos\",\"additionalGeneralManagerEmail\":\"\",\"salesManagerName\":\"\"},\"travelAgentCommission\":{\"percentage\":10.0,\"enabled\":true},\"locationCode\":\"\",\"operationalLocationCode\":\"D\",\"firstOpenDate\":\"2024-07-26\",\"yearBuilt\":\"1978\",\"reportingLocationCode\":\"D\",\"fax\":null,\"phone\":\"(385) 355-3345\",\"STRMarketCode\":\"490100\",\"STRTractCode\":\"490102\",\"STRLocationCode\":\"ARPT\",\"reservationStatus\":\"\",\"status\":\"Pending\",\"effectiveContract\":{\"contractUUID\":\"a0GPB0000013Jn72AE\",\"effectiveContractFlag\":true,\"contractId\":\"0000044744\",\"contractStatus\":\"TERM\",\"contractSubStatus\":\"\",\"effectiveTerminationDate\":\"2025-01-24\",\"legalSecName\":\"by Radisson, Salt Lake City Airport\"},\"propertyManagementSystemName\":\"\",\"pointOfSaleDescription\":\"\",\"rateManagementSystemName\":\"\",\"crsIntegrationName\":\"\",\"channelManagerName\":\"\",\"vanityWebsiteURL\":\"\",\"isBookingcomDirectConnected\":false,\"isExpediacomDirectConnected\":false,\"isChoiceBookingWidgetConnected\":false,\"choiceRMLevelName\":\"\",\"isChoiceRMTrial\":false,\"choiceRMStartDate\":null,\"choiceRMEndDate\":null,\"revenueManagementSystemName\":\"\",\"rmsStartDate\":null,\"rmReportingSolutionName\":\"\",\"choiceRevenueManagerResourceUUID\":\"\",\"isChoiceRevenueManagerThePropertyRevenueManager\":false}"
}</con:request>
            <con:originalUri>http://testdataapi-testops-chi-qa.sharedev.cloud.chotel.com/api/kafka/topic/z360-prop-api-sys-v2-qa/message</con:originalUri>
            <con:assertion type="Valid HTTP Status Codes" id="d5e78e7c-54c8-46ff-b095-14ea71edeacf" name="Valid HTTP Status Codes">
              <con:settings/>
              <con:configuration>
                <codes>200</codes>
              </con:configuration>
            </con:assertion>
            <con:assertion type="Response SLA Assertion" id="b601c82b-7b90-425a-951f-cffaa1d0a0a0" name="Response SLA">
              <con:configuration>
                <SLA>200</SLA>
              </con:configuration>
            </con:assertion>
            <con:assertion type="GroovyScriptAssertion" id="39bcee60-571f-42f1-89da-0d40eb39aa04" name="Script Assertion">
              <con:configuration>
                <scriptText>import groovy.json.JsonSlurper

// JSON string
String jsonString = context.expand( '${POST - SUPER_ENRICHED_PROPERTY message#RawRequest#$[\'value\']}' )

// Parse JSON string
def jsonSlurper = new JsonSlurper()
def data = jsonSlurper.parseText(jsonString)
log.info data
// Get propertyCode value
def propertyCode = data.propertyCode
log.info propertyCode
// Set propertyCode value to project level
context.testCase.testSuite.project.setPropertyValue('propertyNew', propertyCode)</scriptText>
              </con:configuration>
            </con:assertion>
            <con:credentials>
              <con:selectedAuthProfile>No Authorization</con:selectedAuthProfile>
              <con:authType>No Authorization</con:authType>
            </con:credentials>
            <con:jmsConfig JMSDeliveryMode="PERSISTENT"/>
            <con:parameters>
              <con:entry key="topicName" value="z360-prop-api-sys-v2-qa"/>
            </con:parameters>
          </con:restRequest>
        </con:config>
      </con:testStep>
      <con:testStep type="request" id="e18a9e31-cace-40c0-9be5-e02651eabf30" name="getHotel(HDS) -  Validate holet created">
        <con:settings/>
        <con:config xsi:type="con:RequestStep" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
          <con:interface>HotelDistributionSoapBinding</con:interface>
          <con:operation>getHotel</con:operation>
          <con:request name="getHotel(HDS) -  Validate holet created" id="6ed8539b-bbe7-421e-9057-81d59ddaac25">
            <con:settings>
              <con:setting id="com.eviware.soapui.impl.wsdl.WsdlRequest@request-headers">&lt;xml-fragment/></con:setting>
            </con:settings>
            <con:encoding>UTF-8</con:encoding>
            <con:endpoint>${#Project#HDSENDPOINT}</con:endpoint>
            <con:request><![CDATA[<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:msg="http://www.choicehotels.com/schema/v6/dist/msg" xmlns:cdm="http://www.choicehotels.com/schema/v6/common/cdm">
   <soapenv:Header/>
   <soapenv:Body>
      <msg:getHotel>
         <msg:request>
            <cdm:requestMessageHeader version="1" sequenceNumber="1">
               <cdm:timeStamp>${#Project#timeStamp}</cdm:timeStamp>
            </cdm:requestMessageHeader>
            <cdm:hotelId>
               
            <cdm:id>${#Project#propertyNew}</cdm:id></cdm:hotelId>
         </msg:request>
      </msg:getHotel>
      <msg1:getHotel xmlns:msg1="http://www.choicehotels.com/schema/v6/dist/msg"/>
   </soapenv:Body>
</soapenv:Envelope>]]></con:request>
            <con:assertion type="Valid HTTP Status Codes" id="45a2ec3d-c423-4209-8489-c6212faf7ffb" name="Valid HTTP Status Codes">
              <con:settings/>
              <con:configuration>
                <codes>200</codes>
              </con:configuration>
            </con:assertion>
            <con:assertion type="SOAP Fault Assertion" id="ebdd61e3-08d3-4bd4-be65-1460945d14da" name="Not SOAP Fault"/>
            <con:assertion type="XPath Match" id="69ccd0a6-ec92-4c75-b5a0-127a99fde1fa" name="Match content of [cmn:line1]">
              <con:configuration>
                <path>declare namespace dst='http://www.choicehotels.com/schema/v6/dist/cdm';
declare namespace ns6='http://www.choicehotels.com/schema/v6/dist/msg';
//ns6:getHotelResponse[1]/ns6:response[1]/dst:hotelDistribution[1]/dst:buildingCapacitySummary[1]/dst:guestRooms[1]</path>
                <content>125</content>
                <allowWildcards>false</allowWildcards>
                <ignoreNamspaceDifferences>false</ignoreNamspaceDifferences>
                <ignoreComments>false</ignoreComments>
              </con:configuration>
            </con:assertion>
            <con:assertion type="XPath Match" id="9f90e2fa-1fab-484a-a9fa-1327e11fbf54" name="XPath Match - hotel code">
              <con:configuration>
                <path>declare namespace ns2='http://www.choicehotels.com/schema/v6/dist/cdm';
declare namespace ns0='http://www.choicehotels.com/schema/v6/dist/msg';
declare namespace ns1='http://www.choicehotels.com/schema/v6/common/cdm';
//ns0:getHotelResponse[1]/ns0:response[1]/ns2:hotelDistribution[1]/ns1:hotelReference[1]/ns1:hotelId[1]/ns1:id[1]</path>
                <content>${#Project#propertyNew}</content>
                <allowWildcards>false</allowWildcards>
                <ignoreNamspaceDifferences>false</ignoreNamspaceDifferences>
                <ignoreComments>false</ignoreComments>
              </con:configuration>
            </con:assertion>
            <con:credentials>
              <con:selectedAuthProfile>No Authorization</con:selectedAuthProfile>
              <con:authType>No Authorization</con:authType>
            </con:credentials>
            <con:jmsConfig JMSDeliveryMode="PERSISTENT"/>
            <con:wsaConfig action="getHotel" mustUnderstand="NONE" version="200508"/>
            <con:wsrmConfig version="1.2"/>
            <con:environmentSpec>
              <con:entry environmentId="85ab9fa6-0169-4d73-8d01-a914c335f57b">
                <con:authProfile>Inherit From Parent</con:authProfile>
              </con:entry>
              <con:entry environmentId="7aa79c75-0aae-4877-991a-4831f886d4cc">
                <con:authProfile>Inherit From Parent</con:authProfile>
              </con:entry>
              <con:entry environmentId="4616e1b3-bc00-4528-a7d0-4d215fb2de82">
                <con:authProfile>Inherit From Parent</con:authProfile>
              </con:entry>
              <con:entry environmentId="4101a08c-af1b-41bb-9ac2-f42539ea0156">
                <con:authProfile>Inherit From Parent</con:authProfile>
              </con:entry>
              <con:entry environmentId="ca1b0d5d-339b-41fb-abf5-34b9e768e4de">
                <con:authProfile>No Authorization</con:authProfile>
              </con:entry>
              <con:entry environmentId="679a36cf-96b3-4460-9a93-f7c45a64006b">
                <con:authProfile>No Authorization</con:authProfile>
              </con:entry>
            </con:environmentSpec>
          </con:request>
        </con:config>
      </con:testStep>
      <con:properties/>
      <con:reportParameters/>
    </con:testCase>
    <con:testCase id="cd0f3edd-4ef5-49ef-8324-c5ee14392910" discardOkResults="false" failOnError="true" failTestCaseOnErrors="true" keepSession="false" name="postKafka-CONTRACT_CHANGES_ALL TERMINATED proprty" searchProperties="true" timeout="0">
      <con:settings/>
      <con:properties/>
      <con:reportParameters/>
    </con:testCase>
    <con:testCase id="3cd3071e-2ec9-410d-aee7-b9aeb0a15c0d" discardOkResults="false" failOnError="true" failTestCaseOnErrors="true" keepSession="false" name="postKafka-CONTRACT_CHANGES_ALL INACTIVE proprty" searchProperties="true" timeout="0">
      <con:settings/>
      <con:properties/>
      <con:reportParameters/>
    </con:testCase>
    <con:testCase id="b7bcbdbc-cc4e-4e53-a975-9e655e32faa9" discardOkResults="false" failOnError="true" failTestCaseOnErrors="true" keepSession="false" name="postKafka-CONTRACT_CHANGES_ALL ACTIVE proprty" searchProperties="true" timeout="0">
      <con:settings/>
      <con:properties/>
      <con:reportParameters/>
    </con:testCase>
    <con:testCase id="71f207dc-fc8e-405c-8e80-45411893b5c8" discardOkResults="false" failOnError="true" failTestCaseOnErrors="true" keepSession="false" name="postKafka-CONTRACT_CHANGES_ALL SUSPENDED proprty" searchProperties="true" timeout="0">
      <con:settings/>
      <con:properties/>
      <con:reportParameters/>
    </con:testCase>
    <con:testCase id="93747342-1797-462f-bc72-9283d5fbfbd5" discardOkResults="false" failOnError="true" failTestCaseOnErrors="true" keepSession="false" name="postKafka-OPEN CONTRACT_CHANGES_ALL" searchProperties="true" timeout="0">
      <con:settings/>
      <con:properties/>
      <con:reportParameters/>
    </con:testCase>
    <con:testCase id="9f867788-2d04-4a11-8ef0-fa83d62ca581" discardOkResults="false" failOnError="true" failTestCaseOnErrors="true" keepSession="false" name="postKafka-EXEC CONTRACT_CHANGES_ALL" searchProperties="true" timeout="0">
      <con:settings/>
      <con:properties/>
      <con:reportParameters/>
    </con:testCase>
    <con:testCase id="f8f1de7d-682e-4dd8-819b-333349541a86" discardOkResults="false" failOnError="true" failTestCaseOnErrors="true" keepSession="false" name="postKafka-TERM CONTRACT_CHANGES_ALL" searchProperties="true" timeout="0">
      <con:settings/>
      <con:properties/>
      <con:reportParameters/>
    </con:testCase>
    <con:testCase id="4b2e355c-14d9-48a1-aa0c-76a9e3e71f5b" discardOkResults="false" failOnError="true" failTestCaseOnErrors="true" keepSession="false" name="postKafka-DEAD CONTRACT_CHANGES_ALL" searchProperties="true" timeout="0">
      <con:settings/>
      <con:properties/>
      <con:reportParameters/>
    </con:testCase>
    <con:properties/>
    <con:reportParameters/>
  </con:testSuite>
  <con:requirements/>
  <con:properties>
    <con:property>
      <con:name>trackingID</con:name>
      <con:value>${=java.util.UUID.randomUUID()}</con:value>
    </con:property>
    <con:property>
      <con:name>propertyCode</con:name>
      <con:value>CK${=(int)(Math.random()*1000)}</con:value>
    </con:property>
    <con:property>
      <con:name>QUlALIFIER</con:name>
      <con:value>prod</con:value>
    </con:property>
    <con:property>
      <con:name>ENVIRONMENT</con:name>
      <con:value>distprod</con:value>
    </con:property>
    <con:property>
      <con:name>HDSENDPOINT</con:name>
      <con:value>http://hds-main-api-qa.distdev.cloud.chotel.com:8080/hds?wsdl</con:value>
    </con:property>
    <con:property>
      <con:name>propCode</con:name>
      <con:value/>
    </con:property>
    <con:property>
      <con:name>propertyNew</con:name>
      <con:value>CK653</con:value>
    </con:property>
    <con:property>
      <con:name>addr</con:name>
      <con:value>${=(int)(Math.random()*1000)}</con:value>
    </con:property>
    <con:property>
      <con:name>pin</con:name>
      <con:value>${=(int)(Math.random()*1000000)}</con:value>
    </con:property>
    <con:property>
      <con:name>latln</con:name>
      <con:value>${=(int)(Math.random()*100)}</con:value>
    </con:property>
    <con:property>
      <con:name>geoCodeLongitude</con:name>
      <con:value>-52.948188</con:value>
    </con:property>
    <con:property>
      <con:name>geoCodeLatitude</con:name>
      <con:value>76.772322</con:value>
    </con:property>
    <con:property>
      <con:name>addressLine1</con:name>
      <con:value>968 North W Temple Street</con:value>
    </con:property>
    <con:property>
      <con:name>postalCode</con:name>
      <con:value>84116</con:value>
    </con:property>
  </con:properties>
  <con:wssContainer/>
  <con:databaseConnectionContainer/>
  <con:jmsConnectionContainer/>
  <con:oAuth2ProfileContainer/>
  <con:oAuth1ProfileContainer/>
  <con:reporting>
    <con:xmlTemplates/>
    <con:parameters/>
  </con:reporting>
  <con:eventHandlers type="RequestFilter.filterRequest" name="RequestFilter.filterRequest">
    <con:script>// Sample event script to add custom HTTP header to all outgoing REST, SOAP and HTTP(S) calls
// This code is often used for adding custom authentication to ReadyAPI functional tests

// If hardcoding the token, uncomment and change line 5
// token = '4567'

// If your token is parameterized in Project level custom property, uncomment line 8
// token = request.parent.testCase.testSuite.project.getProperty('auth_token').getValue()

// To modify all outgoing calls, remove comments from lines 11 to 16
// headers = request.requestHeaders
// if (headers.containsKey('auth_token2') == false) {
//   headers.put('auth_token2', token)
//   request.requestHeaders = headers
// }</con:script>
  </con:eventHandlers>
  <con:eventHandlers type="TestRunListener.afterStep" name="TestRunListener.afterStep">
    <con:script>// Save all test step results into files
// Change the directory path in line 5 to a location where you want to store details
// then uncomment lines 5 to 10

// filePath = 'C:\\tempOutputDirectory\\'
// fos = new java.io.FileOutputStream(filePath + testStepResult.testStep.label + '.txt', true)
// pw = new java.io.PrintWriter(fos)
// testStepResult.writeTo(pw)
// pw.close()
// fos.close()</con:script>
  </con:eventHandlers>
  <con:authRepository/>
  <con:tags/>
</con:soapui-project>
