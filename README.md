# 44-2nd-Dream-backend 경매 플랫폼 제작 프로젝트

<img src=https://user-images.githubusercontent.com/121158293/236659809-3ff8df57-9fe3-4515-93da-a2581b72d309.png width="280" height="65">

<br/>

## 프론트앤드
김영운([**Github**](https://github.com/), [회고록]())<br/>
조건호([**Github**](https://github.com/), [회고록]())<br/>
최선영([**Github**](https://github.com/suny0ung), [회고록](https://note-ballpen.tistory.com/24))<br/>

<br/>

## 백앤드
박세익([**Github**](https://github.com/), [회고록](https://walwaldev.tistory.com/))<br/>
장다희([**Github**](https://github.com/walwald), [회고록](https://walwaldev.tistory.com/))<br/>
김민서([**Github**](https://github.com/), [회고록](https://walwaldev.tistory.com/))<br/>
송석준([**Github**](https://github.com/), [회고록](https://walwaldev.tistory.com/))<br/>

<br/>

## 📍프로젝트 기간 & 인원
* 프로젝트 기간: 2주 (2023.04.20 ~ 2023.05.04)   
* 개발 인원:  
  `Frontend`: 최선영(Product Manager), 김영운, 조건호 <br/>
  `Backend`: 박세익(Project Manager), 장다희, 김민서, 송석준 <br/>
* [백엔드 Github 저장소](https://github.com/wecode-bootcamp-korea/44-2nd-Dream-backend)
* 모델링한 사이트: [KREAM](https://kream.co.kr/)
<br/>

## 📍사용 기술

* FrontEnd   

 |React|JavaScript|styledcomponents|Rest|Prettier|
|---|---|---|---|---|
|<div style="display: flex; align-items: flex-start;"><img src="https://techstack-generator.vercel.app/react-icon.svg" alt="icon" width="52" height="52" /></div>| <div style="display: flex; align-items: flex-start;"><img src="https://techstack-generator.vercel.app/js-icon.svg" alt="icon" width="65" height="65" /></div>| <div style="display: flex; align-items: flex-start;"><img src="https://img.shields.io/badge/styledcomponents-DB7093?style=for-the-badge&logo=styledcomponents&logoColor=white"> </div>|<div style="display: flex; align-items: flex-start;"><img src="https://techstack-generator.vercel.app/restapi-icon.svg" alt="icon" width="65" height="65" /></div>|<div style="display: flex; align-items: flex-start;"><img src="https://techstack-generator.vercel.app/prettier-icon.svg" alt="icon" width="65" height="65" /></div>|<div style="display: flex; align-items: flex-start;"><img src="https://techstack-generator.vercel.app/docker-icon.svg" alt="icon" width="65" height="65" /></div>|<div style="display: flex; align-items: flex-start;"><img src="https://techstack-generator.vercel.app/aws-icon.svg" alt="icon" width="65" height="65" /></div>|
<br/>



</div>

* 협업 <br/>
<div style="display: flex; align-items: flex-start;">
<img src="https://img.shields.io/badge/github-181717?style=for-the-badge&logo=github&logoColor=white">
<img src="https://img.shields.io/badge/trello-0055cc?style=for-the-badge&logo=trello&logoColor=yellow">
<img src="https://img.shields.io/badge/slack-4A154B?style=for-the-badge&logo=Slack&logoColor=wihte">
<img src="https://img.shields.io/badge/notion-000000?style=for-the-badge&logo=notion&logoColor=white">
<br/>
<br/>


 ## flow
 
 <img width="500" alt="스크린샷 2023-05-07 오후 6 17 45" src="https://user-images.githubusercontent.com/121158293/236668841-92202a4a-31ab-4610-bf53-4c8b0d5229ca.png">


 ## 구현 페이지 (메인페이지, 제품나열)
  
### - 메인페이지
 
<br/> 
 
<!-- ### - Search -->
  

https://github.com/suny0ung/44-2nd-Dream-frontend/assets/121158293/4413b61f-3e2d-4c63-b2e1-44b400b5fa6f
  

 **상품 검색 :**
    <br/>
    debounce 커스텀 훅 컴포넌트를 정의하였고, 해당 훅을 사용하여 검색 컴포넌트에서 input 검색 단어 작성이 완료 되었을때 fetch API를 받아오게 구현하여 불필요한 API 사용을 줄였습니다.<br/>
    제품명, 카테고리명으로 검색이 가능하게  Fatch API를 통해 백엔드와 통신하여 해당 제품들을 모달창으로 보여주었습니다. <br/>
    modal의 boolean을 이용, 검색의 모달창과 input 검색 단어의 모달창을 구현하였고, <br/>
    input 검색 단어의 모달창을 구현할때 useRef를 사용하여 바깥 영역을 클릭하면 모달창이 꺼지게 설정하였습니다.
<!--   useDebounce 컴포넌트 훅을 정의하여, 검색창에 검색할 단어가 완성되어야 백앤드와 통신이 가능하게 구현, 불필요한 통신 횟수를 줄임. -->
 <br/>
  
 **인기상품 검색 :** 
   <br/>
   Fatch API를 통해 백엔드와 통신하여, 검색어 데이터를 역대 검색량 순으로 정렬 상위 10개의 검색어를 map 함수를 통해 보여주었습니다.
  
<br/>
  
### - 제품나열 페이지
  
https://github.com/suny0ung/44-2nd-Dream-frontend/assets/121158293/c9a427f2-0dd2-4100-bc71-4d2a65e22ea4
 

**다중필터 :**
  <br/>
  오른쪽 드롭박스 & 왼쪽 카테고리의 선택값에 따라 fetch로 받아온 필터링된 데이터를 map으로 나열되게 구현하였습니다.

<br/>

**무한스크롤 :**
  <br/>
  보여지는 화면의 최상단의 값과 화면의 보여지는 값의 합이 해당 실제 페이지의 영역보다 커지면 offset값에 추가로 보여질 아이템 값을 더해서 쿼리스트링과 Fatch함수를 통해 리랜더링되어 나열되는 상품의 수가 늘어나게 구현하혔습니다.
  </br>
  
<!--   <details>
  <summary> 토글기능 </summary>
  <div markdown="1">
    **작성한 글 보기**
  </div>
  </details> -->
