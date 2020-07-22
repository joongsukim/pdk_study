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

