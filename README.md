# Flutter 개발 환경 설정

## Windows

### flutter install 

[flutter install](https://flutter.dev/docs/get-started/install/windows)에 접속하여 SDK 다운로드.

![SDK 다운로드](https://github.com/kjk7034/FlutterSetup/blob/master/mages/winSetup01.png)

`C:\Users\wise7034\Desktop\workspace\flutterSDK 폴더에 설치.`

### 시스템 환경 변수 설정

`시스템 속성 > 환경 변수 > Path 편집 > 찾아보기 > 설치한 bin파일 추가`

![시스템 환경 변수 설정](https://github.com/kjk7034/FlutterSetup/blob/master/mages/winSetup02.png)

### 설치 확인

`터미널을 열고 flutter --version 확인`

![flutter 버전확인](https://github.com/kjk7034/FlutterSetup/blob/master/mages/winSetup03.png)

### Android 스튜디오 설치

[Android 스튜디오 설치](https://developer.android.com/studio/install)

다운로드 링크를 통해 설치

### Android 스튜디오 실행

Android 스튜디오를 실행

![Import Android Studio Settings From...](https://github.com/kjk7034/FlutterSetup/blob/master/mages/winSetup04.png)

처음 설치하는 것이라면 `Do not Import settings`를 선택하고 `OK`

`Configure > Plugins`를 선택

![선택 화면](https://github.com/kjk7034/FlutterSetup/blob/master/mages/winSetup05.png)

`Marketplace`에서 flutter를 검색하여 install

![Plugins > Flutter 검색](https://github.com/kjk7034/FlutterSetup/blob/master/mages/winSetup06.png)

IDE를 재실행 하면 다음과 같이 Start a new Flutter project를 통해서 시작.

![Android Studio 실행화면](https://github.com/kjk7034/FlutterSetup/blob/master/mages/winSetup07.png)


### 프로젝트 생성

Create New Flutter project에서 Flutter Application을 선택하고 Next

![Create New Flutter project](https://github.com/kjk7034/FlutterSetup/blob/master/mages/winApp01.png)

New Flutter Application에서 다음 항목들을 작성하고 Next

* 프로젝트 이름
* Fluuter SDK 경로 (...을 눌러서 flutter install시 설치한 폴더를 설정)
* 프로젝트 위치
* 설명

![New Flutter Application](https://github.com/kjk7034/FlutterSetup/blob/master/mages/winApp02.png)

Set the package name에서 패키지명과 AndroidX설정. Finish

![Set the package name](https://github.com/kjk7034/FlutterSetup/blob/master/mages/winApp03.png)

### flutter 환경 구성 검사

터미널에 다음 명령어로 확인이 가능

```
flutter doctor
```

실행했더니 `Try re-installing or updating your Android SDK Manager.`가 나왔다.

![flutter doctor 실행결과](https://github.com/kjk7034/FlutterSetup/blob/master/mages/doctor01.png)

`Android Studio > Tools > SDK Manager`를 선택

![SDK Manager 선택](https://github.com/kjk7034/FlutterSetup/blob/master/mages/doctor02.png)

SDK Tools에서 Hide Obsolete Packages를 해제하고 Android SDK Tools (Obsolete)를 체크 하고 Apply

![Android SDK Tools Apply 과정](https://github.com/kjk7034/FlutterSetup/blob/master/mages/doctor03.png)

그리고 다시 flutter doctor를 실행

![flutter doctor 실행결과](https://github.com/kjk7034/FlutterSetup/blob/master/mages/doctor04.png)

경고 문구에 따라 다음을 실행

```
flutter doctor --android-licenses
```

실행 후 다시 flutter doctor를 실행

![flutter doctor 실행결과](https://github.com/kjk7034/FlutterSetup/blob/master/mages/doctor05.png)

### 에뮬레이터 실행

`Tools > AVD Manager`를 선택

![Tools > AVD Manager 선택](https://github.com/kjk7034/FlutterSetup/blob/master/mages/avd01.png)

Your Virtual Devices에서 `+ Create Virtual Device ...` 클릭 후 기본으로 설정되어 있는 `Phone > Pixel 2`를 그대로 선택 후 Next

![Virtual Device 추가 화면](https://github.com/kjk7034/FlutterSetup/blob/master/mages/avd02.png)

System Image에서 `Q Download`를 클릭 후 Install 후 Next

![Q Download Install](https://github.com/kjk7034/FlutterSetup/blob/master/mages/avd03.png)

AVD Name 설정 후 Finish

![AVD Verify Configuration](https://github.com/kjk7034/FlutterSetup/blob/master/mages/avd04.png)

생성된 디바이스를 Launch

![Launch this AVD in the emulator](https://github.com/kjk7034/FlutterSetup/blob/master/mages/avd05.png)

Android Studio에서 `Android SDK built for x86(mobile)`선택 후 main.dart **Run**

![emulator run](https://github.com/kjk7034/FlutterSetup/blob/master/mages/avd05.png)

데모 화면 실행.

![Flutter Demo App](https://github.com/kjk7034/FlutterSetup/blob/master/mages/avd07.png)

## macOS
