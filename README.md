# Picture Repository(사진저장소)

TO DO LIST를 작성하며 진행하고 있는 Spring Web 사이드 프로젝트 입니다.
 
## 프로젝트 목표

- 이미지 포스팅, 공유 소설 네트워크인 핀터레스트를 벤치마킹하여 사진저장소 플랫폼 [Picture Repository] 구현
- 모바일에서도 문제없이 동작하는 반응형 웹서비스 구현
- 비동기 통신 웹서비스 구현

## **TO DO LIST**

- [로그인 화면]
    - [x]  로그인 기능 구현 - 로그인 성공시 [HOME 화면]으로 이동
    - [x]  로그인 실패 후 부가기능 구현 - 로그인 실패시 입력했던 아이디, 비밀번호 남도록 처리
    - [x]  로그인 실패 후 부가기능 구현 - 로그인 실패시 "아이디가 존재하지 않거나 비밀번호가 일치하지 않습니다" 빨간색 에러 메세지 처리
    - [x]  회원가입 화면 이동 기능 구현 - [회원가입 화면]으로 이동하는 버튼 추가
- [회원가입 화면]
    - [x]  생성에 성공하면 [화원가입 완료 화면] 으로 이동
    - [x]  회원가입 기능 구현 - 아이디 생성 기능(아이디, 이메일, 비밀번호, 비밀번호 확인 입력)
    - [x]  비밀번호 재확인 기능 구현 - 비밀번호를 두번 입력하게 하여 일치할 경우에만 생성 아니면 "비밀번호가 일치하지 않습니다." 에러 메시지 표현
    - [x]  [로그인 화면] 이동 기능 구현 - [로그인 화면]으로 이동할 수 있는 버튼 추가
    - [x]  아이디 중복 체크 구현 - 아이디가 이미 생성된 아이디인 경우 "이미 중복된 아이디입니다." 에러 메세지 표현
    - [ ]  아이디 조합 체크 에러메세지 구현 - 네이버의 회원가입 화면처럼 5~20자의 영문 소문자, 숫자와 특수기호(_),(-)만 사용 가능한 이이디 체크 로직 구현 제대로 됬으면 "멋진 아이디네요!" 메세지 파란색으로 표현
    - [x]  비동기 에러메세지 처리 구현 - 네이버 회원가입 페이지 처럼 비동기적으로 에러메시지 처리 (예 : 비밀번호와 비밀번호 확인이 일치하지 않은 경우 입력란을 옮기자 마자 바로 "비밀번호가 일치하지 않습니다." 에러메시지 표현
- [회원가입 완료 화면]
    - [x]  "회원가입에 성공하셨습니다!" 라는 메세지를 보여줌.
    - [x]  [로그인 화면]으로 이동할 수 있도록 "로그인 하러 가기"버튼 추가
- [HOME 화면]
    - [x]  사진 검색 기능 구현 - 검색단어로 사진을 검색하여 게시판에 표현한다.
    - [x]  부트스트랩을 이용하여 검색폼 UI 구현
    - [x]  사진 게시판 기능 구현
        - [x]  화면에 4 x 4 격자 형태로 16개의 그림을 배치하기
        - [x]  좋아요 기능 구현 (비동기적으로 구현)
        - [x]  조회된 사진이 16개 이상일 경우 하단 네비게이션 바를 페이지 별로 생성하여 이후, 이전 페이지 사진을 조회 가능하도록 구현
    - [x]  로그인하면 핀터레스트처럼 계정아이디, 로그아웃 버튼이 오른쪽에 표현될 수 있도록 구현
    - [x]  검색데이터가 없을 경우 "검색된 데이터가 없습니다."라는 메세지 중앙에 표현 추가
    - [x]  하단에 네비게이션 페이지 링크 동적 추가 - 검색된 페이지 갯수만큼 동적으로 생성되고 클릭하면 해당페이지로 이동하도록 구현
    - [ ]  태그별 사진 검색 기능 구현 - 검색 단어로 입력한 태그를 갖는 사진을 검색한다.
- [회원가입 성공 화면]
    - [x]  로그인 화면 이동버튼 구현
- [사용자 사진 업로드 화면]
    - [x]  사용자가 사진 원본을 resources/images/fulls 경로에 업로드 한다.
    - [x]  사용자가 사진 원본을 업로드하면 resources/images/thumbs 경로에도 사진크기를 줄일 썸네일 사진을 업로드한다.
    - [x]  사용자가 사진을 업로드하면 해당정보를 DB의 userfileinfo에 저장한다.
    - [x]  사진 제목, 내용, 태그, 공개범위를 입력 및 지정하고 해당정보를 DB의 userfileinfo에 저장한다.
    - [x]  파일선택을 눌러 파일들을 선택 후 확인하면 화면상 올라간 파일들의 갯수, 총 크기를 화면 상에 같이 보여준다.
    - [x]  파일선택은 기본 확장자를 JPEG, GIF, PNG, JPG로 하도록 하고 잘못된 확장자 파일이 올라가면 메세지 띠우고 화면상 올라가 있는 것을 삭제 처리한다.
    - [x]  최대 용량을 초과할 경우 '최대 업로드 용량을 초과했습니다.'메세지 표현 후 화면상 올라가 있는 것을 삭제 처리한다.
- [사용자 사진 조회 화면]
    - [ ]  [HOME 화면]에서 사진을 조회하여 사진 클릭시 사진 원본과 업로드 화면에서 입력한 정보들을 표현한다.
    - [ ]  이 화면에서도 좋아요를 누를 수 있도록 구현
    - [ ]  총 좋아요 갯수를 표시 - 좋아요를 누를 때도 새로 반영되도록 비동기적으로 구현
    - [ ]  다른 로그인 사용자가 사진 아래에 댓글을 입력할 수 있도록 한다.
- [사용자 정보 관리 화면]
    - [ ]  사용자의 정보를 수정하여 저장할 수 있도록 한다. (비밀번호 변경등)

## 기능개선 / 버그수정 / 리팩토링 REPORT

- [x]  부트스트랩을 활용하여 사진 업로드 화면 UI 개선
- [x]  다중으로 파일이 업로드 되도록 개선
- [x]  상수 값을 .propertes 파일로 따로 관리할 수 있도록 개선
- [x]  파일 업로드 후 이동한 페이지에서 새로고침하면 다시 업로드 되는 현상 발견 > redirect 방식으로 이동하여 해결
- [x]  javascript에서 빈 값의 EL 표현식 에러 개선
- [x]  모바일 환경에서도 홈화면 header부분 UI가 최적화 될 수 있도록 개선 - 반응형 네비게이션 바로 변경
- [ ]  사진 렌더링 기능 구현 - 스크롤을 내리면 아래 공간에 사진이 추가되어 계속 보여지도록 구현
- [ ]  비효율적으로 동작하고 있는 검색 기능 개선 - 페이징 처리, 인덱스 재구성

## **사용 기술**

- [Front-End]
    - CSS3
    - HTML5
    - Javascript ES6
    - jQuery 2.2.1
    - Bootstrap 4.4.1
- [Back-End]
    - Java 1.8
    - Spring Framework 4.3.12
    - MySQL 5.7.19

## **도입 예정 기술**

- REST API
- AWS

## **개발 환경**

- OpenJDK 1.8
- Tomcat 8.5
- Maven

      
