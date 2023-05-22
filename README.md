# About
DigiD Stub (FREE) - Emulates DigiD SAML2.0 IDP (Identity Provider)

DOWNLOAD FREE VERSION: https://www.arpha.nl/digid-stub/

Check all features below.

# License
See LICENSE.txt

# Author
Arpha B.V. @ [www.arpha.nl](https://www.arpha.nl) 

# Configuration
1. Configure IDP URL's in ```settings.php``` with public IP/hostname: ```sys_sso_url, sys_slo_url, sys_art_res_service_url, sys_entity_id```
2. Configure ```$sp_settings``` in ```settings.php```
3. Run ```create-certs.sh```
4. Optional: configure exposed ports in ```doker-compose.yml```

# How to run
1. ```./docker-compose up```
2. Open ``http://[sys_entity_id]/metadata/``
3. Import IDP-metadata in your SAML2.0 Service Provider
4. Initiate authentication from your application
5. :)

Feedback is welcome at [servicedesk@arpha.nl](mailto:servicedesk@arpha.nl)

# Features FREE version
- Dockerized application
- HTTP-redirect binding for Login
- Login screen with:
    - BSN generator
    - custom BSN input
    - authentication level select
- Automatic session cleaning

# Why buy the PRO version?
Our PRO version offers all features needed to fully test the authentication flow of your application. The PRO version also contains features which makes testing a lot easier and quicker to test different scenario's.
Features include:

- DigiD Stub PRO emulates a SAML2.0 IDP with the same behaviour as DigiD:
  - Redirect, POST, SOAP-binding
  - AuthnRequest front channel
  - Re-authentication (using cookie)
  - Backchannel ArtifactResolve & Response
  - LogoutRequest front channel 

- Provided as Docker image, which ensures easy deployment

- Written in PHP, easy to read and understand (not obfuscated)

- License allows for customisation for own use

- User interface (Login screen and BSN picker):
  - shows list of predefined BSN’s or lets tester pick random BSN
  - remembers last used BSN's 
  - lets tester pick desired authentication level

- Works without DB, making it extremely suitable for performance testing

- Support for different error scenario's, including canceling login and time-outs

- Supports multiple simultaneously connected SAML2.0 SP's (Service Providers)

- Outputs detailed debug logging for analysis

- One-time payment. Lifetime license to use


Please contact us at [servicedesk@arpha.nl](mailto:servicedesk@arpha.nl) if you are interested.

