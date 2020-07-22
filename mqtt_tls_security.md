# mqtt broker을 대상으로 tls security 적용

ca로 openssl사용 

ssl connection을 시험하기 위해서 paho python client사용

- openssl genrsa -out server.key 2048  ---> key 생성하는 command

- openssl req -new -x



key 발급 순서 

1. ca key pair 생성 (private key public key)

2. ca 인증서를 생성하고 ca key를 동봉시킴

3. broker key pair을 생성

4. broker 인증서를 생성

5. ca 인증서를 




## mosquitto에서 client certificate을 만들고 사용하는 법 


### mosquitto(mqtt broker)의 구성을 수정

- require_certificates  : client에게 인증서가 필요하다고 알려줌 -> true로 setting

- use_identity_as_username : mosquitto는 password file을 사용하지말고 인증서로부터 username을 가져가라고 지시 --> true로 setting 

- crlfile : client의 인증서를 폐지하고 싶을때 사용하는 certificate revocation file을 생성가능 


### client와 broker 모두 같은 ca(여권 사무소 같은 느낌)을 사용


