# 플라스크 공부

## 기본 구조

- 모듈파일로 구성 

- 모듈파일을 import하는 순간 init.py는 저절로 구동 

- static에는 css images js등등 정적인 파일들이 존재

- template에는 html파일 들이 있음 
 - index.html 은 시작지점 
 
- init.py 에는 해당 모듈의 시작 지점을 기술  


- mvc 구조 사용 

  m은 model의 약자로써 데이너베이스와 연결되는 부분
  
  v는 view를 의미, 클라이언트가 보는 부분 
  
  
  c 는 routing 역할 (접근 url에 따라 비즈니스 로직이 수행되는 부분 )
  
  
 
## __init__.py

- from flask import Flask

- 플라스크 객체를 생성 

- 요청을 port(default:5000)로 받음

- 



