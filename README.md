# week06

## 오늘 한 일
         지금까지 해온 것 피드백, 디자인 통일을 위한 회의, DB, 서버, 모든 화면 구성 정리
         
### Feedback

         박승준 - 버스 번호 or 정류장 번호를 통해 도착정보를 불러오는 것을 구현하려고 함. 그러나 API연동에 어려움이 있어서 실시간으로 불러오는 것을 실패함 
                  카카오맵 API 연동을 통해 버스 정보를 불러오는 것이 가능할지 알아와보기로 함.

         김다혜 - 셔틀 버스 정보를 스피너를 통해 출발지를 설정하면 시간표가 뜨도록 구현함. 
                  앞으로 현재 시간에 맞게 실시간으로 시간표를 보여주는 부분을 구현해오면 될 것 같음.

         마혜준 - 로그인, 회원가입 layout을 잘 만들어옴. DB연동으로 완성할 예정임.
                  (친구목록 화면을 구성하여 채팅방 추가 버튼을 만들어주면 채팅방 만드는 화면 사람과 이어질 예정)

         박윤빈 - 시간표와 일정을 추가할 수 있는 스케줄표의 layout을 구성중임. 
                  화면 전체에 짜는 것보다 LinearLayout을 통해 화면을 나눠서 추가하는 것이 좋을 것 같다는 피드백을 받음.
                  대면/비대면 투표 부분은 시간표 부분을 완성한 후에 할 예정임. 

         심우정 - firebase 연동에 어려움을 겪음. 지난주에 이어 layout을 잘 만들어옴. 
                  다음주까지 firebase 연동을 하고, DB까지 연동해올 예정임.

         양하은 - 채팅방 추가 화면을 구성해왔으며 친구 추가 부분이 완성되면 연동할 예정임. 졸업학점 계산 부분은 자신의 학과를 선택할 수 있는 spinner를 만들어 놓았으며 
                  학과별 입학년도와 졸업년도를 넣으면 자동으로 졸업이수학점이 불러와지며 자신이 들은 시간을 빼는 형식으로 진행할 예정임.


### 디자인 통일(다음시간까지 바꿔오기)

         기본 배경색: #C695DEFF
         버튼색: 
         글자색: 
         
## DB
#### <회원정보>
         아이디, 비밀번호, 이름, 핸드폰, 학교이메일, 닉네임

#### <과목>
         학수번호, 분반, 전공영역, 강의명, 교수명, 교실, 강의요일, 강의시간, 학점

#### <졸업학점계산기>
         아이디, 학과, 전공영역, 학점 

#### <게시판>
         -작성 
         
         게시판번호, 제목, 내용, 첨부파일, 익명T/F, 닉네임

         -목록
         
         게시판번호, 제목, 내용(글자수제한), 글쓴이(익명), 작성시간, 좋아요 수, 댓글 수

         -보기
         
         게시판번호, 제목, 내용, 첨부파일, 글쓴이, 작성시간, 좋아요 수, 댓글 수

         -댓글
         
         댓글번호, 게시판번호, 내용, 익명T/F

#### <채팅>
         -메세지
         
         메세지ID, 내용, 시간, 아이디, 채팅방ID

         -채팅방 초대
         
         채팅방ID, 채팅방타입, 아이디(초대한사람), 아이디(초대된사람)...
         
#### 택시
         -모집글
         
         출발장소, 도착장소, 탑승시간, 탑승인원

         -채팅
         
#### 버스(api적용 후 db설계 예정)
         
## 다음주까지 할 일
         
         
