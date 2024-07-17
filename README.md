
# 📱shop-techmya
 1인 크리에이터들을 위한 최고의 모바일 액세서리 Shop!!

# TECHMYA-CAT 팀원 및 GitHub
  👦🏻 [송재혁](https://github.com/speter6501)
  👦🏻 [장준영](https://github.com/finite2030)
  👦🏻 [이창민](https://github.com/l2chmnl)
  👧🏻 [연주현](https://github.com/DISNOTACAT)
  
  
### 📋프로젝트 소개
* 개발기간 : 2024.06.25 - 2024.06.28 (4일)
* 최근 수요가 급격히 증가하고 있는 1인 크리에이터에게 필요한 방송 주변 장비 및 액세서리를 판매하는 온라인 쇼핑몰과 관리자 페이지
  

### 프로젝트 스터디 목표
- 쇼핑몰 관리 프로세스 이해 증진
- 협업 및 커뮤니케이션 능력 강화
- 실제 환경에서의 적용 가능성 탐색
- 학습 및 개인 발전


### 📈주요 목적
1. 재고 관리 최적화: 가시적인 재고 관리로 인한 업무 난이도 하향으로 인한 효율적인 재고관리로 비용 절감.
2. 주문 및 상품 관리: 상품의 등록, 수정과 주문 처리 등 통합적인 기능 수행.
3. 게시판 관리: 주요 공지사항 및 FAQ, 1:1 문의를 통한 고객 관리 용이.
   

### 🛠️주요 기능
1. 회원관리
   - 회원 정보 조회
   - 회원 계정 생성
2. 게시판 관리
   - FAQ 게시판
     - 게시글 조회
       - 전체 조회
       - 상세 조회
     - 게시글 등록
   - 공지사항 및 문의 게시판
     - 게시글 조회
       - 전체 조회
       - 상세 조회
     - 게시글 등록
3. 상품 관리
   - 상품 등록
   - 상품 조회
   - 상품 판매글 조회
   - 상품 판매글 등록
   - 상품 판매용 이미지 보여주기
4. 재고 관리
   - 재고 조회
     - 이름 조회
     - 전체 조회
   - 입고 전체 조회
   - 출고 전체 조회
5. 주문 관리
   - 주문 조회
     - 전체 조회
     - 회원명 조회
     - 주문 상세 조회
  


### 🐬데이터베이스 구성
[ERDcloud](https://www.notion.so/coffit23/ERD-dd0a633005d84a369d7bb7646868bebb?pvs=4#53c223cd509d4feea2e045b7cdb040eb)

### 📂메뉴 구조도
![DBSTRUCTOR](https://github.com/l2chmnl/shop-techmya/assets/162394517/ee47120f-514d-4f27-ab00-c00687a082a1)


### 📊기대효과
- 상품/재고 관리 효율성 향상 : 주문과 재고를 실시간으로 관리하여 서류와 현장의 차이를 최소화 할 수 있다.
- 시간과 장소의 제약 최소화 : 대면 및 방문 없이 전반적인 관리가 가능하여 제약을 최소화 하여 고객 만족을 높인다.
- 운영 피드백 용이 : 고객 및 업무 프로세스 또한 온라인 비대면으로 피드백을 주고 받을 수 있어 다양한 장단점 파악이 가능하다.


## 📑상세 다이어그램 및 기획 문서 노션
  🔗[테크먀-켓 노션]([https://www.notion.so/coffit23/3-3355ABC-c26bbee54bbf44fd86fc559fd41e5981?pvs=4](https://www.notion.so/coffit23/1-TECHMYA-CAT-5952080481e34f45b226e3aed24d8055))
* [ERD](https://www.notion.so/coffit23/ERD-dd0a633005d84a369d7bb7646868bebb)
* [TEST CASE](https://www.notion.so/coffit23/TEST-CASE-794dbaf902654990aa8641309e937833)

* * *

## 🧑‍💻팀원 구성
1. 송재혁
2. 장준영
3. 연주현
4. 이창민
5. ~~육슬찬~~

## ⚙️ 개발 환경
* devtool : IntelliJ IDEA 2024.1.3 (Ultimate Edition)
* JAVA JDK: Temurin version '17.0.10'
* MySQL-connector-j : 8.0.33
* Mybatis : 3.5.6
* Build Tool : gradle
* Version Control : Git
* Communicate : Slack
* Collaboration Tool : Figma, Github, Notion, ERDCLOUD

## 🩻프로젝트 구조
```
  java  
  │  └─com  
  │      └─ohgiraffers  
  │          └─techmya  
  │              ├─admin  
  │              │  ├─common  
  │              │  │  └─paging  
  │              │  ├─order  
  │              │  │  ├─controller  
  │              │  │  └─model  
  │              │  │      ├─dao  
  │              │  │      ├─dto  
  │              │  │      └─service  
  │              │  ├─product  
  │              │  │  ├─controller  
  │              │  │  └─model  
  │              │  │      ├─dao  
  │              │  │      ├─dto  
  │              │  │      └─service  
  │              │  └─stock  
  │              │      ├─controller  
  │              │      └─model  
  │              │          ├─dao  
  │              │          ├─dto  
  │              │          └─service  
  │              ├─board  
  │              │  ├─controller  
  │              │  └─model  
  │              │      ├─dao  
  │              │      ├─dto  
  │              │      └─service  
  │              ├─configuration  
  │              ├─member  
  │              │  ├─controller  
  │              │  └─model  
  │              │      ├─dao  
  │              │      ├─dto  
  │              │      └─service  
  │              └─shop  
  │                  └─order  
  │                      ├─controller  
  │                      └─model  
  │                          ├─dao  
  │                          ├─dto  
  │                          └─service  
  └─resources  
      ├─mappers  
      │  ├─adminOrder  
      │  ├─product  
      │  ├─shopOrder  
      │  └─stock  
      ├─static  
      │  ├─admin  
      │  │  └─assets  
      │  │      ├─css  
      │  │      ├─img  
      │  │      │  ├─avatars  
      │  │      │  ├─backgrounds  
      │  │      │  ├─elements  
      │  │      │  ├─icons  
      │  │      │  │  ├─brands  
      │  │      │  │  └─unicons  
      │  │      │  ├─illustrations  
      │  │      │  ├─layouts  
      │  │      │  └─logo  
      │  │      ├─js  
      │  │      └─vendor  
      │  │          ├─css  
      │  │          │  └─pages  
      │  │          ├─fonts  
      │  │          │  └─boxicons  
      │  │          ├─js  
      │  │          └─libs  
      │  │              ├─apex-charts  
      │  │              ├─highlight  
      │  │              ├─jquery  
      │  │              ├─masonry  
      │  │              ├─perfect-scrollbar  
      │  │              └─popper  
      │  └─shop  
      │      ├─assets  
      │      │  ├─css  
      │      │  ├─images  
      │      │  └─js  
      │      └─order-assets  
      │          └─products-assets  
      │              ├─css  
      │              ├─img  
      │              ├─js  
      │              └─webfonts  
      └─templates  
          ├─admin  
          │  ├─board  
          │  ├─order  
          │  ├─product  
          │  └─stock  
         ├─common  
          │  ├─admin  
          │  │  └─layouts  
          │  └─shop  
          │      ├─fragments  
          │      └─layouts  
          ├─member  
          └─shop  
```


## 역할 분담 🐯🐶🐷🐭👻

#### 송재혁
* 회원관리
* 게시판

#### 장준영
* 상품관리

#### 연주현
* 주문관리

#### 이창민
* 재고관리

#### ~~육슬찬~~
* 치어리더

## 📕 프로젝트 후기

#### 송재혁
* 선택과 집중이 필요했던거 같다
다음에는 내 능력 안에서 하되 너무 스스로 부담을 주진 말자는 마인드로 해야겠다는 생각이 강했다 기능구현 못한 부분이 조금 많았고 데이터 흐름에 대한 이해도가 필요할 거 같다. html자체가 이해하기 조금 어려운 경우도 있었고 단지 db랑 콘솔을 연결하는 작업이라고 생각해서 쉬울줄 알았지만 페이지 연결과 꾸미는 것도 어려웠다.  파이널때는 준비를 잘해서 기능을 제대로 구현해보고 싶고 이번을 계기로 디테일 부분에서 기르는 게 필요할 거 같다. 

#### 장준영
* HTML에서 전달받은 데이터를 조건에 맞게 제어하는 게 어려웠다. 사용자가 직접 사용하는 것이기에 예외 사항을 고려하는 부분과 사용하기 쉽게 만들고 싶었는데 기능 구현에서 막힌 부분이 있어 아쉬웠다.

#### 연주현
* 프론트 설계와 함께 진행하며 부족한 프로세스 개념을 많이 느꼈다. 서버와이 관계도와 데이터의 흐름을 더 이해할 필요가 있을거같다. 팀 프로젝트를 진행하며 시간과 역할 분배의 중요성을 다시한번 느꼈다. 부족했던 부분은 이후 연습과 함께 천천히 채워가고 싶다.

#### 이창민
* 첫 미니프로젝트에는 java 콘솔과 DB만을 이용한 프로젝트였다. 걱정했던 것 보다 수월하게 진행했었는데, 그 때문인지 이번엔 단지 html과 연동만 추가된 것 뿐이라고 가볍게 생각했었다. 단지 html이 추가된 것 뿐인데 작업 진행 속도가 엄청나게 느려졌다. 시작도 전에 자만했던 내 자신에 대해 반성하게 되었다. 실시간으로 서버에 연동한 것도 아닌 로컬에 한 것 뿐이지만, 고려해야할 점이 너무 많았다. html, css를 모두 이용하고 싶었지만 html만 사용해서 기능을 구현해 아쉬웠다. 프로젝트도 준비했던 기능을 모두 구현하지 못해서 아쉽다. 파이널 프로젝트에는 발전한 모습을 보여주고 싶어서 부족한 부분들을 연습해야겠다.




<hr>

