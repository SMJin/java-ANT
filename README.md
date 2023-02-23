![ANT](https://upload.wikimedia.org/wikipedia/commons/thumb/2/2f/Apache-Ant-logo.svg/220px-Apache-Ant-logo.svg.png)
# java-ANT
###### exercise example project with java build tool ANT

## What is Build tool ?
- 정형화되어 있는 반복적인 작업들을 자동화하기 위한 소프트웨어.
- Java를 예로 들어보면, .java 파일을 .class 파일로 변환하고 코드를 패키징해서 압축해서 환경에 배포하는 모든 일련의 활동을 개발자가 직접 했어야 했다. 그러나 초창기 빌드 소프트웨어 make로 시작해서 이러한 일련의 과정들을 편리하고 쉽게 한 번에 묶어서 처리가 가능하게 되었다.
- 수작업으로 진행되었던 빌드 과정을 자동화
- 빌드 과정에서 수정되어야 하는 부분들을 즉각적으로 반영. (작업 순서 및 변경 사항을 스크립트화)
- 환경에 의존적이지 않음. (ex) Window 환경이나 Linux 환경이 함께 빌드할 시 쉽게 대응이 가능. 
- 서로 의존적인 라이브러리들을 자동으로 불러옴. (무한 라이브러리 지옥에 갇히지 않음.)

## 빌드 툴 미사용
![BuildTool01](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FMmbxm%2FbtrJwYDH6S6%2FFK8e9VXv0k5IvqjkcTPL50%2Fimg.png)
![Buildtool02](https://blog.kakaocdn.net/dn/tCsTu/btrJrPIJEmi/6ZME7pbXxuwxPbGFWUDn1k/img.png)

## 빌드 툴을 활용하면
![BuildTool03](https://blog.kakaocdn.net/dn/Xbtlc/btrJwvhscaG/nBIcR8sRXN2XlJpm0ANtKk/img.png)
![Buildtool04](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2Fb9W8YO%2FbtrJt4MaXmD%2FHsvIjOv7wjtPEXGhov2lF0%2Fimg.png)

###### [이미지 출처](https://cornswrold.tistory.com/565?category=806549, "빌드툴이란 무엇인가?")

## What is ANT ?
- java + xml 기반의 build tool.
- 환경에 독립적 (운영체제가 다르거나 IDE가 달라도 같은 프로젝트 진행 가능)
- java 소스를 클래스(.class)파일로 compile 해서 배포본으로 변경해주고 API문서를 생성하는 등의 일련의 작업들을 "단 한번의 Batch 작업"으로 처리할 수 있도록 해주는 프로그램.
- 미리 정의된 태스크(task)를 이용하여 batch 작업 수행.
- 새로운 task의 추가로 batch 작업을 확장 가능.
- \bin : 실행 파일 (Ant 환경 변수 설정시에 이 경로로 ANT_HOME 지정)
- \lib : 핵심 package나 xml parser 등등 핵심 class library 보유.

## ANT의 구성요소
- project : 프로젝트 자체를 정의. 하나의 build.xml 당 하나의 프로젝트를 지님.
- target : 프로젝트가 수행할 작업 단위
- task : 프로젝트가 수행할 더 작은 작업의 단위
- property : Built-in Properties(시스템에 이미 만들어져있는 프로퍼티) / User defined Properties (사용자 지정 프로퍼티)
##### [Ant 구성요소 : 자세히](https://javacan.tistory.com/entry/60)
##### [Ant 간단한 예제](https://www.tutorialspoint.com/ant/ant_ifelse_arguments.htm)

## 이 git Repository에 추가한 ANT 소스 코드에 대한 결과
![image](https://user-images.githubusercontent.com/32761189/220858727-db265a8c-71c1-4f88-b5a0-8a8daf70e06f.png)

