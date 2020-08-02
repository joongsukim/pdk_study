# 플라스크 공부

## 기본 구조

 - 모듈파일로 구성 

 - 모듈파일을 import하는 순간 init.py는 저절로 구동 

 - static에는 css images js등등 정적인 파일들이 존재

 - template에는 html파일 들이 있음   
   (index.html 은 시작지점) 
 
 - init.py 에는 해당 모듈의 시작 지점을 기술  


- mvc 구조 사용 

  + m은 model의 약자로써 데이너베이스와 연결되는 부분
  
  + v는 view를 의미, 클라이언트가 보는 부분 
  
  + c 는 routing 역할 (접근 url에 따라 비즈니스 로직이 수행되는 부분 )
  
## flask로 get,post 요청 보내기 

 - 사용되는 모듈(request,render_template)

 - request: 클라이언트에서 서버로 어떤 요청을 보낼지 정함
 
   + get : 모든 파라미터를 url로 보냄
   
   + post: 전달하려는 정보가 http body에 포함되어 전달 
   
'''  
 @app.route('/post',methods = ['POST'])
 def post():
    value = request.form['test']
    return value 
    
'''  

- client에서 form으로 정보를 보내서 서버쪽에서 처리 


    
   
- render_template : template 폴더안에 있는 html문서를 사용할때 사용 

'''  
@app.route('test')
def test():
    return render_template('post.html')
    
'''   
 
  post.html이라는 파일을 불러와 리턴 
  
 ## routing 
 
 - @app.route('/~')
 
 - 해당 url로 요청이 들어오면 정의된 함수를 호출 
 
 



