# Picture Repository(사진저장소)

TO DO LIST를 작성하며 진행하고 있는 Spring Web 사이드 프로젝트 입니다.

- <b>[TO DO LIST]</b>
- 로그인 화면(login.jsp)
    - [x]  로그인 기능 구현 - 로그인 성공시 home.jsp 로 이동
    - [x]  로그인 실패 후 부가기능 구현 - 로그인 실패시 입력했던 아이디, 비밀번호 남도록 처리
    - [x]  로그인 실패 후 부가기능 구현 - 로그인 실패시 "아이디가 존재하지 않거나 비밀번호가 일치하지 않습니다" 에러 메세지 처리
    - [x]  회원가입 화면 이동 기능 구현 - 회원가입 화면(join.jsp)으로 이동하는 버튼 추가

- 회원가입 화면(join.jsp)
    - [x]  생성에 성공하면 "회원가입이 완료되었습니다." 라는 메세지를 보여주는 joinSuccess.jsp 로 이동
    - [x]  회원가입 기능 구현 - 아이디 생성 기능(아이디, 이메일, 비밀번호, 비밀번호 확인 입력)
    - [x]  비밀번호 재확인 기능 구현 - 비밀번호를 두번 입력하게 하여 일치할 경우에만 생성 아니면 "비밀번호가 일치하지 않습니다." 에러 메시지 표현
    - [x]  로그인 화면 이동 기능 구현 - 로그인 화면으로 이동할 수 있는 버튼 추가
    - [ ]  아이디 중복 체크 구현 - 아이디가 이미 생성된 아이디인 경우 "이미 중복된 아이디입니다." 에러 메세지 표현
    - [ ]  아이디 조합 체크 에러메세지 구현 - 네이버의 회원가입 화면처럼 5~20자의 영문 소문자, 숫자와 특수기호(_),(-)만 사용 가능한 이이디 체크 로직 구현 제대로 됬으면 멋진 아이디네요! 메세지 파란색으로 표현
    - [x]  비동기 에러메세지 처리 구현 - 네이버 회원가입 페이지 처럼 비동기적으로 에러메시지 처리 (예 : 비밀번호와 비밀번호 확인이 일치하지 않은 경우 클릭을 때자마자 바로 "비밀번호가 일치하지 않습니다." 에러메시지 표현

- HOME 화면(home.jsp)
    - [ ]  태그별 사진 검색 기능 구현 - 검색 단어로 입력한 태그를 갖는 사진을 검색한다.
    - [x]  부트스트랩을 이용하여 그럴싸한 검색폼 UI 구현
    - [ ]  사진 게시판 기능 구현
        - [x]  화면에 4 x 4 격자 형태로 16개의 그림을 배치하기
        - [ ]  좋아요 기능 구현
        - [ ]  댓글 기능 구현
    - [ ]  사진 렌더링 기능 구현 - 스크롤을 내리면 아래 공간에 사진이 추가되어 계속 보여진다.
    - [x]  로그인하면 핀터레스트처럼 계정아이디, 로그아웃 버튼이 오른쪽에 표현될 수 있도록 구현

- 회원가입 성공 화면 (joinSuccess.jsp)
    - [x]  로그인 화면 이동버튼 구현

- 사용자 사진 업로드 화면(userPictureUpload.jsp)
    - [x]  사용자가 사진 원본을 resources/images/fulls 경로에 업로드 한다.
    - [x]  사용자가 사진 원본을 업로드하면 resources/images/thumbs 경로에도 사진크기를 줄일 썸네일 사진을 업로드한다.
    - [x]  사용자가 사진을 업로드하면 해당정보를 DB의 userfileinfo에 저장한다.

- 사용자 정보 관리 화면(user.jsp)
