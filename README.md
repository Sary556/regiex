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

  2) 제한하기위해서 사용하는
     ```
     - ? : 있거나 없거나 (zero or one)
     - * : 있거나 없거나 많거나 (zero or more)
     - + : 하나 또는 많거나 (one or more)
     - {n} : n번 반복
     - {min,} : 최소
     - {min,max} :  최소~최대
     ```

  4) 경계에 대한
     ```
     - \b : 단어경계
     - \B : 단어경계가 아닌것
     - ^  : 문장의 시작 ( []안에있는 [^]과 다른뜻임 )
     - $  : 문장의 끝
     ```

  6) 특징을 이용하는 방법
     ```
     - \ : 특수문자가 아닌 문자
     - . : 모든 어떤글자 특문 숫자 모두 포함하나봄(예제보고수정) (줄바꿈 문자제외??? <br/>같은건가)
     - \d : 숫자(digit)
     - \D : 숫자가 아닌것
     - \w : 문자(word)
     - \W : 문자가 아닌것
     - \s : 공백(Space)
     - \S : 공백이 아닌것
    ```

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

# a 부터 z까지 A부터 Z까지 0부터 9까지 하나라도 만족하면 모두찾음
![image](https://github.com/Sary556/regiex/assets/141836031/f4737460-d88a-4ab7-a84b-af3c63ededd7)

# ^ 부정을 붙혀서 그외 특수문자가 해당되는것을 찾음
    - [^] : 부정 문자셋, 괄호안의 어떤문자가 아닐때

![image](https://github.com/Sary556/regiex/assets/141836031/1c9e8b6e-cec2-48c2-b181-9f6ef8df9187)

![image](https://github.com/Sary556/regiex/assets/141836031/ce489866-cc49-47d3-8d60-3e90bebc7a5e)




# - ? : 있거나 없거나 (zero or one)


![image](https://github.com/Sary556/regiex/assets/141836031/a246726a-d4c0-4779-b501-970cce844134)

# - * : 있거나 없거나 많거나 (zero or more)


![image](https://github.com/Sary556/regiex/assets/141836031/228953bb-56c1-484b-94e8-57e61882835e)


# - + : 하나 또는 많거나 (one or more)


![image](https://github.com/Sary556/regiex/assets/141836031/0bb9b982-29c8-4ac6-9a92-794d677f029a)


# - {n} : n번 반복

![image](https://github.com/Sary556/regiex/assets/141836031/29a300b1-320f-45c8-b60d-203b656b9fbe)

![image](https://github.com/Sary556/regiex/assets/141836031/818d01ba-3df5-4192-b4ec-706a95f41e44)

![image](https://github.com/Sary556/regiex/assets/141836031/77197694-c5c0-4a86-9b71-25baed077ddf)



# - {min,} : 최소
최소를 모두 포함중

![image](https://github.com/Sary556/regiex/assets/141836031/6d6a4884-dad6-4cd0-b345-2e0e1b743479)


# - {min,max} :  최소~최대
마지막 graaaaa는 {2,4}의 4의 걸려서 5개가있기때문에 제한 

![image](https://github.com/Sary556/regiex/assets/141836031/61a24f98-fdf1-4a8c-8479-c9acaff4f681)




     - ? : 있거나 없거나 (zero or one)
     - * : 있거나 없거나 많거나 (zero or more)
     - + : 하나 또는 많거나 (one or more)
     - {n} : n번 반복
     - {min,} : 최소
     - {min,max} :  최소~최대



     

