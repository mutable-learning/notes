tags:: Software Development
topic:: [[Software Security]] 
softdev:: Unit 4 Outcome 2

-
- validates who someone is before they can access a system
- used in conjunction with [[User Authorisation]] to restrict access to systems and data
- commonly a username and password is required
- other possible methods of authenticaton include
	- biometrics
	- token-based
	- passwordless (using social account and OpenID Connect)
	- passkeys (using Fast Identity Online and special apps or a security key)
- **Two-Factor Authentication (2FA)** enhances security with passwords by requiring a second method of verifying the user, such as by sms (not very secure) or biometrics
	- **Multi-Factor Authentication** is the same but with a third or more steps added
- Password Rules
	- make passwords long (and complex if required)
	- make passwords unique (never re-use across systems)
	- make passwords random (don't use guessable patterns or personal info)
	- use a password manager
	- lockout after multiple failed attempts
	- use 2FA or MFA
	- log all activity and monitor logs for suspicious activity
	- don't use passwords if possible (use passwordless or passkeys)