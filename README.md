# 🎉IntroduceMember🎉
---
## 🛠️  Tools :<img src="https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white"/>, <img src="https://img.shields.io/badge/Visual Studio-5C2D91?style=flat-square&logo=Visual Studio&logoColor=white"/>, <img src="https://img.shields.io/badge/Firebase-DD2C00?style=flat-square&logo=Firebase&logoColor=black"/>, <img src="https://img.shields.io/badge/jQuery-0769AD?style=flat-square&logo=jQuery&logoColor=black"/> 

---
## Intro
팀원들 소개 홈페이지 
---
## 🛠️ 기능 
### - Home 
  - 팀 이름의 의미, Grow up 
### - Team 
  - About us, Our Goals, ground Rules
### - Member 
  ##### Modal 기능을 활용해 create와 card 클릭시 해당 정보가 나타날 수 있도록 함
  - Create : fireabase db와 연동해 member 생성시 addDocs를 통해 db에 값이 넘어오고, getDocs를 통해 MemberCard 값 나타날 수 있도록 구현
             생성이 완료 되면, 해당 alert를 통해 사용자가 확인 할 수 있도록 형성 
  - Card : 팀원에 대한 정보 등록 및 확인 가능
### - Contact us 
  - email, 이름, 휴대폰 번호와 궁금한 사항을 입력해 FireBase로 넘어올 수 있게 설정 
  - 개인정보이기 때문에 db를 가져오는 부분은 따로 구현 하지 않음 
--- 
## 🥵 TroubleShooting 
1. contactus를 firebase와 연결하는 과정 중에, bootstarp version 4, 5가 Header 부분에 동시에 존재해 이부분 수정 
2. onsubmit 이벤트를 HTML에 직접 호출할때 event 적용 되지 않음. + alert 문제 또한 발생 
-> 폼 제출 이벤트를 직접 등록 
-> onsubmit을 사용하지 않고 JavaScript에서 DOM 로드 후 이벤트 처리 하도록 변경 
+a) DOM - document object Model (웹 브라우저가 HTML 페이지를 인식하는 방식) 


  
