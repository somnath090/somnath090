Groovy script to assertion to get the values of longitude,latitude,line1 and postalCode for ReadyAPI test step "getHotel(HDS) -  Validate hotel created" and get the values of geoCodeLongitude,geoCodeLatitude addressLine1, and postalCode for ReadyAPI test step "postKafka-PROPERTY_CHANGES_ALL NEW proprty" matches correctly

ReadyAPI test step "postKafka-PROPERTY_CHANGES_ALL NEW proprty"
raw request : POST http://testdataapi-testops-chi-qa.sharedev.cloud.chotel.com/api/kafka/topic/z360-prop-api-sys-v2-qa/message HTTP/1.1
Accept-Encoding: gzip,deflate,br
Content-Type: application/json
Content-Length: 3637
Host: testdataapi-testops-chi-qa.sharedev.cloud.chotel.com
Connection: Keep-Alive
User-Agent: Apache-HttpClient/4.5.14 (Java/17.0.10)

{
    "brokerUrl" : "z360-kafka-qa.frandev.cloud.chotel.com:9092",
    "key" : "CK653",
    "value" :"{\"messageTimestamp\":\"2025-01-24T21:18:03.801Z\",\"eventMessageType\":\"PROPERTY_CHANGES_ALL\",\"transactionUUID\":\"4debcfaa-4f8f-497e-921c-835159e5b609\",\"eventReplayId\":1840444,\"propertyUUID\":\"a03PB0000091CrZYAU\",\"propertyCode\":\"CK653\",\"name\":\"WI122 Salt Lake City\",\"fullName\":\"Park Inn by Radisson, by Radisson, Salt Lake City Airport\",\"createdDatetime\":\"2024-03-15T17:07:43.000Z\",\"lastModifiedDatetime\":\"2025-01-24T21:18:00.000Z\",\"deleted\":false,\"propertyEmailAddress\":\"PD_UT320@parkinnamericas.com\",\"innboxPropertyEmail\":\"WI122@stayatchoice.com\",\"externalPropertyCode\":\"\",\"secondaryExternalPropertyCode\":\"\",\"hotelAddress\":{\"addressLine1\":\"564 North W Temple Street\",\"addressLine2\":\"\",\"addressLine3\":\"\",\"city\":\"Salt Lake City\",\"stateOrProvinceCode\":\"US-UT\",\"postalCode\":\"84116\",\"county\":\"\",\"countryCode\":\"US\"},\"mailingAddress\":{\"addressLine1\":\"295 North W Temple Street\",\"addressLine2\":\"\",\"city\":\"Salt Lake City\",\"stateOrProvinceCode\":\"US-UT\",\"postalCode\":\"684257\",\"countryCode\":\"US\"},\"geoLocation\":{\"locationMethod\":\"MAP\",\"locationVerifiedFlag\":false,\"geoCodeLatitude\":48.7723221,\"geoCodeLongitude\":-81.9481882},\"propertyManagementCompanyUUID\":\"001PB00000CZUabYAH\",\"propertyManagementCompanyCode\":\"GLX\",\"propertyManagementCompanyName\":\"Galaxy Hotels Group\",\"controllingOfficeUUID\":\"001PB00000CZUqjYAH\",\"controllingOfficeCode\":\"GLXCO\",\"controllingOfficeName\":\"Galaxy Hotels Group (CO)\",\"masterFranchisorUUID\":null,\"masterFranchisorCode\":null,\"masterFranchisorName\":null,\"franchisePrimaryContactAccountUUID\":null,\"franchisePrimaryContactAccountName\":null,\"buildingCapacity\":{\"floors\":1,\"guestRooms\":104,\"meetingRooms\":null},\"buildingAmenities\":{\"liquorOnPremises\":false,\"foodAndBeverage\":false,\"lounges\":null,\"outdoorPools\":null,\"indoorPools\":null,\"fitnessCenter\":false,\"laundryCenter\":false,\"corridorType\":\"Exterior\"},\"localAmenities\":{\"militaryBase\":null,\"medicalFacilities\":null,\"arenas\":null,\"universities\":null,\"otherAmenities\":null},\"hotelManagement\":{\"generalManagerName\":\"Katie Gallegos\",\"additionalGeneralManagerEmail\":\"\",\"salesManagerName\":\"\"},\"travelAgentCommission\":{\"percentage\":10.0,\"enabled\":true},\"locationCode\":\"\",\"operationalLocationCode\":\"D\",\"firstOpenDate\":\"2024-07-26\",\"yearBuilt\":\"1978\",\"reportingLocationCode\":\"D\",\"fax\":null,\"phone\":\"(385) 355-3345\",\"STRMarketCode\":\"490100\",\"STRTractCode\":\"490102\",\"STRLocationCode\":\"ARPT\",\"reservationStatus\":\"\",\"status\":\"Pending\",\"effectiveContract\":{\"contractUUID\":\"a0GPB0000013Jn72AE\",\"effectiveContractFlag\":true,\"contractId\":\"0000044744\",\"contractStatus\":\"TERM\",\"contractSubStatus\":\"\",\"effectiveTerminationDate\":\"2025-01-24\",\"legalSecName\":\"by Radisson, Salt Lake City Airport\"},\"propertyManagementSystemName\":\"\",\"pointOfSaleDescription\":\"\",\"rateManagementSystemName\":\"\",\"crsIntegrationName\":\"\",\"channelManagerName\":\"\",\"vanityWebsiteURL\":\"\",\"isBookingcomDirectConnected\":false,\"isExpediacomDirectConnected\":false,\"isChoiceBookingWidgetConnected\":false,\"choiceRMLevelName\":\"\",\"isChoiceRMTrial\":false,\"choiceRMStartDate\":null,\"choiceRMEndDate\":null,\"revenueManagementSystemName\":\"\",\"rmsStartDate\":null,\"rmReportingSolutionName\":\"\",\"choiceRevenueManagerResourceUUID\":\"\",\"isChoiceRevenueManagerThePropertyRevenueManager\":false}"
}
ReadyAPI test step "getHotel(HDS) -  Validate hotel created"
response : <S:Envelope xmlns:S="http://schemas.xmlsoap.org/soap/envelope/">
   <S:Body>
      <ns0:getHotelResponse xmlns:ns0="http://www.choicehotels.com/schema/v6/dist/msg" xmlns:ns1="http://www.choicehotels.com/schema/v6/common/cdm" xmlns:ns2="http://www.choicehotels.com/schema/v6/dist/cdm" xmlns:ns13="http://www.choicehotels.com/schema/v6/dist/evt" xmlns:ns3="http://www.choicehotels.com/schema/v6/support/cdm" xmlns:ns4="http://www.choicehotels.com/schema/v6/guest/cdm">
         <ns0:response>
            <ns1:responseMessageHeader version="1" sequenceNumber="1">
               <ns1:timeStamp>2025-06-04T09:26:26Z</ns1:timeStamp>
            </ns1:responseMessageHeader>
            <ns2:hotelDistribution coOpParticipant="false" language="en" country="US">
               <ns1:hotelReference>
                  <ns1:hotelId>
                     <ns1:id>CK653</ns1:id>
                     <ns1:altId>ACKLUzWNEfC6mQowJguSGw</ns1:altId>
                  </ns1:hotelId>
                  <ns1:hotelName>
                     <ns1:name>Park Inn by Radisson, by Radisson, Salt Lake City Airport</ns1:name>
                  </ns1:hotelName>
                  <ns1:brandReference>
                     <ns1:brandCode>
                        <ns1:id>FR</ns1:id>
                     </ns1:brandCode>
                     <ns1:name>RocketFuel</ns1:name>
                  </ns1:brandReference>
                  <ns1:productReference>
                     <ns1:productCode>
                        <ns1:id>HO</ns1:id>
                     </ns1:productCode>
                     <ns1:name>Hotel</ns1:name>
                  </ns1:productReference>
               </ns1:hotelReference>
               <ns2:alternateHotelNames>
                  <ns2:legalNameExtension>by Radisson, Salt Lake City Airport</ns2:legalNameExtension>
               </ns2:alternateHotelNames>
               <ns2:businessAddress>
                  <ns1:line1>564 North W Temple Street</ns1:line1>
                  <ns1:city>Salt Lake City</ns1:city>
                  <ns1:postalCode>84116</ns1:postalCode>
                  <ns1:stateOrProvince>UT</ns1:stateOrProvince>
                  <ns1:country>US</ns1:country>
               </ns2:businessAddress>
               <ns2:primaryPhoneNumber kind="PRIMARY">
                  <ns1:countryAccessCode>1</ns1:countryAccessCode>
                  <ns1:areaCode>385</ns1:areaCode>
                  <ns1:phoneNumber>355-3345</ns1:phoneNumber>
               </ns2:primaryPhoneNumber>
               <ns2:effectiveDate>2025-05-20</ns2:effectiveDate>
               <ns2:hotelEffectiveStatus>
                  <ns2:hotelStatus>New</ns2:hotelStatus>
                  <ns2:effectiveDate>2025-05-20</ns2:effectiveDate>
               </ns2:hotelEffectiveStatus>
               <ns2:geoLocation>
                  <ns2:point latitude="48.772322" longitude="-81.948188">
                     <ns2:determinationMethod>Map Look-up</ns2:determinationMethod>
                     <ns2:locationVerified>false</ns2:locationVerified>
                  </ns2:point>
               </ns2:geoLocation>
               <ns2:currencyCode>USD</ns2:currencyCode>
               <ns2:buildingCapacitySummary>
                  <ns2:guestRooms>104</ns2:guestRooms>
                  <ns2:meetingRooms>0</ns2:meetingRooms>
                  <ns2:floors>1</ns2:floors>
               </ns2:buildingCapacitySummary>
               <ns2:hotelAmenities>
                  <ns2:amenity code="NPET" description="No Pets Allowed" charge="false">
                     <ns2:operatingSchedule/>
                     <ns2:distanceFromHotel value="0.0" text="Onsite"/>
                  </ns2:amenity>
               </ns2:hotelAmenities>
               <ns2:timeZoneInfo>
                  <ns2:GMTOffset>-420</ns2:GMTOffset>
                  <ns2:timezoneLocation>America/Phoenix</ns2:timezoneLocation>
                  <ns2:observesDaylightSavingsTime>false</ns2:observesDaylightSavingsTime>
               </ns2:timeZoneInfo>
               <ns2:awards/>
               <ns2:directBillingConfig participating="false"/>
               <ns2:alternativeCurrencyEnabled>false</ns2:alternativeCurrencyEnabled>
               <ns2:enableOverbookingRI>false</ns2:enableOverbookingRI>
               <ns2:paymentCardCollectedExternally>false</ns2:paymentCardCollectedExternally>
               <ns2:refurbishInfo/>
               <ns2:descriptions/>
               <ns2:contactInfo>
                  <ns2:hotelMailingAddress>
                     <ns1:line1>295 North W Temple Street</ns1:line1>
                     <ns1:city>Salt Lake City</ns1:city>
                     <ns1:postalCode>684257</ns1:postalCode>
                     <ns1:stateOrProvince>UT</ns1:stateOrProvince>
                     <ns1:country>US</ns1:country>
                  </ns2:hotelMailingAddress>
                  <ns2:hotelEmailAddresses>
                     <ns1:emailAddress kind="WORK">
                        <ns1:address>PD_UT320@parkinnamericas.com</ns1:address>
                     </ns1:emailAddress>
                  </ns2:hotelEmailAddresses>
                  <ns2:contactNumbers>
                     <ns1:phone kind="FAX">
                        <ns1:countryAccessCode>1</ns1:countryAccessCode>
                        <ns1:areaCode>707</ns1:areaCode>
                        <ns1:phoneNumber>584-8180</ns1:phoneNumber>
                     </ns1:phone>
                  </ns2:contactNumbers>
                  <ns2:urls/>
               </ns2:contactInfo>
               <ns1:relatedOrganizations>
                  <ns1:relatedOrganization>
                     <ns1:organization>
                        <ns1:organizationId>GLX</ns1:organizationId>
                        <ns1:name>Galaxy Hotels Group</ns1:name>
                     </ns1:organization>
                     <ns1:relationshipKind>MGTCO</ns1:relationshipKind>
                  </ns1:relatedOrganization>
                  <ns1:relatedOrganization>
                     <ns1:organization>
                        <ns1:organizationId>GLXCO</ns1:organizationId>
                        <ns1:name>Galaxy Hotels Group (CO)</ns1:name>
                     </ns1:organization>
                     <ns1:relationshipKind>CTRLO</ns1:relationshipKind>
                  </ns1:relatedOrganization>
               </ns1:relatedOrganizations>
               <ns2:acceptedPaymentForms>
                  <ns2:acceptedPaymentForm>
                     <ns2:code>AM</ns2:code>
                     <ns2:kind>PaymentCard</ns2:kind>
                     <ns2:description>Amoco Multicard</ns2:description>
                     <ns2:use guarantee="true" settlement="true" deposit="true"/>
                  </ns2:acceptedPaymentForm>
                  <ns2:acceptedPaymentForm>
                     <ns2:code>AX</ns2:code>
                     <ns2:kind>PaymentCard</ns2:kind>
                     <ns2:description>American Express</ns2:description>
                     <ns2:use guarantee="true" settlement="true" deposit="true"/>
                  </ns2:acceptedPaymentForm>
                  <ns2:acceptedPaymentForm>
                     <ns2:code>CB</ns2:code>
                     <ns2:kind>PaymentCard</ns2:kind>
                     <ns2:description>Carte Blanche</ns2:description>
                     <ns2:use guarantee="true" settlement="true" deposit="true"/>
                  </ns2:acceptedPaymentForm>
                  <ns2:acceptedPaymentForm>
                     <ns2:code>DC</ns2:code>
                     <ns2:kind>PaymentCard</ns2:kind>
                     <ns2:description>Diner's Club</ns2:description>
                     <ns2:use guarantee="true" settlement="true" deposit="true"/>
                  </ns2:acceptedPaymentForm>
                  <ns2:acceptedPaymentForm>
                     <ns2:code>DS</ns2:code>
                     <ns2:kind>PaymentCard</ns2:kind>
                     <ns2:description>Discover</ns2:description>
                     <ns2:use guarantee="true" settlement="true" deposit="true"/>
                  </ns2:acceptedPaymentForm>
                  <ns2:acceptedPaymentForm>
                     <ns2:code>JC</ns2:code>
                     <ns2:kind>PaymentCard</ns2:kind>
                     <ns2:description>Japan Credit Bureau</ns2:description>
                     <ns2:use guarantee="false" settlement="true" deposit="false"/>
                  </ns2:acceptedPaymentForm>
                  <ns2:acceptedPaymentForm>
                     <ns2:code>MC</ns2:code>
                     <ns2:kind>PaymentCard</ns2:kind>
                     <ns2:description>MasterCard</ns2:description>
                     <ns2:use guarantee="true" settlement="true" deposit="true"/>
                  </ns2:acceptedPaymentForm>
                  <ns2:acceptedPaymentForm>
                     <ns2:code>RD</ns2:code>
                     <ns2:kind>Voucher</ns2:kind>
                     <ns2:description>Guest Privileges</ns2:description>
                     <ns2:use guarantee="false" settlement="false" deposit="false"/>
                  </ns2:acceptedPaymentForm>
                  <ns2:acceptedPaymentForm>
                     <ns2:code>VI</ns2:code>
                     <ns2:kind>PaymentCard</ns2:kind>
                     <ns2:description>VISA</ns2:description>
                     <ns2:use guarantee="true" settlement="true" deposit="true"/>
                  </ns2:acceptedPaymentForm>
               </ns2:acceptedPaymentForms>
               <ns2:drivingDirections/>
               <ns2:destinations/>
               <ns2:groupPolicies/>
               <ns2:hotelManagement>
                  <ns2:generalManager>
                     <ns1:person>
                        <ns1:personName>
                           <ns1:given>Katie</ns1:given>
                           <ns1:surname>Gallegos</ns1:surname>
                        </ns1:personName>
                     </ns1:person>
                  </ns2:generalManager>
               </ns2:hotelManagement>
               <ns2:childrenStayFree>false</ns2:childrenStayFree>
               <ns2:paymentPolicy/>
               <ns2:roomTypes/>
               <ns2:meetingRooms>
                  <ns2:largestConferenceCapacity>0</ns2:largestConferenceCapacity>
                  <ns2:largestBanquetCapacity>0</ns2:largestBanquetCapacity>
               </ns2:meetingRooms>
               <ns2:mlosStrategy>Stay Through</ns2:mlosStrategy>
               <ns2:platformFeatures>
                  <ns1:attributes>
                     <ns1:attribute>
                        <ns1:key>AutoRollinAvailability</ns1:key>
                        <ns1:values>
                           <ns1:value>true</ns1:value>
                        </ns1:values>
                     </ns1:attribute>
                     <ns1:attribute>
                        <ns1:key>AdultsOnlyFeature</ns1:key>
                        <ns1:values>
                           <ns1:value>false</ns1:value>
                        </ns1:values>
                     </ns1:attribute>
                     <ns1:attribute>
                        <ns1:key>ParticipateCentralGroupProcessing</ns1:key>
                        <ns1:values>
                           <ns1:value>true</ns1:value>
                        </ns1:values>
                     </ns1:attribute>
                     <ns1:attribute>
                        <ns1:key>RateHurdlesEnabled</ns1:key>
                        <ns1:values>
                           <ns1:value>true</ns1:value>
                        </ns1:values>
                     </ns1:attribute>
                     <ns1:attribute>
                        <ns1:key>RoomTypeBucketDisplayOrder</ns1:key>
                        <ns1:values>
                           <ns1:value>false</ns1:value>
                        </ns1:values>
                     </ns1:attribute>
                  </ns1:attributes>
               </ns2:platformFeatures>
               <ns2:travelAgentTerms>
                  <ns2:travelAgentCommission>
                     <ns2:percentage>10</ns2:percentage>
                     <ns2:enabled>true</ns2:enabled>
                  </ns2:travelAgentCommission>
               </ns2:travelAgentTerms>
               <ns2:taxInclusive>false</ns2:taxInclusive>
               <ns2:specialInventory>
                  <ns2:items>
                     <ns2:id>
                        <ns1:id>494213</ns1:id>
                     </ns2:id>
                     <ns2:name>Crib</ns2:name>
                     <ns2:count>0</ns2:count>
                  </ns2:items>
                  <ns2:items>
                     <ns2:id>
                        <ns1:id>494214</ns1:id>
                     </ns2:id>
                     <ns2:name>Rollaway</ns2:name>
                     <ns2:count>0</ns2:count>
                  </ns2:items>
               </ns2:specialInventory>
               <ns2:marketSegment>
                  <ns2:segmentCode>17</ns2:segmentCode>
                  <ns2:name>Midscale</ns2:name>
               </ns2:marketSegment>
            </ns2:hotelDistribution>
         </ns0:response>
      </ns0:getHotelResponse>
   </S:Body>
</S:Envelope>
