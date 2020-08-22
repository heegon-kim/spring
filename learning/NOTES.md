## 2020-07-28
### 스프링을 배우는 이유
실무에서 제대로 동작하는 웹 어플리케이션을 개발하기 위해서...

### 준비
요즘은 이클립스보다는 인텔리J를 많이 사용하는 추세   
https://www.jetbrains.com/ko-kr/idea/download/#section=windows   
   
스프링 부트 스타터 사이트로 이동해서 스프링 프로젝트 생성   
https://start.spring.io/   

### 프로젝트 생성
위의 스프링부트 링크에서 프로젝트를 생성
- 과거에는 Maven을 많이 사용하였으나 요즘은 Gradle로 넘어가는 추세   
- SNAPSHOT, M1은 정식 릴리즈 버전이 아님
- group은 보통 기업이름, Artifact는 빌드 결과물(프로젝트명)
- ADD DEPENDENCIES는 어떤 라이브러리를 추가할지 선택
  - Spring Web: Web개발 목적
  - Thymeleaf: HTML을 만들어주는 템플릿 엔진
   
      
IntelliJ에서 프로젝트 열기
- 위의 프로젝트를 zip파일로 다운받고 압축해제
- IntelliJ에서 'Open File or Project' 선택
- 압축해제한 폴더에 build.gradle을 선택하여 프로젝트를 열음
- src - main - java - hello - hellospring - .java - run
- localhost:8080

## 2020-08-20
### 컴파일 에러 java: Invalid Source Release: 11 Error
조치방법: https://www.programmersought.com/article/7983892146/
버전을 11에서 8로 낮춤.

### Welcome Page(=index.html) 생성
Spring사이트의 본문 설명: https://docs.spring.io/spring-boot/docs/current/reference/html/spring-boot-features.html#boot-features-spring-mvc-welcome-page
Welcome Page는 src-main-resources-static 디렉터리에 index.html(정적 페이지)로 생성

### 템플릿 엔진 사용 (thymeleaf)
https://docs.spring.io/spring-boot/docs/current/reference/html/spring-boot-features.html#boot-features-spring-mvc-template-engines

### controller 생성 및 사용
![Alt text](https://user-images.githubusercontent.com/57381163/90747569-0e76c980-e30c-11ea-90a5-517a4503525d.png)   
  
   
### 프로젝트 빌드 및 실행
![image](https://user-images.githubusercontent.com/57381163/90749481-74645080-e30e-11ea-8c40-f2a12f01f096.png) 
   
## 2020-08-22
### 정적 컨텐츠
파일을 고객에게 웹브라우저에 그-대로 전달.   
main - resouces - static - *.html   
웹 브라우저 -> 내장 톰캣 서버 -> 1. 스프링 컨테이너 or 2. resources: static/*.html -> 웹 브라우저
### MVC와 템플릿 엔진
Model-View-Controller의 구성으로 서버에서 html을 좀 변형시켜서 전달   
View: 화면을 그리는 부분에 집중   
Model, Controller: 비즈니스 로직, 내부적 처리에 집중   
### API
data를 전달하는 여러가지 방법(json. react..)

강의: https://www.inflearn.com/course/%EC%8A%A4%ED%94%84%EB%A7%81-%EC%9E%85%EB%AC%B8-%EC%8A%A4%ED%94%84%EB%A7%81%EB%B6%80%ED%8A%B8   
markdown 참고: https://gist.github.com/ihoneymon/652be052a0727ad59601#21-%ED%97%A4%EB%8D%94headers   
github에 spring 커밋하기: https://twoicefish-secu.tistory.com/121   
