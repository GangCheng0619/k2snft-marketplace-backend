# icicb-portal-backend
### Error Code
| code | message | meaning |
| --- | --- | --- |
| 1001 | RECAPTCHA_INVALID | RECAPTCHA_INVALID
| 1002 | RECAPTCHA_FAILED | RECAPTCHA_FAILED
| 1003 | invalid password | invalid password length
| 1004 | unregistered user | unregistered user in server
| 1005 | no permission | the user haven't login permision
| 1006 | wrong password | password is wrong
| 1007 | duplicated | target already exist
| 1008 | already logged | already logged
| 2000 | login | require login.
| 2001 | invalid code | code must be 6 digits number.
| 2002 | unknown coin | unknown coin
| 2003 | not enough | not enough balance for purchasing ICICB or transfer
| 2004 | applied | you have already applied.
| 2005 | invalid code | the code is invalid
| 2006 | already used | the code already used by other person.
| 2007 | already taken | wallet already taken by you.
| 2008 | invalid amount | invalid amount
| 2009 | invalid chain | invalid chain
| 2010 | no address | there is no free address in system 
| 2011 | not enough fee | there is not enough tokens for pay transaction fee
| 10000 | admin only | admin only
| 10001 | zero length array | zero length array
| 10002 | invalid data format | invalid data format
| -32700 | Parse error | Invalid JSON was received by the server. An error occurred on the server while parsing the JSON text. |
| -32600 | Invalid Request | The JSON sent is not a valid Request object. |
| -32601 | Method not found | The method does not exist / is not available. |
| -32602 | Invalid params | Invalid method parameter(s). |
| -32603 | Internal error | Internal JSON-RPC error. |
| -32000 | Server error | Reserved for implementation-defined server-errors. |
| -32001 | ChainApi Server error | api server-errors. |
## API
	

changed v1.1 what's new:
```
	changed type name PincodeReqeustType to CodeReqeustType
	added some fields in type LoginResponseType.
	affected apis
		/portal/login

	added type
		WalletReqeustType
		AdminQueryType
		AdminCreateType
		AdminUpdateType
		AdminDeleteType
		AdminUserType
		AdminPresaleCodeResponseType
		AdminVoucherCodeType

	added new api:
		/portal/get-user-wallet
		/portal/set-presale-code
		/portal/set-voucher
		/admin/login
		/admin/get-users
		/admin/create-user
		/admin/update-user
		/admin/delete-user
		/admin/get-presale-code
		/admin/import-presale-code
		/admin/get-voucher
		/admin/import-voucher
		/admin/get-wallets
		/admin/import-wallets
```
