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


## CA

- certificate authority 

- 사용자는 요구되는 정보를 넣고 certificate request를 함

- ca는 해당 정보를 보고 인증서를 받음(public key 동봉) 

- 파일 확장자는  .DER .PEM .CRT .CERT 등등











