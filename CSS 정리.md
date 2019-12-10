### CSS 정리###



> 사용법

1. HTML 문서에 <style> </style>을 삽입하여 CSS를 작성

2.  style= " " 속성으로 삽입

    ​



> CSS의 등장 배경

1. HTML로 디자인하는 것의 한계

2. HTML은 정보에 집중하고 디자인은 CSS에 맡김

   ​



> CSS의 장점

1. 가독성

2. 중복의 제거

3. 의도에 맞게 작업

   ​



> 선택자, 선언, 속성

p  { color:red; padding:5px;}

선택자 : p

선언 블록 : { }

선언 : color:red , padding:5px

속성: color , padding

속성값: red, 5px



> 선택자 종류

1. 태그 선택자

   p { } 

   - 태그를 선택

2. 클래스 선택자 .

   .p { }

   - 클래스를 선택
   - 클래스 선언은  class="클래스 이름" 으로 선언

3. id 선택자#

   // #p { }	

   - id를 선택
   - id선언은 id="아이디 이름"으로 선언



4. 선택자 우선순위 id>클래스>태그





> Block level element

화면 전체를 사용하는 태그 

- 선택자 선언부 안에 displat:inline 을 선언할 경우 사용하는 콘텐츠 만큼만 사용



> Inline element 

자신의 콘텐츠만큼 사용하는 태그

- 선택자 선언부 안에 display :block 을 선언할 경우 화면 전체를 사용



> Box model

<img src="https://user-images.githubusercontent.com/45009100/70387784-c0739d00-19ec-11ea-9d8d-7587f123dd9f.png" width="80%" >



> 의미가 없는 태그 div, span

디자인의 용도로 사용할 수 있는 태그

- div 는 block line element

- span은 inline element

  ​



> grid 템플릿

display:grid; //그리드 

**grid-template-columns: 150px 1fr**; //첫번째 div는 150픽셀의 열로 고정. 나머지는 자동으로 지정됨



> 반응형 웹 (mediaquery)

- 반응형 웹이란 기기마다 다른 화면크기에 맞춰 다른 정보를 보여주는 웹

  @media(max-width:800px){	//크기가 800보다 작으면

​                div{

​                    display:none;	//아무것도 안보임

​                }

​            }