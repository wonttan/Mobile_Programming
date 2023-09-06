# Mobile_Programming
컴퓨터공학과 모바일 프로그래밍 정리입니다.

## 23.09.06 프로젝트 개발 일지
[SplashActivity 3초간 지속 후 IntroActivity로 변경]
![image](https://github.com/wonttan/Mobile_Programming/assets/58906858/63361fdc-ecbe-484d-aa3e-37297a21537b)   
[auth패키지의 IntroActivity 화면]
![image](https://github.com/wonttan/Mobile_Programming/assets/58906858/dbd816b9-cd83-4d6f-afd6-05c2748ad7f3)
```
SplashActivity 화면을 구현한 후에 배경색을 노랑색으로 변경하고
로고 이미지를 다운받아서 Split으로 화면의 정중앙에 위치시켰다.
또 메인화면으로 바로 SplashActivity가 나올 수 있도록 AndroidManifest 에서 intent 태그를 SplashActivity 안으로 넣어주었다.

values/themes.xml에서 WindowNoTitle 값을 True로 줘서 타이틀 바를 없앴다.
values/colors.xml에서 mainColor를 정의하여 색상코드없이 사용할 수 있도록 하였다.
상태표시바 colorPrimaryVariant를 mainColor로 변경하여 전체적인 색상의 통일성을 부여하였다.

다음으로 로그인,로그아웃,회원가입 등 계정인증과 관련한 패키지 auth를 생성하고
패키지 안에 IntroActivity를 생성하였다.

SplashActivity를 3초간 띄우고 IntroActivity를 띄우도록 Handler.postDelayed를 사용하였다.

플러터를 사용할 때보다 핫리로드 기능이 없다는 단점과
layout의 Split에서 로고의 위치를 마우스로 설정할 수 있다는 장점을 발견하였다.

다음으로 auth 패키지 안의 IntroActivity를 꾸며준다.
```
