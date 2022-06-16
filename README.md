# (주)나인커뮤니케이션 프론트엔드 면접 사전 테스트
자격증넷 사이트 클론코딩하기(https://janet.co.kr/)
<img width="1287" alt="main" src="https://user-images.githubusercontent.com/69252064/174094746-76d82973-678a-432a-9634-07dc6ec6da25.png">


## 구현한 기능
### 1. 상단 고정바(스크롤 이벤트)
### 2. 가이드버튼에 마우스 올리면 색 전환
### 3. 광고슬라이드 자동재생 (미완)
### 4. 광고배너 슬라이드 - 화살표 클릭 시 다음 배너
### 5. HOT키워드TOP20에 마우스 올리면 추가정보 보이기

## 해야할 것
1. 화면 줄일때 hot title 가리는 부분 수정하기
2. Guide 파트에 광고슬라이드 구현



##코드
/page
  /HomeWrapper - 홈화면의 전체적인 틀
  /Home - 홈화면 코드의 집합
/components
  /Ads - 작은사이즈의 광고배터 파트
  /Guide - 광고/정보/인기순위 파트
  /Header
    /FixedHeader - 스크롤이벤트시에 발생하는 고정헤더 파트
    /HeaderGuide - /*고정헤더에서의 재사용을 위하여 컴포넌트별로 나누어서 구현*/
      /Burger - 드롭다운 컨텐츠를 위한 햄버거바 이미지
      /GuideBar - Top100/자격증정보 등의 파트로 이동을 위한 가이드 파트
      /GuideTown - 우리동네학원/커뮤니티 등의 파트로 이동을 위한 가이드 파트
    /HeaderSearch - 통합검색을 하는 파트
    /UserService - 회원가입/로그인 등 사용자서비스를 위한 파트
    
 /data
   /image - 페이지 구현을 위한 이미지들을 저장
   /top20 - 과제에서 주어진 top20의 정보들을 저장
