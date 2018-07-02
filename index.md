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
  | Request Body |  |

 

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
