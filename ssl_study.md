# TLS and SSL

 TLS : transport layer security 
 Ssl : secure sockets layer 
 
 
 - ssl은 https에도 쓰임 

 ## 보장하는 것들 
 
 - message가 이동되는 동안 아무도 보지 않았다는 것
 
 - 아무도 메세지를 변경하지 않았다는 것
 
 - 의도한 사람과 메세지를 주고받는 것


## 보장하기 위한 해결점

- 메세지를 암호화함으로써 메세지를 특정 사람만 열어보게함 

- sign it : 받는 사람이 다른 사람이 열지 않았고 변경되지 않았음을 확인 


## public key와 private key 

- public key와 private key는 서로 key pair

- public key로 암호화된 message는 private key로 풀어야함

- public key는 아무나 받을 수 있음 

- public key가 자신만을 위한 key인지 판단은 ca를 통해함 

- private key는 오로지 한 곳만 가질 수 있음 


## CA

- certificate authority : certificate 발급해주는 곳 

- 사용자는 요구되는 정보를 넣고 certificate request를 함

- ca는 해당 정보를 보고 인증서를 받음(public key 동봉) 

- 여권(certificate)을 받기 위해서 여권 사무소(ca)에 신청하는 것과 같음 

- 파일 확장자는  .DER .PEM .CRT .CERT 등등

- ca는 certificate을 발급해주고 사용자는 certificate에 서명하면서 신뢰성 상승 


## Certificate types

### 1. Domain Validated Certificates(DVC)

- X509 digital certificate으로써 주로 tls(transport layer security)에서 사용

- 신청자의 신원이 어느정도 파악된 경우 

- 민감한 데이터가 아닌 일반 컨텐츠를 제공하는 웹사이트들이 사용

### 2. Extended Validation Certification(EVC)

- https website들에 사용

- 좀더 강화된 인증 







