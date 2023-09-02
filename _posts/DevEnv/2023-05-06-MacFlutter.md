---
title:  "[Flutter] Mac M1에 설치하는 법"
excerpt: "Flutter를 Mac M1에 설치하는 방법을 알아보자."

categories:
  - DevEnv
tags:
  - [Flutter, Macbook, M1 Silicon, Xcode, Android Studio, cocoapods]

toc: true
toc_sticky: true

date: 2023-05-06
last_modified_at: 2023-05-06
---

## Xcode 설치 및 호환성
![](https://velog.velcdn.com/images/sungmyeonggi/post/ef84ea60-349b-47af-8ec9-04b9d0899b5d/image.png)
- [Flutter Document](https://docs.flutter.dev/get-started/install/macos)
- Xcode 설치
- Terminal 입력

```
$ sudo softwareupdate --install-rosetta --agree-to-license
```

## Flutter SDK 설치
![](https://velog.velcdn.com/images/sungmyeonggi/post/c066500f-3cbe-4cea-a2a4-76e907b55b43/image.png)
- flutter_macos_arm64_3.7.xx-stable.zip 설치
- 설치 파일은 HOME에 압축 풀기

## Sublime Text 설치
![](https://velog.velcdn.com/images/sungmyeonggi/post/708b6020-d48a-4b15-be5c-f1abcb49dd78/image.png)
- [Sublime Text URL](https://www.sublimetext.com/)

## 환경변수 설정
![](https://velog.velcdn.com/images/sungmyeonggi/post/8d636b92-1ef6-4dd0-ae7e-b0978daebf46/image.png)![](https://velog.velcdn.com/images/sungmyeonggi/post/e73d9a02-b176-4590-b263-06fb279bdab1/image.png)

- 이 부분을 Sublime Text에 복붙
```
export PATH="$PATH:$HOME/flutter/bin"
```
- 사진과 같이 저장, HOME(PC ID)

## Android Studoio 설치
- [풍혜림님 Velog 참조](https://velog.io/@poonghr/Android-Studio-M1-Mac%EC%97%90-Android-Studio-%EC%84%A4%EC%B9%98%ED%95%98%EA%B8%B0)

> More Actions 클릭 ⏭️ SDK Manager 클릭 ⏭️ SDK Tool 클릭 ⏭️ 
Android SDK Command-line Tools 클릭 ⏭️ Apply ⏭️ 설치 완료

- 설치 완료후 Terminal에 아래의 텍스트 입력
```
>> flutter doctor --android-licenses
```

## cocoapods 설치
- [Youngwoo Jeon님 Velog 참조](https://velog.io/@jyw3927/macOS-macOS%EC%97%90-cocoapods-%EC%84%A4%EC%B9%98%ED%95%98%EA%B8%B0)

🚨 혹시 Youngwoo Jeon님 Velog 참조하고 brew까지 설치해서 했는데도 cocoapods가 설치가 안된다면???
> vi ~/.zshrc로 들어가서
export PATH=/opt/homebrew/bin:$PATH를 추가
ESC누르고 :wq로 탈출 

## 모든 것이 잘 설치됐는지 확인
![](https://velog.velcdn.com/images/sungmyeonggi/post/8ba061ca-dee4-496c-9278-24bc906fcdab/image.png)

***
<br>

🌜 개인 공부 기록용 블로그입니다. 오류나 틀린 부분이 있을 경우 
언제든지 댓글 혹은 메일로 지적해주시면 감사하겠습니다! 😄

[맨 위로 이동하기](#){: .btn .btn--primary }{: .align-right}