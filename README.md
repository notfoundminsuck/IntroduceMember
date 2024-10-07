# 🎉IntroduceMember🎉
---
## 🛠️  Tools :<img src="https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white"/>, <img src="https://img.shields.io/badge/Visual Studio-5C2D91?style=flat-square&logo=Visual Studio&logoColor=white"/>, <img src="https://img.shields.io/badge/Firebase-DD2C00?style=flat-square&logo=Firebase&logoColor=black"/>, <img src="https://img.shields.io/badge/jQuery-0769AD?style=flat-square&logo=jQuery&logoColor=black"/> 
---
## 😄 Intro
팀원들 소개 홈페이지 
---
## 👨‍💻 Our Role 
- home : 한승완 (Team)
- team : 이창현 (Team, 발표자)
- member : 이유진 (Team)
- member, contactUs : 황상익 (leader)
---
## 👨‍💻 Our Progress 🥅

#### 2024/10/1 
- 4주차까지 강의를 듣고 firebase사용해서 팀원 정보 DB에 저장하는 방식
- MBTI, 취미, 자신이 생각하는 이상적인 개발자?, 팀의 목표(가족같은팀?, 추후 회의를 통해 결정)
- github 주소구성-home, team, members 페이지로 구성-멤버 개인 소개 메뉴
- 멤버 카드 클릭시 멤버 상세정보로 넘어가는 Modal 사용
- Team → css 부분 수정 
- Home → 틀은 git에 올린대로 / css 부분 & 소개글 
- Member → 추가적으로 기능 구현 할 부분 있으면 추가 할 예정
- <a>tag 로 구현 하는 부분은 수요일 구현 예정 
- Home에 대한 네비 바 사용 (10/2)일 마무리 추후 홈 네비바 구현 코드를 갖고 나머지 코드들 추가 할 예정 
- 네비 바 할때 (구글)폰트 맞춰서 적용

#### 2024/10/02
- 팀이름 변경 unranked → 팀이름 선정 이유 : 아직 빛나지 않는(발견되지 않은) 보석이라는 뜻
- 팀이 추구하는 목표, 팀만의 특징 선정, 팀 노션에 개인적으로 생각하는 팀 목표 적기
- 멤버 추가하기 버튼 → 멤버카드 밑 가운데로 옮기는게 미관상 좋을거 같다
- 소개 페이지에 넣을 임시사진 : 찾기
- 최종목표 : 금요일까지 pt완성, 오늘까지 페이지 모두 완성
- Gaol 🥅 : home 페이지 완성, team페이지 완성, 네비바 통일, contect us 추가, member card 오류 수정(멤버카드 생성시 카드 겹치는 것, 상세정보 표기오류), 와이어프레임 수정, ContactUs 수정

#### 2024/10/04
- 발표준비 ppt제작(시연영상찍기)
- Todo : 각자 페이지 만든 기술적인면, 어려웠던 부분 정리해서 슬랙으로 보내기
- ppt 향후 계획 부분 추가(CRUD부분 업그레이드)
- 시연 영상은 월요일 회의 끝난 후 제작

#### 2024/10/07
- 11시까지 제출해야될 자료 : 프로젝트 깃허브 주소, 프로젝트 설명ppt, 시연 영상
---
## 🔊 PT & Video 
- 📢 PT : [[Spring 7기] 17조  .pptx](https://github.com/user-attachments/files/17271519/Spring.7.17.pptx)
- 🎥 Video : https://www.youtube.com/watch?v=wN-fnUDYgW8
---
## 🛠️ 기능 
### - Home 
  - 팀 이름을 선정한 이유, 팀의 소통방식, 팀이 성장하는 방법 게시
  - 부트스트랩의 그리드 시스템을 이용하여 사진과 텍스트 정렬 배치
### - Team 
  - #### About us, Our Goals, ground Rules
  - javascript 의 onclick function과 display block,none visivility visible,hidden 을 이용하여 사진과 글을 열거나 닫을 수 있게 구현
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
### contact us 작성시 어려웠던 점

onsubmit을 html에 구현시 form 태그에서 입력 받은 값을 onsubmit에 넘겨줄 수 있지만 form 태그를 중첩해서 사용해 적용이 안되어 한참 해맸다.
결국 못찾아 addEventListner를 사용해 onsubmit을 사용하지 않고 해결 했다.
event는 변수가 아니라 객체이다. 그렇기 때문에 처음에 잘 모르고 사용했을때 message를 썼다가 alert창이 뜨지 않는 상황이 발생해 찾아보니 event 함수를 써야 된다고 알게 되었고, event.preventDefault()를 통해 폼 제출 시 데이터를 우선 처리하거나 다른 작업을 완료한 후에 폼 제출을 하게끔 만들기 위해 이 기능을 사용했다.
 
<a href>https://velog.io/@ik0605/Event</a> , <a href>https://velog.io/@ik0605/onsubmit-addEventListener</a> 

### addMember를 만들면서 어려웠던점

상세보기 페이지를 사용했을때 고유 id 값을 할당하지 않아 상세보기 페이지가 중복되는 경우가 발생해  let memberId = member.id; 를 따로 처리해 상세보기 모듈 작동시 멤버들의 값이 겹치는 중복 문제를 해결했다.
css 부분에선 card를 한 줄에 4개까지 생성할 수 있도록 설정했지만, 4번쨰 카드가 생성될때 카드가 마지막으로 생성된 카드가 밑으로 내려가는 경우가 발생했다. gap 과 flex-wrap을 원인으로 생각했지만 원인이 아니었고, 원인을 찾지 못해 팀원 분들이 도와주셔서 margin 10px, margin-right = 300px로  값을 주어 해결했다.

--- 
## After Project what we learn 


  
