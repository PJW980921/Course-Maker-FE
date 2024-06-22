# ✈ 코스메이커(in.부산광역시)

# 프로젝트 소개

![스크린샷 2024-06-15 오후 3 27 00](https://github.com/PJW980921/Course-Maker-FE/assets/124119421/50a1fe26-659f-4dc3-8326-66e88d95eff3)

코스메이커는 여행객들에게 다양한 테마별 코스를 제공하고, 직접 코스를 등록할 수 있는 서비스입니다.
# 배포 주소
http://api.course-maker.net/
# 설치 가이드
```
1.yarn set version berry
2.yarn install
3.yarn dlx @yarnpkg/sdks vscode
4.yarn dev 이후 http://localhost:5173 접속
```

# 기여 부분
## 코스등록페이지
### Stepper Component 구현

<img width="281" alt="스크린샷 2024-06-10 오후 10 29 58" src="https://github.com/PJW980921/Course-Maker-FE/assets/124119421/7c14fd9a-3e55-48e5-8b81-d84f71d1c968">

 각 단계에서 공통으로 사용되는 상태를 Context로 관리하면, 필요할 때마다 props drilling 없이 쉽게 접근할 수 있어 ContextAPI를 활용했습니다.

 이전,다음 버튼으로 각 Step으로 이동할 수 있어 데이터 지속성을 위해 로컬스토리지를 활용했습니다.

## 코스/여행지 상세페이지

<img width="305" alt="스크린샷 2024-06-22 오후 1 13 34" src="https://github.com/PJW980921/Course-Maker-FE/assets/124119421/56907e07-9c6f-4357-b162-868ebb8465c2">

여행 경로를 쉽게 이해할 수 있는 직관적인 지도 기능을 제공하기 위해 KaKao Maps SDK 라이브러리를 활용했습니다.

데이터 캐싱을 위해 TanstackQuery를 활용했습니다.


