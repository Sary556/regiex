# 정규표현식
# /Regiex/ == > ReGular expression의 약자

# 언제 사용하는가?
  - 텍스트에서 우리가 원하는 특정한 패턴을 찾을때 (전화번호형태의 패턴,웹사이트주소형태의 패턴,이메일형식의 패턴을 찾을때 등등..)
  - 사용자가 입력한 텍스트가 이메일이나 패스워드와 같이 특정한 패턴에 부합하는지 유효성검사를 할때도 사용 할 수 있다.
  - 정규식은 문자를 검사하고자할때 사용하는 식이다.

# 정규식은 /로 시작하여 "나는 정규표현식"임을 나타낸다
  - /우리가 찾고자하는 패턴/

  - /regex/i
  - i는 어떤 옵션에 따라 검색할건지 플래그를 활용할 수 있다.



 #문법
  1) Groubs anf ranges

    - |   : 또는
    - ()  : 그룹
    - []  : 문자셋, 괄호안의 어떤 문자든
    - [^] : 부정 문자셋, 괄호안의 어떤문자가 아닐때
    - (?) : 찾지만 기억하지는 않음 

- |   : 또는
![image](https://github.com/Sary556/regiex/assets/141836031/b93a577b-0ff9-41a0-b9cd-ab84cd5fd0be)


- ()  : 그룹
![image](https://github.com/Sary556/regiex/assets/141836031/09ca90c3-5422-4f81-b790-2cc1d356fea9)


#  re로시작하고 중간글자가 fer 또는 can이 되고 ence로 끝나는걸 찾음 
![image](https://github.com/Sary556/regiex/assets/141836031/d3cd2ac1-792b-42a5-a52c-90336d4850d7)

![image](https://github.com/Sary556/regiex/assets/141836031/95b6f9b6-61ec-4805-94a3-e7dd021db681)



 
# 찾아는 지지만 그룹으로 만들고 싶지 않다면 사용
- (?) : 찾지만 기억하지는 않음 
![image](https://github.com/Sary556/regiex/assets/141836031/0f31ce74-5c62-4cba-9014-668ecc39219f)








# gr로 시작하고 a또는 e또는 d가 있고 y로 끝나는걸 찾음
- |   : 또는
- ()  : 그룹

![image](https://github.com/Sary556/regiex/assets/141836031/6efcdc85-cad2-4c09-a4d7-7bbc4f6f72fe)



- [aed] --> 대괄호 안에 있는 글자르 하나라도 만족하는것을 찾음
- []  : 문자셋, 괄호안의 어떤 문자든
![image](https://github.com/Sary556/regiex/assets/141836031/2647e1d3-0fd0-47fa-8979-7c80c77dcd9e)

# gr로시작하고 []A~G(ABCDEFG)사이의 글자를 하나라도 포함되고 y로 끝나면 찾음
![image](https://github.com/Sary556/regiex/assets/141836031/0ecae517-4a22-40cc-b934-193a1f9a1674)


