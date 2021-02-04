# Picture Repository(사진저장소)

TO DO LIST를 작성하며 진행하고 있는 Spring Web 사이드 프로젝트 입니다.

 - [x] 구현 
 - [ ] 미구현 
 
- <b>[TO DO LIST]</b>
- 로그인 화면
    - [x]  로그인 기능 구현 - 로그인 성공시 home.jsp 로 이동
    - [x]  로그인 실패 후 부가기능 구현 - 로그인 실패시 입력했던 아이디, 비밀번호 남도록 처리
    - [x]  로그인 실패 후 부가기능 구현 - 로그인 실패시 "아이디가 존재하지 않거나 비밀번호가 일치하지 않습니다" 에러 메세지 처리
    - [x]  회원가입 화면 이동 기능 구현 - 회원가입 화면(join.jsp)으로 이동하는 버튼 추가

- 회원가입 화면
    - [x]  생성에 성공하면 "회원가입이 완료되었습니다." 라는 메세지를 보여주는 joinSuccess.jsp 로 이동
    - [x]  회원가입 기능 구현 - 아이디 생성 기능(아이디, 이메일, 비밀번호, 비밀번호 확인 입력)
    - [x]  비밀번호 재확인 기능 구현 - 비밀번호를 두번 입력하게 하여 일치할 경우에만 생성 아니면 "비밀번호가 일치하지 않습니다." 에러 메시지 표현
    - [x]  로그인 화면 이동 기능 구현 - 로그인 화면으로 이동할 수 있는 버튼 추가
    - [x]  아이디 중복 체크 구현 - 아이디가 이미 생성된 아이디인 경우 "이미 중복된 아이디입니다." 에러 메세지 표현
    - [ ]  아이디 조합 체크 에러메세지 구현 - 네이버의 회원가입 화면처럼 5~20자의 영문 소문자, 숫자와 특수기호(_),(-)만 사용 가능한 이이디 체크 로직 구현 제대로 됬으면 멋진 아이디네요! 메세지 파란색으로 표현
    - [x]  비동기 에러메세지 처리 구현 - 네이버 회원가입 페이지 처럼 비동기적으로 에러메시지 처리 (예 : 비밀번호와 비밀번호 확인이 일치하지 않은 경우 클릭을 때자마자 바로 "비밀번호가 일치하지 않습니다." 에러메시지 표현

- HOME 화면
    - [x]  사진 검색 기능 구현 - 검색단어로 사진을 검색하여 게시판에 표현한다.
    - [ ]  태그별 사진 검색 기능 구현 - 검색 단어로 입력한 태그를 갖는 사진을 검색한다.
    - [x]  부트스트랩을 이용하여 그럴싸한 검색폼 UI 구현
    - [ ]  사진 게시판 기능 구현
        - [x]  화면에 4 x 4 격자 형태로 16개의 그림을 배치하기
        - [x]  좋아요 기능 구현
        - [ ]  댓글 기능 구현
    - [ ]  사진 렌더링 기능 구현 - 스크롤을 내리면 아래 공간에 사진이 추가되어 계속 보여진다.
    - [x]  로그인하면 핀터레스트처럼 계정아이디, 로그아웃 버튼이 오른쪽에 표현될 수 있도록 구현
    - [x]  검색데이터가 없을 경우 "검색된 데이터가 없습니다."라는 메세지 중앙에 표현 추가
    - [x]  하단에 네비게이션 페이지 링크 동적 추가 - 검색된 페이지 갯수만큼 동적으로 생성되고 클릭하면 해당페이지로 이동하도록 구현
- 회원가입 성공 화면
    - [x]  로그인 화면 이동버튼 구현

- 사용자 사진 업로드 화면
    - [x]  사용자가 사진 원본을 resources/images/fulls 경로에 업로드 한다.
    - [x]  사용자가 사진 원본을 업로드하면 resources/images/thumbs 경로에도 사진크기를 줄일 썸네일 사진을 업로드한다.
    - [x]  사용자가 사진을 업로드하면 해당정보를 DB의 userfileinfo에 저장한다.
    - [x]  사진 제목, 내용, 태그, 공개범위를 입력 및 지정하고 해당정보를 DB의 userfileinfo에 저장한다.
    - [ ]  파일선택을 눌러 파일들을 선택 후 확인하면 화면상 올라간 파일들의 갯수, 총 크기를 화면 상에 같이 보여준다.
    - [ ]  파일선택은 기본 확장자를 JPEG, GIF, PNG, JPG로 하도록 하고 잘못된 확장자 파일이 올라가면 메세지 띠우고 화면상 올라가 있는 것을 삭제 처리한다.
- 사용자 정보 관리 화면
    - [ ]  사용자의 정보를 수정하여 저장할 수 있도록 한다.
    
- 개선해야할 사항
    - [x]  부트스트랩을 활용하여 사진 업로드 화면 UI 개선
    - [x]  다중으로 파일이 업로드 되도록 개선
    - [x]  상수 값을 .propertes 파일로 따로 관리할 수 있도록 개선
    - [ ]  모바일 환경에서도 홈화면 header부분 UI가 최적화 될 수 있도록 개선 - 크롬처럼 로그인시 오른쪽에 아이디 버튼만 존재하고 클릭시 업로드, 로그아웃 버튼을 포함한 팝업띄우기

- 사용 기술
    - Front-End
      - CSS
      - Javascript 1.7
      - jQuery v2.2.1
      - Bootstrap 4.4.1      
    - Back-End
      - Java 1.8
      - Spring Framework 4.3.12
      - MySQL 5.7.19

- 개발 환경
    - Chrome 88.0.4324.146
    - OpenJDK 1.8
    - Tomcat 8.5

      
