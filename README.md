# 🤝 팀 프로젝트
#### KREAM 👟 
한정판을 거래하는 가장 확실한 방법. 럭키드로우, 발매정보, 패션트렌드도 이제 KREAM(크림)!

## 📌 프로젝트 개요
#### 프로젝트 기간
- 2022년 06월 09일(목) ~ 2022년 07월 22일(금)

#### 프로젝트 목표
- 브랜치 전략으로 Git Flow 적극 활용!
- 주어진 API 요구사항대로 기능 구현 하되, 전체적인 디자인은 KREAM 사이트 클론하기!

#### 배포 주소
KREAM

<br />

## 🙋🏻 팀원 소개

<img width="500" alt="team4" src="https://velog.velcdn.com/images/yejine2/post/f4cb6600-6e0b-46de-ab14-c82a6f560aae/image.png">


| [양예진](https://github.com/yejine2)       | [신재일](https://github.com/ShinJaeIl01)               | [김민구](https://github.com/kimmgu)                | [박선홍](https://github.com/Mangrove-Sun)                                             
| --------------------------------------------------- | ------------------------------------------- | ------------------------------------------------- | ------------------------------------------------- 
| 로그인 / 회원가입 / 메인 페이지  | 사용자 파트(제품 검색 및 구매관리) | 관리자 파트(제품, 판매 관리) | 계좌 파트 / 사용자 정보 수정 |
 

<br />

## 프로젝트 내용

### ⭐️ 주요 기능

 #### 로그인 / 회원가입

<img width="800" alt="auth" src="https://user-images.githubusercontent.com/85099612/180381065-5cc9287d-ae6c-43e7-8b18-d6324f62a883.png">

 - 로그인 및 회원가입 시 이메일 및 비밀번호 형식이 맞는지 실시간으로 유효성 검사를 합니다.
 - 유효성 검사에 통과하지 못하면 로그인 / 가입 버튼이 비활성화 됩니다.
 - 로그인이 된 사용자라면 로그인 페이지에 접근이 불가하도록 설정했습니다.
  
  #### 인증

  - 로그인이 필요한 페이지에 접속 시 인증 확인을 거칩니다.
  - 로그인이 안 된 사용자 ➡️ 로그인 페이지로 이동
  - 마이페이지 - 사용자 아이디 로그인 ➡️ 사용자 페이지로 이동 / 관리자 아이디 로그인 ➡️ 관리자 페이지로 이동


<br />

 #### 검색 및 사용자 제품 구매

<img width="800" alt="serch" src="https://user-images.githubusercontent.com/85099612/180413942-a66a5cf4-cc86-410b-8552-1c646154e3d8.png">

#### 헤더 섹션 검색
- 검색어를 로컬스토리지에서 스토어로 전달합니다.
- 최근 검색어를 로컬스토리에서 가져옵니다.

#### 검색 필터
- 상단 카테고리, 필터 분류와 현재 검색된 필터 연동을 합니다.
- 필터 카테고리, 브랜드, 가격으로 검색합니다.

#### 제품 구매
- 로그인 상태, 계좌 유무, 잔액으로 구매 가능여부 판단합니다.
- 비로그인으로 구매 시도하면 로그인페이지로 유도하는 문구가 뜹니다.
- 연결된 계좌가 없을 경우에 계좌조회 링크로 유도되도록 합니다.
- 잔액 부족하거나 다른 계좌문제로 구매가 안될때 계좌 확인 요청 창이 뜹니다.
  
<br />

#### 사용자 정보 수정 및 계좌 관리

<img width="800" alt="account" src="https://user-images.githubusercontent.com/85099612/180416804-03a19ea9-8c95-4f07-a9e1-1cfd4732fa9f.png">

#### 사용자 이미지, 이름, 비밀번호 수정
- 사용자가 이미지를 선택하면 Base64 인코딩하여 전송합니다.
- 사용자 이름 및 비밀번호 수정 시 형식 실시간 유효성 검사를 합니다.
- 유효성 검사 통과했을 경우에 저장 버튼 활성화 됩니다.

#### 계좌 등록 및 해지
- 각 은행 정보에 맞게 계좌 자릿수 실시간 유효성 검사를 합니다.
- 입력 폼(계좌번호, 전화번호, 서명) 전부 유효성 검사 통과했을 경우에 등록 버튼 활성화 됩니다.

#### 구매 내역
- 구매 내역이 '전체', '확정 대기', '구매 확정', '구매 취소' 탭으로 필터링 되도록 했습니다.


<br />

#### 관리자 파트
<img width="800" alt="admin" src="https://user-images.githubusercontent.com/85099612/180399750-0abdfd7c-a97f-477a-98d1-e2b68f11476b.png">



#### 제품 추가
- 관리자 페이지 및 전체 제품 조회 페이지에 아이콘으로 구현했습니다.
- 제품가격 입력 시 천 단위마다 쉼표를 표시하여 가독성 높였습니다.
- 이미지 파일(썸네일, 상세 사진)은 Base64를 구현하여 어떤 이미지 파일이든지 등록 가능합니다.

#### 제품 수정
- 전체 제품 조회 페이지에서 하나씩 수정이 가능하도록 구현했습니다.
- 재고 유무를 토글 버튼으로 만들어서 손쉽게 재고 관리를 할 수 있도록 구현했습니다.
- 매진 여부를 자유롭게 설정 또는 해제 할 수 있도록 구현했습니다.

#### 제품 삭제
- 전체 제품 조회 페이지에서 단 한번의 클릭으로 간편하고 신속하게 삭제가 가능하게끔 구현했습니다.

#### 단일 제품 상세 조회
- 등록된 제품의 썸네일을 클릭하면 제품 상세 조회 페이지가 나오게끔 구현했습니다.
- 예약 정보(reservation)는 추가하지 않았습니다.


<br />

### 🛠 기술 스택
- Front 
  - Vue.js
  - Vite
  - Pinia
  - SCSS
  - Bootstrap
  - Eslint

<br />

### 🌳 설계도


<img width="800" alt="User flow" src="https://velog.velcdn.com/images/yejine2/post/51e77242-9821-4dd6-b77f-de42657b03ee/image.jpg">


- [User Flow](https://app.diagrams.net/#G1CvW9kHXPxmw40lganlLvndA0Nr9bjmlQ)


<br />

## 팀 프로젝트를 진행하며...
#### 양예진
- 다들 팀 프로젝트는 처음이라서 우여곡절이 많았던 것 같습니다. 어찌 되었든 결국 완성해준 4조 분들 감사합니다!👍🏻
- git flow 전략을 프로젝트에 도입해서 사용하니 git과 친해졌습니다. 다음 프로젝트에서도 자신 있게 git flow 전략을 사용할 수 있을 것 같습니다.
- 로그인 / 회원가입에 유효성 검사를 도입하면서 Vue의 흐름에 다시 한번 공부할 수 있는 계기가 되었습니다.
- 아쉬움이 남은 부분도 있지만 여러모로 이번 프로젝트에서 많이 배웠고, 다음 프로젝트에서는 커밋 메시지 컨벤션 설정 등 디테일하게 정하면서 진행해보고 싶습니다!

#### 신재일
- 팀프로젝트를 통해서 역할분담을 하고 git-flow를 활용해보니 개발자 팀 협업에 대해 적응이 되었습니다.
- 이번 프로젝트는 구조에 대해 더 집중했고 데이터 흐름에 많은 신경을 써가며 작업했습니다.
- 많은 데이터를 하나로 묶어서 코드를 정리하며 작업 했는데 그러다보니 배열 메서드 활용에 대해 많은 공부가 됐습니다.
- 부족했던 점은 조건문과 for문을 남발한 기분이 들어서 아직 부족함이 많이 느껴지는 부분입니다.

#### 김민구
- 항상 혼자서만 프로젝트를 구현을 하다가 이번에 처음으로 여러명에서 팀을 이루어서 프로젝트를 하게 되었는데 색다르고 좋은 경험을 했던거 같습니다.
- 첫째로 대부분의 기업에서 사용하는 git-flow를 사용하면서 여러가지 문제점도 많이 있었지만 팀원들과 함께 의논하고 토론하면서 해결하는 과정에서 많은것을 익히고 배웠고 완벽하게는 아니지만 어느정도 깃 플로우를 다룰 수 있게 되었습니다.
- 둘째로 구매 판매 API를 도입하면서 구입을 누르면 판매내역 페이지에서 표시가 되고 반대로 판매내역 쪽에서 구매 취소를 누르면 구매가 취소 되는 기능들을 구현해 보면서 팀원들과의 커뮤니케이션의 중요성을 깨닫게 되었습니다.
- 마지막으로 더 구현해보고 싶은 기능들이 많이 있었는데 마음속으로나 생각으로만 구현을 하고 실제 프로젝트에는 적용을 하지 못해 아쉬운점이 있었습니다. 예를들어 관리자 페이지 메인에 있는 막대표 같은 경우 색깔도 입히고 한눈에 판매내역을 확인하기 좋게 구현하고 싶었는데 막상 마지막날까지 데이터 연결도 못하는 그냥 가짜표가 된 상태로 제출하는게 너무 아쉬웠습니다. 또한 구매를 하거나 판매를 하거나 편집을 하거나 삭제를 하거나 할 때 사용자(판매자)의 편의성을 높이기 위해서 다시 한번 묻거나 확실히 등록이 되었다는 것을 알려주는 모달창을 구현을 하고 싶었는데 패키지만 설치하고 고민만 하다가 결국 구현을 하지 못한 점이 정말 아쉽습니다.

#### 박선홍
- 처음으로 진행해본 팀 프로젝트를 통해 동료들과의 의사소통이 얼마나 필요하고 또 얼마나 중요한지에 대해 알 수 있었다.
- 현업에서도 많이 쓰이는 git-flow 또한 사용해보면서 실수도 많이 있었지만 팀원들과 의논하며 해결하는 과정에서 많은 것을 배웠다.
- 이번 프로젝트로 인해 vue사용에 조금은 익숙해진 느낌입니다.
