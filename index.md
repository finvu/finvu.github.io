---
---
# Welcome to Finvu
#### **Software prerequisite**
- Postman    _(URL : https://www.getpostman.com/)_

#### **API to enter your own sample data**

  - **Account Discover API**
	
  | Tables        | Are           |
  | ------------- |:-------------:|
  | URL      | _http://<<0.0.0.0>>:<<0000>>/ConnectHub/V1/Accounts/discover_ |
  | Key      | ```x-access-token```      |
  | Value | ```Please email us on info@cookiejar.co.in for value of key``` |
  
  Request Body

 

```
<?xml version="1.0" encoding="UTF-8"?>
<AccDiscoveryRequest xmlns="https://standards.rebit.org.in/aa" ver="1.0" timestamp="2018-05-22T17:30:15.239Z" txnid="8399263c-4a15-11e8-bcd1-0277a9fbfedc">
<Identifiers><Identifier category="STRONG" type="MOBILE" value="7030608902"></Identifier></Identifiers>
<FIPDetails name="string" id="string">
<FITypes>
<FIType1 name="DEPOSIT" value="string"></FIType1>
<FIType name="DEPOSIT" value="string"></FIType>
</FITypes>
</FIPDetails>
<Meta type="PERSON" value="string">
<DeviceInfo>
<Tag name="MOBILE" value="string"></Tag>
<Tag1 name="GEOCODE" value="string"></Tag1>
<Tag3 name="LOCATION" value="string"></Tag3>
<Tag4 name="IP" value="string"></Tag4>
<Tag5 name="TYPE" value="string"></Tag5>
<Tag6 name="ID" value="string"></Tag6>
<Tag7 name="OS" value="string"></Tag7>
<Tag8 name="APP" value="string"></Tag8>
<Tag9 name="CAPABILITY" value="string"></Tag9>
<Tag10 name="TELECOM" value="string"></Tag10>
</DeviceInfo>
</Meta>
</AccDiscoveryRequest>
```
Response Expected: 
```
<AccDiscoveryResponse><timestamp>1527010215239</timestamp><txnid>8399263c-4a15-11e8-bcd1-0277a9fbfedc</txnid><AuthenticatorType/><DiscoveredAccounts><DiscoveredAccounts><Account><FIType>DEPOSIT</FIType><accType>CURRENT</accType><accRefNumber>999</accRefNumber><maskedAccNumber>XXXXXXXXX3456</maskedAccNumber><aeba>N</aeba></Account></DiscoveredAccounts></DiscoveredAccounts></AccDiscoveryResponse>
  ```


  - **Account Linking API**
	
  | Tables        | Are           |
  | ------------- |:-------------:|
  | URL      | _http://<<0.0.0.0>>:<<0000>>/ConnectHub/V1/Accounts/{AccountRefNo}_ |
  | Key      | ```x-access-token```      |
  | Value | ```Please email us on info@cookiejar.co.in for value of key``` |
  
  e.g. URL : http://215.216.217.72:9090/ConnectHub/V1/Accounts/RefSBI004
  
  Request Body

 

```
<?xml version="1.0" encoding="UTF-8"?>
<AccLinkRequest xmlns="https://standards.rebit.org.in/aa" ver="1.0" timestamp="2018-05-09T17:51:18.412Z" callbackURL="string" txnid="f35761ac-4a18-11e8-96ff-0277a9fbfedc">
<AccDetails>
<Account FIType="DEPOSIT" accType="SAVINGS" accRefNumber="RefSBI001" maskedAccNumber="SBI111111111111" aeba="Y"></Account>
<FIPDetails id="string" name="string"></FIPDetails>
</AccDetails>
</AccLinkRequest>
```
Response Expected: 

```
<AccLinkResponse><ver>1.0</ver><timestamp>1529153879076</timestamp><txnid>f35761ac-4a18-11e8-96ff-0277a9fbfedc</txnid><Account><FIType>DEPOSIT</FIType><accType>SAVINGS</accType><accRefNumber>999</accRefNumber><maskedAccNumber>XXXXXXXXX3456</maskedAccNumber><aeba>Y</aeba></Account></AccLinkResponse>
```


  - **Account Confirm Token API**
	
  | Tables        | Are           |
  | ------------- |:-------------:|
  | URL      | _http://<<0.0.0.0>>:<<0000>>/ConnectHub/V1/Accounts/{AccountRefNo}/confirm-token_ |
  | Key      | ```x-access-token```      |
  | Value | ```Please email us on info@cookiejar.co.in for value of key``` |
  
  e.g. URL : http://215.216.217.72:9090/ConnectHub/V1/Accounts/RefSBI001/confirm-token
  
  Request Body
  Put the SMS received on mobile in <token>{OTP sms}</token>
 

```
<?xml version="1.0" encoding="UTF-8"?>
<ConfirmLinkingRequest ver="1.0"
timestamp="2018-05-05T10:27:17.699Z"
txnid="410c2d2e-4a1e-11e8-960e-0277a9fbfedc">
<token>774265</token>
</ConfirmLinkingRequest>
```
Response Expected: 

```
<ConfirmLinkingResponse><ver>1.0</ver><timestamp>1525516037699</timestamp><txnid>410c2d2e-4a1e-11e8-960e-0277a9fbfedc</txnid></ConfirmLinkingResponse>
```
