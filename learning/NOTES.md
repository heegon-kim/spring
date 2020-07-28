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
