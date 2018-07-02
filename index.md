---
---
# Welcome to Finvu
#### **Software prerequisite**
- Postman    _(URL : https://www.getpostman.com/)_

#### **API to enter your own sample data**

  - **Account Discover API**
    - URL : _http://<IP>:<Port>/ConnectHub/V1/Accounts/discover_
    - Key : `x-access-token`
    - Value :  `eyJraWQiOiJjb29raWVqYXIiLCJhbGciOiJSUzI1NiJ9.eyJpc3MiOiJjb29raWVqYXIiLCJleHAiOjE1NTk2NDE0MjIsImp0aSI6Im5tbWpnd3VGb21acjVWWm1NMjRhaHciLCJpYXQiOjE1MjgxMDU0MjIsIm5iZiI6MTUyODEwNTM2Miwic3ViIjoic29tZUFBIiwiZ3JvdXBzIjpbImFnZ3JlZ2F0b3IiXX0.lJsU7hdZo9NKLLz9PVa3TJYy-Xi-ZX94_IHnJd-XGr5Skc8iHXBo7FW1L65rA7cOb9Spmira9vulP_a_qsik2XktTWlBXoWcRnLl8LaPLTsUH8cHqrP57CXCdhR3jQAjvu1913r-82xbQGYbc_S8aET2p529jnsBQ3LCR8hhGSvPPF5lo7N3EZNxQOLK3YuKNhrkcUICD7OZcIHSsXhqJAsYnonsnj4nBImsnyz9MA3xYxW3vjMQI6XmgiFIjYRh9ddqfAEcIyYAeQUQ8U9HmBpEUboMwRbCmbGfbEeu6F2SpukhwoBYzHLFHUfOq8wVBsY3essYtVnlv8cGqsJsww`
    - Request Body
 ```<FIRequest ver="1.0" timestamp="2018-06-09T09:58:50.505Z" txnid="c5a1450c-d08a-45b4-a475-0468bd10e380">
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
  ```

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| URL      | _http://<IP>:<Port>/ConnectHub/V1/Accounts/discover_ | $1600 |
| Key      | x-access-token      |   $12 |
| Value | `eyJraWQiOiJjb29raWVqYXIiLCJhbGciOiJSUzI1NiJ9.eyJpc3MiOiJjb29raWVqYXIiLCJleHAiOjE1NTk2NDE0MjIsImp0aSI6Im5tbWpnd3VGb21acjVWWm1NMjRhaHciLCJpYXQiOjE1MjgxMDU0MjIsIm5iZiI6MTUyODEwNTM2Miwic3ViIjoic29tZUFBIiwiZ3JvdXBzIjpbImFnZ3JlZ2F0b3IiXX0.lJsU7hdZo9NKLLz9PVa3TJYy-Xi-ZX94_IHnJd-XGr5Skc8iHXBo7FW1L65rA7cOb9Spmira9vulP_a_qsik2XktTWlBXoWcRnLl8LaPLTsUH8cHqrP57CXCdhR3jQAjvu1913r-82xbQGYbc_S8aET2p529jnsBQ3LCR8hhGSvPPF5lo7N3EZNxQOLK3YuKNhrkcUICD7OZcIHSsXhqJAsYnonsnj4nBImsnyz9MA3xYxW3vjMQI6XmgiFIjYRh9ddqfAEcIyYAeQUQ8U9HmBpEUboMwRbCmbGfbEeu6F2SpukhwoBYzHLFHUfOq8wVBsY3essYtVnlv8cGqsJsww`      |    $1 |
