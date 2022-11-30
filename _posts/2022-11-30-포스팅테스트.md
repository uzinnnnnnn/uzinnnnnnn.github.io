---
title: "Google Analytics로 방문자 통계하기"
last_modified_at: 2022-11-30
categories:
  - Github Blog
comments: true
---

사람들이 내 블로그에 얼마나 방문했을까?
Google Analytics를 적용하여 알아보자

## ✨ Google Analytics?✨
> 구글에서 제공하는 웹로그 분석 도구 무료이다!


## Google Analytics 시작하기
###### *이 글은 minimal mistakes 테마 기준으로 작성하였습니다*
1. [Google Analytice](https://www.markdownguide.org/basic-syntax/) 에 접속하여 **회원가입** 또는 **로그인**을 해준다. 

2. 계정 설정 페이지가 나오면 '새 계정 이름'을 넣고 **다음**을 누른다.

3. 속성 이름 -> github 블로그 주소 등록

     보고 시간대 -> 대한민국

     통화 -> 대한민국


## 블로그에 사용할 ID 찾기
1. 왼쪽 가장 하단에 있는 `관리`탭으로 간다.
2. `데이터 스트림`을 찾아 들어간 후 **Github Blog** 주소를 찾아 들어간다.
3. **웹 스트림 세부정보** 페이지에서 `측정 ID` 복사!


## `_config.yml` 파일 수정하기

```
# Analytics
analytics:
  provider               : "google-gtag"
  google:
    tracking_id          : "G-ESG92JFC0S" 
    anonymize_ip         : # true, false (default)
```
* `tracking_id`에 복사한 `측정 ID` 넣기 

## Aanlytics 테스트 해보기
Google Analytics에 재접속하면 방문자 통계 확인 가능!
