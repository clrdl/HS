# <img src='https://raw.githubusercontent.com/beefed-up-geek/hns_readme_images/main/images/hns.png' width='30px'> H&S BioLab

### H&S는 신장기능 이상 조기진단 키트와 연동한 디지털 헬스케어 서비스입니다.

<br>

## TEAM

| 이름      | 담당 업무                                                           |
| --------- | ------------------------------------------------------------------- |
| 최한송  | **팀장 / 백엔드** : 프로젝트 관리, API 구현, Web Push, 인공지능 학습 |
| 곽태윤    | **백엔드** : API 구현, Flask 서버 구축, 배포, 인공지능 학습         |
| 김지수    | **프론트엔드** : UX/UI, 메인 페이지, 소개 페이지, 마이 페이지, 디자인      |
| 오지훈    | **프론트엔드** : 스케줄러 페이지, 검색 페이지, 디자인                            |
| 황재현    | **프론트엔드** : 스케줄러 페이지, 검색 페이지, 디자인                            |

<br>

## 1. 서비스 소개

### 💡 기획 배경

- 만성콩팥병 환자 수 10년간 2배 이상 증가, 진료비는 2조 3천억 원으로 10년간 1조 원 이상 증가 (전체 진료비 3위)<br>
  📎[관련 기사](https://www.medicaltimes.com/Main/News/NewsView.html?ID=1146111)
  📎[관련 통계자료](https://www.phwr.org/journal/view.html?pn=vol&uid=684&vmd=Full)

- 신장질환은 특이적 증상이 없어 조기 진단이 어려움 <br>

- 만성신장질환 조기 진단을 위한 바이오 마커의 부재<br>

- 신장손상의 유형별/단계별 조기진단을 위한 진단 기술의 부재

<br>

### 🚩 목적 및 필요성

⚒️ **목표**

**H&S BioLab 자가진단키트와 연동**되는 신장질환 관리 서비스
- 만성 신부전증 조기 진단을 위한 바이오 마커 연동
- 신장 손상의 유형별/단계별 조기 진단에 따른 관리 서비스 개발
  
<br>


🔎 **유사 서비스와의 분석**
<div align='center'>
  <img src='https://github.com/beefed-up-geek/hns_readme_images/blob/main/images/KakaoTalk_20240816_140456548.png?raw=true' width='500px'>
</div>

<br>

- 자가진단키트로 몇 가지 항목을 통해 건강 상태 진단 (잠혈, 단백질, 포도당, pH, 케톤 등)
- 맞춤 건강 관리를 위해 많은 정보를 일일이 입력하고, 식사 및 소변량, 수분섭취량 등을 모두 작성해야 함.
- 신장질환 관리 서비스는 존재하지만, 업데이트가 잘 되지 않고 있으며, 자가진단 기능은 부재함.

<br>

✨ **기존 서비스와의 차별화**

- 검사 항목의 이름이 어려워 잘 이해하지 못하는 사용자들을 위해 **네 단계의 위험도**로 현재 상태 가시화. (안전, 주의, 위험, 매우위험)
<div align='center'>
    <img src='https://raw.githubusercontent.com/beefed-up-geek/hns_readme_images/main/images/image.png' width='500px'>
</div>

- 모든 정보를 매일 하나하나 입력할 필요 없이, **궁금한 정보만 검색**하는 건강 관리 서비스 (투석병원 검색, 신기능에 영향을 주는 의약품 검색)
- **건강검진 연동**으로 5초만에 내 건강 상태 파악 가능

<br>

### 🎯 기대 효과


- 가족력이 있거나 관련 질환을 앓고 있는 경우, 자가진단으로 만성콩팥병 예방하여 **사회적 의료 비용 감소**  <br>
- 의학적 지식이 없어도 쉽게 이해할 수 있는 지표로 **의료정보 불균형 해소**
- 간편한 건강관리와 기저질환 파악으로 환자의 **삶의 질 향상**

<br>


<br>

### 🔩 서비스 내용

### 1. 메인 기능

- **신장질환 진단키트와 연동** <br />
  
<div align='center'>
  <img src='https://raw.githubusercontent.com/beefed-up-geek/hns_readme_images/main/images/%ED%82%A4%ED%8A%B8.png' width='300px'>
</div>

  - 소변검사 동영상 가이드 제공

  - 검사 후, 키트 촬영 및 데이터 전송

  - 바이오마커 인식 결과 출력

<br>

### 2. 서브 기능

- **건강검진 데이터 연동 및 분석 서비스**

<div align='center'>
  <img src='https://raw.githubusercontent.com/beefed-up-geek/hns_readme_images/main/images/%EA%B1%B4%EA%B0%95%EA%B2%80%EC%A7%84.png' width='300px'>
</div>

  - 기저질환 파악 및 관리를 위해 국가건강검진 데이터 연동 (CODEF OpenAPI 적용)
    
    - 간편인증 지원으로 빠르고 간단하게 연동
      
    - **신장질환 및 합병증 관련 항목**을 중심으로 그래프 및 분석 제공 & 정상범위 파악

<br>

- **영양 관리 서비스**

  - 신기능 이상 정도 (안전/주의/위험/매우위험)에 따른 영양소 섭취 정보 제공
    
    - 인, 칼륨, 나트륨 등의 영양소 제한량이 있어 식단 계획이 어려운 신장병 환자들을 위한 서비스
  
    - 식약처 영양 DB 활용 (식품이름, 열량, 탄수화물, 단백질, 지방, 나트륨, 칼륨, 인 성분값 사용)

<br>

- **투석 병원 검색 서비스**

<div align='center'>
  <img src='https://raw.githubusercontent.com/beefed-up-geek/hns_readme_images/main/images/%EB%B3%91%EC%9B%90.png' width='300px'>
</div>

  - 환자가 근처 투석병원을 미리 알고 준비할 수 있는 기능
    
    - 신장질환자들이 가장 중요하게 생각하는 건강보험심사평가원의 "혈액투석 적정성 평가" 등급 사용
      
    - 투석병원 등급과 거리, 병원종류에 따른 데이터 필터링
      
    - 그 외에도 다양한 병원 정보 제공

<br>

- **의약품 검색 서비스**

<div align='center'>
  <img src='https://raw.githubusercontent.com/beefed-up-geek/hns_readme_images/main/images/%EC%9D%98%EC%95%BD%ED%92%88.png' width='650px'>
</div>

  - 약물에 의해 발생하는 신장 손상의 비율이 매우 높음 (고령자 및 동반 질환 환자: 30% 이상)
    
  - 따라서, 약물을 섭취하기 전에 신기능에 영향을 주는 성분이 있는지 검색할 수 있는 기능 제공
    
    - 식약처의 다양한 의약품 데이터를 활용해 하나의 통합 DB 구축 (4만개 의약품)

<br>

## 2. 프로젝트 설계

### 🗂 파일 구조도

<details>
<summary>Frontend</summary>

```
📦src
 ┣ 📂components
 ┃ ┣ 📜bottom_navigation.js
 ┃ ┣ 📜bottomtab_design.js
 ┃ ┣ 📜context.js
 ┃ ┗ 📜header.js
 ┣ 📂images
 ┃ ┣ 📂bottm_navigation
 ┃ ┣ 📂health_screen
 ┃ ┣ 📂home
 ┃ ┣ 📂hospital
 ┃ ┣ 📂login
 ┃ ┣ 📂medicine
 ┃ ┣ 📜chevronArrowLeft.png
 ┃ ┣ 📜hns.png
 ┃ ┗ 📜xButton.png
 ┣ 📂screen
 ┃ ┣ 📂Kit_checkup
 ┃ ┃ ┣ 📂assets/images
 ┃ ┃ ┣ 📜Camera.js
 ┃ ┃ ┣ 📜Kit_checkup2.js
 ┃ ┃ ┣ 📜Kit_checkup3.js
 ┃ ┃ ┣ 📜QRcode.js
 ┃ ┃ ┗ 📜index.js
 ┃ ┣ 📂diet
 ┃ ┃ ┗ 📜index.js
 ┃ ┣ 📂healthscreen
 ┃ ┃ ┣ 📂tabs
 ┃ ┃ ┃ ┣ 📜data.js
 ┃ ┃ ┃ ┣ 📜styles_tab.js
 ┃ ┃ ┃ ┣ 📜tab_anemia.js
 ┃ ┃ ┃ ┣ 📜tab_dyslipidemia.js
 ┃ ┃ ┃ ┣ 📜tab_hypertension_diabetes.js
 ┃ ┃ ┃ ┣ 📜tab_kidney.js
 ┃ ┃ ┃ ┗ 📜tab_liver.js
 ┃ ┃ ┣ 📜authentication1.js
 ┃ ┃ ┣ 📜authentication1.js
 ┃ ┃ ┣ 📜authentication3.js
 ┃ ┃ ┣ 📜index.js
 ┃ ┃ ┗ 📜legal_conset_text.js
 ┃ ┣ 📂home
 ┃ ┃ ┗ 📜index.js
 ┃ ┣ 📂hospital
 ┃ ┃ ┣ 📜index.js
 ┃ ┃ ┗ 📜styles.js
 ┃ ┣ 📂kit
 ┃ ┃ ┣ 📂assets/images
 ┃ ┃ ┗ 📜index.js
 ┃ ┣ 📂login
 ┃ ┃ ┣ 📜firebaseConfig.js
 ┃ ┃ ┣ 📜get_kidney_info.js
 ┃ ┃ ┣ 📜get_usr_info.js
 ┃ ┃ ┣ 📜index.js
 ┃ ┃ ┗ 📜login.js
 ┃ ┣ 📂medicine
 ┃ ┃ ┣ 📂assets/images
 ┃ ┃ ┣ 📜index.js
 ┃ ┃ ┗ 📜searchResult.js
 ┃ ┣ 📂src
 ┃ ┃ ┗ 📜index.js
 ┃ ┗ 📜theme.js
 ┣ 📜App.js
 ┣ 📜index.js
 ┗ 📜package.json
```

</details>

<details>
<summary>Backend</summary>

```
┣ 📦config
┃   ┣ 📜database.js
┣ 📦elasticsearch
┃   ┣ 📂hospital
┃   ┃   ┣ 📜byungwon_hospital.py
┃   ┃   ┣ 📜jonghap_hospital.py
┃   ┃   ┣ 📜sangjonghap_hospital.py
┃   ┃   ┣ 📜uione_hospital.py
┃   ┃   ┗ 📜yoyang_hospital.py
┃   ┗ 📂medicine
┃       ┗ 📜medicine.py
┣ 📦routes
┃   ┣ 📜health_checkup.js
┃   ┣ 📜kit.js
┃   ┣ 📜medicine.js
┃   ┗ 📜hospital.js
┗ 📜server.js
```

</details>

<br>

### ⚙️ 아키텍쳐

### 1. 전체적인 구조도

<br>

🔔 **Database**

- Redis : **Refresh Token**을 저장하기 위해 사용
- MySQL : Cloud 서버에서 이용하기 위해 Oracle 인스턴스를 **DB 전용 서버**로 구축

🔔 **AI**

- Sklearn : 요청시 학습한 결괏값을 flask 웹 서비스에 반환
- Flask : 결괏값을 **WSGI 서버**인 gunicorn에 전달
- gunicorn : front에 응답

<div align='center'>
  <img src='https://user-images.githubusercontent.com/97580782/177033692-1fc80c04-5c8a-48d1-b76f-25eb52b5f5b4.png' width='800px'>
</div>

<br>

### 2. Docker-Compose 구조

🔔 **Push 서버 분리**

- 서비스 간의 의존도를 낮추기 위해 기존의 Node 서버와 **Push 전송 서버**를 분리

<div align='center'>
  <img src='https://user-images.githubusercontent.com/97580782/179144069-cc3dcfe8-c2dd-44a8-9eea-beec2f4ec045.png' width='450px'>
</div>

<br>

### ☁️ ER Diagram

- ERD Cloud

📎[ERD 보러가기](https://www.erdcloud.com/d/xx8qkkurmF37XyweN)

<div align='center'>
  <img src='https://user-images.githubusercontent.com/97580782/179144557-7c8f4df5-e24d-4b18-b5a1-8b99229fe361.png' width='450px'>
</div>

<br>

### 📜 API Docs

📎[Swagger API 보러가기](https://kdt-ai4-team17.elicecoding.com/api/swagger/)

<br>

### 🤖 인공지능 모델

- 데이터셋 수집

  1. 식품의약품안전처에서 제공하는 OpenAPI로 데이터셋을 수집 <br>
     📎[공공데이터 활용](http://www.foodsafetykorea.go.kr/api/openApiInfo.do?menu_grp=MENU_GRP31&menu_no=661&show_cnt=10&start_idx=1&svc_no=C003)
  2. 단종, 개편된 영양제 데이터셋들을 방지하기 위해 “최종수정일시” 컬럼이 **2년 이내**(2021년부터)인 데이터만 사용

  3. **네이버 검색 쇼핑 API**를 사용해 영양제 구매 링크, 이미지 썸네일 컬럼 추가 <br>
     📎[네이버 search API](https://developers.naver.com/docs/serviceapi/search/shopping/shopping.md#%EC%87%BC%ED%95%91)

<br>

- **데이터셋 전처리**

  1. 하나의 컬럼이라도 null인 값 제거

  2. 특수문자 제거 (한글, 숫자, 영어 빼고 모두 삭제)

  3. **OKT**를 사용하여 “주된기능성” 컬럼의 형태소 분석 수행, 의미 없는 한국어 불용어 제거 <br>
     📎[open-korean-text](https://github.com/open-korean-text/open-korean-text)

<br>

- 인공지능 모델 학습 및 테스트

  1. Sklearn의 tfidfvectorizer를 사용해 전처리 한 데이터들의 가중치(tf)를 부여 <br>
     📎[sklearn.feature_extraction.text.TfidfVectorizer](https://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.TfidfVectorizer.html)

  2. 사용자에게 문장을 입력 받으면 전처리 단계의 2, 3번을 진행 후 저장된 가중치를 이용해서 “주된기능성” 컬럼과의 **유사도 산정**

  3. 유사도가 **가장 높은 순**으로 3개의 영양제 index 응답

  - 만약 같은 유사도를 가진 영양제들이 3개 이상이면 그 중에 랜덤하게 응답

<br>

- **응답 정확도 개선**

  1. 인공지능 모델 학습만으로 모든 단어를 포괄할 수 없어 QA를 수행하며 부족한 부분은 **룰을 추가**

```
  🪄 여자 → 여성, 생리 → 월경, 변비 → 배변 등
```

<br>

### ⚙️ 기술 스택

- Front-end

  - `React`, `TypeScript`, `axios`
  - `Recoil`, `daisyUI`, `Styled components`

- Back-end

  - `Node.js`, `TypeScript`
  - `Flask`, `Python`
  - `Redis`, `MySQL - Sequelize`

- AI

  - `Sklearn - tfidfvectorizer`

- Deployment

- `Docker`, `Docker-compose`, `Nginx`, `gunicorn`, `Certbot - LetsEncrypt`

<br>

## 3. 시연 영상

![시연영상](https://user-images.githubusercontent.com/97580782/191692840-d946beaf-33c9-4b24-92fb-360943c5dc8d.mp4)

<div align='center'>
  <img src='https://user-images.githubusercontent.com/97580782/191693588-f9157b27-17f8-43e4-a65d-a023f1ba5954.gif' width='450px'>
</div>
1. 첫 번째 시연 영상 1분 30초에 나오는 큐알 코드로 모바일에서 구독
2. 스케줄에 등록한 시간에 웹, 앱 모두 푸시 알람
