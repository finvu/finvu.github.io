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
    <FIRequest ver="1.0" timestamp="2018-06-09T09:58:50.505Z" txnid="c5a1450c-d08a-45b4-a475-0468bd10e380">
	<ConsentID>c4a1450c-d08a-45b4-a475-0468bd10e380</ConsentID>
		<DataConsumer id="123456@finvu.in" type="AA" callbackURL="localhost:9090/AA/Test"></DataConsumer>
	<RequestFIParams>
		<KeyMaterials>
			<KeyMaterial startTime="2018-06-01T09:58:50.505Z">
				<SessionID>string</SessionID>
				<DHPublicKey expiry="2019-06-01T09:58:50.505Z">
					<Parameters>Param 1</Parameters>
					<KeyValue>W0C9Z43fLvtE1ab6itHiZy/5Cc4zvh8r80YQc0ezqAo=</KeyValue>
				</DHPublicKey>
				<Nonce>12345</Nonce>
				<Signature> Signature Value</Signature>
			</KeyMaterial>
		</KeyMaterials>
	</RequestFIParams>
</FIRequest> 
