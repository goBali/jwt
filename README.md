# jwt

Welcome all to my JWT GO Package

To use the JWT, you must create a payload with the following struct

type PayLoad struct {
	Name      string
	Email     string
	MobileNbr string
	IpAddress string
}

All the above fields are optional and you can add more fields. 

MakeJwt
-------
Once you have created the payload, you can use the function MakeJwt with following parameters:

ExpiryTime (in minutes)
Payload    (you have just created)
SecretKey  (only you know)

The MakeJwt will provide you with a JWT which you will provide to the user of your application

ValidateJwt
----------
When a JWT is submitted by a user of your application, you will use the ValidateJwt to to validate if the JWT is correct and get the PayLoad. 
The following parameters are required:

Jwt (the JWT you have received)
SecretKey  (only you know and you have used in MakeJwt)

Cheers
See you soon in Bali






