# APACHE SSL

* 정상 설치시

``` [apache@TEST2 bin]$ openssl s_client –connect localhost:443
CONNECTED(00000003)
depth=3 C = GB, ST = Greater Manchester, L = Salford, O = Comodo CA Limited, CN = AAA Certificate Services
verify return:1
depth=2 C = US, ST = New Jersey, L = Jersey City, O = The USERTRUST Network, CN = USERTrust RSA Certification Authority
verify return:1
depth=1 C = GB, ST = Greater Manchester, L = Salford, O = Sectigo Limited, CN = Sectigo RSA Organization Validation Secure Server CA
verify return:1
depth=0 C = KR, ST = Gyeonggi-Do, L = "Bundang-gu, Seongnam-si", O = KT Corporation, OU = IT, OU = "Hosted by Korea Information Certificate Authority, Inc.", OU = InstantSSL, CN = ibotcms.kt.co.kr
verify return:1
---
Certificate chain
0 s:/C=KR/ST=Gyeonggi-Do/L=Bundang-gu, Seongnam-si/O=KT Corporation/OU=IT/OU=Hosted by Korea Information Certificate Authority, Inc./OU=InstantSSL/CN=ibotcms.kt.co.kr
   i:/C=GB/ST=Greater Manchester/L=Salford/O=Sectigo Limited/CN=Sectigo RSA Organization Validation Secure Server CA 
1 s:/C=GB/ST=Greater Manchester/L=Salford/O=Sectigo Limited/CN=Sectigo RSA Organization Validation Secure Server CA
   i:/C=US/ST=New Jersey/L=Jersey City/O=The USERTRUST Network/CN=USERTrust RSA Certification Authority
2 s:/C=US/ST=New Jersey/L=Jersey City/O=The USERTRUST Network/CN=USERTrust RSA Certification Authority
   i:/C=GB/ST=Greater Manchester/L=Salford/O=Comodo CA Limited/CN=AAA Certificate Services
3 s:/C=GB/ST=Greater Manchester/L=Salford/O=Comodo CA Limited/CN=AAA Certificate Services
   i:/C=GB/ST=Greater Manchester/L=Salford/O=Comodo CA Limited/CN=AAA Certificate Services
---
Server certificate
-----BEGIN CERTIFICATE-----
MIIG8jCCBdqgAwIBAgIRAII1DmNlsZQMTjFRk43QpnYwDQYJKoZIhvcNAQELBQAw
gZUxCzAJBgNVBAYTAkdCMRswGQYDVQQIExJHcmVhdGVyIE1hbmNoZXN0ZXIxEDAO
BgNVBAcTB1NhbGZvcmQxGDAWBgNVBAoTD1NlY3RpZ28gTGltaXRlZDE9MDsGA1UE
AxM0U2VjdGlnbyBSU0EgT3JnYW5pemF0aW9uIFZhbGlkYXRpb24gU2VjdXJlIFNl
cnZlciBDQTAeFw0xOTA5MzAwMDAwMDBaFw0yMDExMjgyMzU5NTlaMIHdMQswCQYD
VQQGEwJLUjEUMBIGA1UECBMLR3llb25nZ2ktRG8xIDAeBgNVBAcTF0J1bmRhbmct
Z3UsIFNlb25nbmFtLXNpMRcwFQYDVQQKEw5LVCBDb3Jwb3JhdGlvbjELMAkGA1UE
CxMCSVQxQDA+BgNVBAsTN0hvc3RlZCBieSBLb3JlYSBJbmZvcm1hdGlvbiBDZXJ0
aWZpY2F0ZSBBdXRob3JpdHksIEluYy4xEzARBgNVBAsTCkluc3RhbnRTU0wxGTAX
BgNVBAMTEGlib3RjbXMua3QuY28ua3IwggEiMA0GCSqGSIb3DQEBAQUAA4IBDwAw
ggEKAoIBAQClg3/v62KjrrdyDuDgQk0IxAtotQDV3JXUExV1uTZ+ZBs33Kh1KRS1
p+LTd1+PLDBr3WQw/j/mcpqoGE0DhnXe3Ay6LV/5Hjkw4Z8ybmPqzAvveWvZQRWk
v8W/SCXc7VCEqArdyMQpM0hwAvN4cag3D1lNpNygni7RwS9kpbNDqUQ7Hmjp0g+i
boue/aTdkA/y0H6AundHsHzNBZb/LmbwBnv+QDBwquKgjTi1N7F1pJxfAq7kCOwZ
2ZeLUBvz/Ul1TIlRbnrco6R5UOavRzCEhLA4b4Hq2vF6IH87Iq/79p0MSa/RrdHz
LMyV1McnSoFz4GJx6mDNRWbkbI8TG6rzAgMBAAGjggLxMIIC7TAfBgNVHSMEGDAW
gBQX2dYlJ2f5McJJQ9kwNkSMbKlP6zAdBgNVHQ4EFgQUb0bqpRLY8bWf0+r2jp9A
Ss85byAwDgYDVR0PAQH/BAQDAgWgMAwGA1UdEwEB/wQCMAAwHQYDVR0lBBYwFAYI
KwYBBQUHAwEGCCsGAQUFBwMCMEoGA1UdIARDMEEwNQYMKwYBBAGyMQECAQMEMCUw
IwYIKwYBBQUHAgEWF2h0dHBzOi8vc2VjdGlnby5jb20vQ1BTMAgGBmeBDAECAjBa
BgNVHR8EUzBRME+gTaBLhklodHRwOi8vY3JsLnNlY3RpZ28uY29tL1NlY3RpZ29S
U0FPcmdhbml6YXRpb25WYWxpZGF0aW9uU2VjdXJlU2VydmVyQ0EuY3JsMIGKBggr
BgEFBQcBAQR+MHwwVQYIKwYBBQUHMAKGSWh0dHA6Ly9jcnQuc2VjdGlnby5jb20v
U2VjdGlnb1JTQU9yZ2FuaXphdGlvblZhbGlkYXRpb25TZWN1cmVTZXJ2ZXJDQS5j
cnQwIwYIKwYBBQUHMAGGF2h0dHA6Ly9vY3NwLnNlY3RpZ28uY29tMDEGA1UdEQQq
MCiCEGlib3RjbXMua3QuY28ua3KCFHd3dy5pYm90Y21zLmt0LmNvLmtyMIIBBAYK
KwYBBAHWeQIEAgSB9QSB8gDwAHUAsh4FzIuizYogTodm+Su5iiUgZ2va+nDnsklT
Le+LkF4AAAFtgFU59gAABAMARjBEAiBP0iBIrxKOAsk0LFjUaP7KquqjcXgovbbr
s9dUNQ5IWgIge1hEIG+dOw75hSoqmOsTqc6OLIl3+SjWbOSDaJlyBH8AdwBep3P5
31bA57U2SH3QSeAyepGaDIShEhKEGHWWgXFFWAAAAW2AVTp0AAAEAwBIMEYCIQCC
8CjfFJ4SN2iYuYIkHqqq836e+GRTH6xywfURrGPa4QIhALUGMT2cnNr7jvzFoQ0V
Kw3e/+ffAOBCbOifZTiC2njBMA0GCSqGSIb3DQEBCwUAA4IBAQBZ4W5vDn3z1Tra
CtW9m2CEwpYcT/D3imL7bDIbd9HGyfnuuddyNzM1BWUc9PnBaGsDuK1ppwgrGHbt
YbwXmwx5oYqJydjzTc26eLnPxK7W3HAF002ZQR6Q0ObYKF1kC5ZQoNqU5o7WKXg9
+CS0f8LB80TPmwZrhx4KoTCuX2hAI8o1txaTB1eRXAyKzbSijutyh3TWJ5+OpYYO
UaEgm0lbKrWtZBvZrcsRR4KcRycaY6/fnnuUpKROCNnwDNSAe0wzvKC41gM3RtT0
qyqgaTyNk4rlsWkWCds/QIwnZwPfahZZC/n+sayU7uJX4xEV47g1nwlD2OnxYvBk
IZWNL33g
-----END CERTIFICATE-----
subject=/C=KR/ST=Gyeonggi-Do/L=Bundang-gu, Seongnam-si/O=KT Corporation/OU=IT/OU=Hosted by Korea Information Certificate Authority, Inc./OU=InstantSSL/CN=ibotcms.kt.co.kr
issuer=/C=GB/ST=Greater Manchester/L=Salford/O=Sectigo Limited/CN=Sectigo RSA Organization Validation Secure Server CA
---
No client certificate CA names sent
Server Temp Key: ECDH, prime256v1, 256 bits
---
SSL handshake has read 6538 bytes and written 373 bytes
---
New, TLSv1/SSLv3, Cipher is ECDHE-RSA-AES256-GCM-SHA384
Server public key is 2048 bit
Secure Renegotiation IS supported
Compression: NONE
Expansion: NONE
SSL-Session:
    Protocol  : TLSv1.2
    Cipher    : ECDHE-RSA-AES256-GCM-SHA384
    Session-ID: A8D73AEED580F1FC39D031AE5DADBC6D741B2B7FC340EAFB23557DA28971D71C
    Session-ID-ctx:
    Master-Key: 76B0E9D229667E420B3502007EFB3A29F4D1390E8460346082FA80173974F847140347FFA153CB06FFE893DC72AB181F
    Key-Arg   : None
    Krb5 Principal: None
    PSK identity: None
    PSK identity hint: None
    TLS session ticket lifetime hint: 300 (seconds)
    TLS session ticket:
    0000 - f2 a7 2b 93 6b 11 95 0a-ee b1 08 bd 99 40 04 1e   ..+.k........@..
    0010 - a8 e5 26 fd d8 06 9d 7f-be 36 78 cd cd 29 a3 d7   ..&......6x..)..
    0020 - 33 e3 dd b9 56 97 12 59-c1 e6 c7 1f 92 e1 99 e7   3...V..Y........
    0030 - e1 1a e8 c0 f1 eb 42 48-d8 c3 9b 00 ac 5a 72 28   ......BH.....Zr(
    0040 - 9d 3c d7 0d 0f ca 49 d5-dd 66 de 55 9b 4c 7a 48   .<....I..f.U.LzH
    0050 - f8 9c e7 a8 d9 ed d8 81-be 2f 75 ff fa 7d e2 12   ........./u..}..
    0060 - 0c f9 9d 30 d4 f6 cc 22-e0 44 11 75 6d f4 5e 68   ...0...".D.um.^h
    0070 - 85 2c 59 bb cb cc 8f 83-2a 71 03 2a d2 8d a7 d9   .,Y.....*q.*....
    0080 - f0 1b f6 e1 29 ba 6c 7e-32 fc 9a b0 2a 50 f6 a9   ....).l~2...*P..
    0090 - e3 56 8d 4a c2 68 bd c8-26 ce 67 13 54 49 3f 32   .V.J.h..&.g.TI?2
    00a0 - 13 d9 54 0d 13 fb 16 d6-d3 3b d2 e0 33 29 d6 ce   ..T......;..3)..
    00b0 - c6 4a 5f ec 9c 19 b9 97-f9 ef 38 e2 22 cb 99 6d   .J_.......8."..m
 
    Start Time: 1574815921
    Timeout   : 300 (sec)
    Verify return code: 0 (ok) ```

* Chain 인증서 미 설정시
	* 제일 하단의 Verify return code: 21 (unable to verify the first certificate)

``` [apache@TEST2 bin]$ openssl s_client -connect localhost:443
CONNECTED(00000003)
depth=0 C = KR, ST = Gyeonggi-Do, L = "Bundang-gu, Seongnam-si", O = KT Corporation, OU = IT, OU = "Hosted by Korea Information Certificate Authority, Inc.", OU = InstantSSL, CN = ibotcms.kt.co.kr
verify error:num=20:unable to get local issuer certificate
verify return:1
depth=0 C = KR, ST = Gyeonggi-Do, L = "Bundang-gu, Seongnam-si", O = KT Corporation, OU = IT, OU = "Hosted by Korea Information Certificate Authority, Inc.", OU = InstantSSL, CN = ibotcms.kt.co.kr
verify error:num=27:certificate not trusted
verify return:1
depth=0 C = KR, ST = Gyeonggi-Do, L = "Bundang-gu, Seongnam-si", O = KT Corporation, OU = IT, OU = "Hosted by Korea Information Certificate Authority, Inc.", OU = InstantSSL, CN = ibotcms.kt.co.kr
verify error:num=21:unable to verify the first certificate
verify return:1
---
Certificate chain
0 s:/C=KR/ST=Gyeonggi-Do/L=Bundang-gu, Seongnam-si/O=KT Corporation/OU=IT/OU=Hosted by Korea Information Certificate Authority, Inc./OU=InstantSSL/CN=ibotcms.kt.co.kr
   i:/C=GB/ST=Greater Manchester/L=Salford/O=Sectigo Limited/CN=Sectigo RSA Organization Validation Secure Server CA
---
Server certificate
-----BEGIN CERTIFICATE-----
MIIG8jCCBdqgAwIBAgIRAII1DmNlsZQMTjFRk43QpnYwDQYJKoZIhvcNAQELBQAw
gZUxCzAJBgNVBAYTAkdCMRswGQYDVQQIExJHcmVhdGVyIE1hbmNoZXN0ZXIxEDAO
BgNVBAcTB1NhbGZvcmQxGDAWBgNVBAoTD1NlY3RpZ28gTGltaXRlZDE9MDsGA1UE
AxM0U2VjdGlnbyBSU0EgT3JnYW5pemF0aW9uIFZhbGlkYXRpb24gU2VjdXJlIFNl
cnZlciBDQTAeFw0xOTA5MzAwMDAwMDBaFw0yMDExMjgyMzU5NTlaMIHdMQswCQYD
VQQGEwJLUjEUMBIGA1UECBMLR3llb25nZ2ktRG8xIDAeBgNVBAcTF0J1bmRhbmct
Z3UsIFNlb25nbmFtLXNpMRcwFQYDVQQKEw5LVCBDb3Jwb3JhdGlvbjELMAkGA1UE
CxMCSVQxQDA+BgNVBAsTN0hvc3RlZCBieSBLb3JlYSBJbmZvcm1hdGlvbiBDZXJ0
aWZpY2F0ZSBBdXRob3JpdHksIEluYy4xEzARBgNVBAsTCkluc3RhbnRTU0wxGTAX
BgNVBAMTEGlib3RjbXMua3QuY28ua3IwggEiMA0GCSqGSIb3DQEBAQUAA4IBDwAw
ggEKAoIBAQClg3/v62KjrrdyDuDgQk0IxAtotQDV3JXUExV1uTZ+ZBs33Kh1KRS1
p+LTd1+PLDBr3WQw/j/mcpqoGE0DhnXe3Ay6LV/5Hjkw4Z8ybmPqzAvveWvZQRWk
v8W/SCXc7VCEqArdyMQpM0hwAvN4cag3D1lNpNygni7RwS9kpbNDqUQ7Hmjp0g+i
boue/aTdkA/y0H6AundHsHzNBZb/LmbwBnv+QDBwquKgjTi1N7F1pJxfAq7kCOwZ
2ZeLUBvz/Ul1TIlRbnrco6R5UOavRzCEhLA4b4Hq2vF6IH87Iq/79p0MSa/RrdHz
LMyV1McnSoFz4GJx6mDNRWbkbI8TG6rzAgMBAAGjggLxMIIC7TAfBgNVHSMEGDAW
gBQX2dYlJ2f5McJJQ9kwNkSMbKlP6zAdBgNVHQ4EFgQUb0bqpRLY8bWf0+r2jp9A
Ss85byAwDgYDVR0PAQH/BAQDAgWgMAwGA1UdEwEB/wQCMAAwHQYDVR0lBBYwFAYI
KwYBBQUHAwEGCCsGAQUFBwMCMEoGA1UdIARDMEEwNQYMKwYBBAGyMQECAQMEMCUw
IwYIKwYBBQUHAgEWF2h0dHBzOi8vc2VjdGlnby5jb20vQ1BTMAgGBmeBDAECAjBa
BgNVHR8EUzBRME+gTaBLhklodHRwOi8vY3JsLnNlY3RpZ28uY29tL1NlY3RpZ29S
U0FPcmdhbml6YXRpb25WYWxpZGF0aW9uU2VjdXJlU2VydmVyQ0EuY3JsMIGKBggr
BgEFBQcBAQR+MHwwVQYIKwYBBQUHMAKGSWh0dHA6Ly9jcnQuc2VjdGlnby5jb20v
U2VjdGlnb1JTQU9yZ2FuaXphdGlvblZhbGlkYXRpb25TZWN1cmVTZXJ2ZXJDQS5j
cnQwIwYIKwYBBQUHMAGGF2h0dHA6Ly9vY3NwLnNlY3RpZ28uY29tMDEGA1UdEQQq
MCiCEGlib3RjbXMua3QuY28ua3KCFHd3dy5pYm90Y21zLmt0LmNvLmtyMIIBBAYK
KwYBBAHWeQIEAgSB9QSB8gDwAHUAsh4FzIuizYogTodm+Su5iiUgZ2va+nDnsklT
Le+LkF4AAAFtgFU59gAABAMARjBEAiBP0iBIrxKOAsk0LFjUaP7KquqjcXgovbbr
s9dUNQ5IWgIge1hEIG+dOw75hSoqmOsTqc6OLIl3+SjWbOSDaJlyBH8AdwBep3P5
31bA57U2SH3QSeAyepGaDIShEhKEGHWWgXFFWAAAAW2AVTp0AAAEAwBIMEYCIQCC
8CjfFJ4SN2iYuYIkHqqq836e+GRTH6xywfURrGPa4QIhALUGMT2cnNr7jvzFoQ0V
Kw3e/+ffAOBCbOifZTiC2njBMA0GCSqGSIb3DQEBCwUAA4IBAQBZ4W5vDn3z1Tra
CtW9m2CEwpYcT/D3imL7bDIbd9HGyfnuuddyNzM1BWUc9PnBaGsDuK1ppwgrGHbt
YbwXmwx5oYqJydjzTc26eLnPxK7W3HAF002ZQR6Q0ObYKF1kC5ZQoNqU5o7WKXg9
+CS0f8LB80TPmwZrhx4KoTCuX2hAI8o1txaTB1eRXAyKzbSijutyh3TWJ5+OpYYO
UaEgm0lbKrWtZBvZrcsRR4KcRycaY6/fnnuUpKROCNnwDNSAe0wzvKC41gM3RtT0
qyqgaTyNk4rlsWkWCds/QIwnZwPfahZZC/n+sayU7uJX4xEV47g1nwlD2OnxYvBk
IZWNL33g
-----END CERTIFICATE-----
subject=/C=KR/ST=Gyeonggi-Do/L=Bundang-gu, Seongnam-si/O=KT Corporation/OU=IT/OU=Hosted by Korea Information Certificate Authority, Inc./OU=InstantSSL/CN=ibotcms.kt.co.kr
issuer=/C=GB/ST=Greater Manchester/L=Salford/O=Sectigo Limited/CN=Sectigo RSA Organization Validation Secure Server CA
---
No client certificate CA names sent
Server Temp Key: ECDH, prime256v1, 256 bits
---
SSL handshake has read 2473 bytes and written 373 bytes
---
New, TLSv1/SSLv3, Cipher is ECDHE-RSA-AES256-GCM-SHA384
Server public key is 2048 bit
Secure Renegotiation IS supported
Compression: NONE
Expansion: NONE
SSL-Session:
    Protocol  : TLSv1.2
    Cipher    : ECDHE-RSA-AES256-GCM-SHA384
    Session-ID: 77E6ABAF8D5E71DEFF675FBA07F27FECA7C83A22F920A3503615EA9FBF7D794C
    Session-ID-ctx:
    Master-Key: F62A2C338BDADB71AF14C9A70E6B3343089F6B8D2028545B768927E41C75DC9D883A6C216EDB5E2E8D7F5CA7D03349E8
    Key-Arg   : None
    Krb5 Principal: None
    PSK identity: None
    PSK identity hint: None
    TLS session ticket lifetime hint: 300 (seconds)
    TLS session ticket:
    0000 - 21 1c c0 b1 47 37 b1 5a-98 87 e8 ee c4 4f 8d 9b   !...G7.Z.....O..
    0010 - 0c 64 a0 8e 53 02 3c d6-e1 a5 87 e7 a0 15 24 e3   .d..S.<.......$.
    0020 - 32 b0 cc dd e8 ff e4 c0-c9 7d d8 51 63 00 fb a0   2........}.Qc...
    0030 - fd 2f c0 f7 14 ec 0b 6a-f9 ef 36 69 46 3a dc ca   ./.....j..6iF:..
    0040 - 38 97 2e 17 9f fa 67 27-a1 2c 38 a4 f4 f0 a9 eb   8.....g'.,8.....
    0050 - 52 c3 f1 5e 9a 07 43 fd-c4 f5 b8 77 fe 6f 01 ef   R..^..C....w.o..
    0060 - fc 7d f5 ea 30 8c 04 38-73 09 75 f3 b5 79 d8 97   .}..0..8s.u..y..
    0070 - af 0d 85 2c 10 fb d3 27-f9 00 1d d8 43 fe fc 6f   ...,...'....C..o
    0080 - 37 45 5e f7 d8 0f c0 0c-d6 7b b4 de 32 07 0d 3e   7E^......{..2..>
    0090 - 8b b4 bc ac bf a4 80 1c-f6 02 52 03 c0 3c 0c 6e   ..........R..<.n
    00a0 - 41 e8 85 5a 6d 67 eb 5f-24 6a 36 a2 65 39 9d ba   A..Zmg._$j6.e9..
    00b0 - 0d 92 ba 96 60 60 6f 19-42 b2 4b eb 0e b6 0c 61   ....``o.B.K....a
 
    Start Time: 1574816019
    Timeout   : 300 (sec)
    Verify return code: 21 (unable to verify the first certificate)
---
closed ```

* 신뢰하지 못하는 ROOT인증서 일 경우
```	제일하단의 Verify return Code:19 ( Self Signed Certifitcate in certificate chain)
		-       사설 인증서 일 경우
		-       OS에서 신뢰할수 있는 ROOT인증서로 미등록이 된 경우```
