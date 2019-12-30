<h1>TIS 인트라넷 페이지 개발 프로젝트</h1>

<h4>01. 프로젝트 개요</h4>
<div>
<h6>가. 주제 선정</h6>
GUI구현부터 DB운용까지 효과적으로 학습하며 설계할 수 있다고 생각되는 가상의 기업체 내 인트라넷 웹페이지를 개발 모델로 선정

<h6>나. 프로젝트 목표</h6>
<pre>
1. 로그인부터 페이지 내 메뉴 사용까지 사원DB정보를 기반으로 페이지 운용
2. 카드 레이아웃을 이용하여 페이지 전환시 새 창이 아닌 패널 전환으로 페이지 구성
3. DB안의 자료를 이용하여 자유로운 입출력이 가능한 게시판 구현
4. 사원의 쪽지함을 개별 DB로 설계하여 각각의 쪽지함 구현
</pre>

<h6>다. 개발 도구</h6>
<pre>
- 사용 언어: java, sql
- 제작 환경: Intel(R) Core(TM) i5-4590 / CPU @ 3.30GHz 3.30GHz
            Oracle Database 11g Express Edition  11.2.0.2.0
            Oracle JDK 1.8.0_231
            Eclipse 2019-09 IDE
            NetBeans IDE 8.2 (Build 201609300101)
</pre>

<h6>라. 팀원 및 파트 분배</h6>
<pre>
- 공통작업
  DB설계: 각 담당 파트별 테이블 작성
  GUI구현
- 김용수(팀장)
  로그인 기능 구현
  쪽지함 기능 구현 : 쪽지목록, 보내기, 받기
- 김원미
  GUI디자인 초안 구현
  공지사항 게시판 구현 : 글목록, 글작성, 글수정, 글삭제
- 박지훈
  한 줄 게시판 구현 : 원글작성, 댓글작성, 수정, 삭제
- 조아영
  로그인 기능 구현
  관리자모드 구현 : 사원목록, 입사-퇴사자 관리, 사원정보 수정
</pre>

<h6>마. 제작 기간</h6>
2019년 11월 27일 ~ 2019 12월 6일(약 10일)
</div>

<hr>

<h4>02. 프로젝트 설계</h4>
<div><pre>
<h6>가. 데이터베이스 모델링(논리적, 물리적)</h6>
총 8개 테이블로 구성
<img src="https://github.com/w086286/TisIntraNet/blob/master/images/db1.png" width="90%">
<img src="https://github.com/w086286/TisIntraNet/blob/master/images/db2.png" width="90%">

<h6>나. UI 스토리보드</h6>
<img src="https://github.com/w086286/TisIntraNet/blob/master/images/ui.png" width="90%">
</pre></div>

<hr>

<h4>03. 프로젝트 결과</h4>
<pre><div>
<h6>가. 로그인</h6>
<img src="https://github.com/w086286/TisIntraNet/blob/master/images/01%20login.png" width="90%">
사번과 비밀번호 입력후 로그인 버튼 클릭시 메인화면 진입
- 관리자의 경우   : 공지사항 등록 및 수정, 삭제 권한 / 관리자 모드 진입 및 입사자 등록, 수정, 삭제 권한
- 일반 사원의 경우: 공지사항 등록 및 수정, 삭제 / 관리자모드 진입 외 모든 권한

<h6>공지사항</h6>
<img src="https://github.com/w086286/TisIntraNet/blob/master/images/02%20notice_.png" width="90%">
로그인 후 진입시 첫 메인 화면
<img src="https://github.com/w086286/TisIntraNet/blob/master/images/03%20notice_write.png" width="90%">
공지사항 글쓰기: 관리자에 한함
<img src="https://github.com/w086286/TisIntraNet/blob/master/images/04%20notice_writeConfirm.png" width="90%">
글쓰기 유효성 검사: 제목 및 본문글이 공백일 경우 에러 메세지 출력
<img src="https://github.com/w086286/TisIntraNet/blob/master/images/05%20notice_write_result.png" width="90%">
글쓰기 성공 결과
<img src="https://github.com/w086286/TisIntraNet/blob/master/images/06%20notice_read.png" width="90%">
공지사항 읽기
<img src="https://github.com/w086286/TisIntraNet/blob/master/images/07%20notice_edit.png" width="90%">
공지사항 읽기 화면 하단의 수정버튼 클릭시 수정 화면 전환: 관리자에 한함
<img src="https://github.com/w086286/TisIntraNet/blob/master/images/08%20notice_del.png" width="90%">
공지사항 읽기 화면 하단의 삭제버튼 클릭시 삭제: 관리자에 한함

<h6>한 줄 게시판<h6>
<img src="https://github.com/w086286/TisIntraNet/blob/master/images/09%20board_main.png" width="90%">
좌측 메뉴 패널의 "한 줄 게시판" 라벨 클릭시 진입
<img src="https://github.com/w086286/TisIntraNet/blob/master/images/16%20board_write.png" width="90%">
상단 텍스트필드에 원글 내용 작성
<img src="https://github.com/w086286/TisIntraNet/blob/master/images/17%20board_writeConfirm.png" width="90%">
등록 버튼 클릭시 확인 메세지 박스 출력
<img src="https://github.com/w086286/TisIntraNet/blob/master/images/18%20board_write_result.png" width="90%">
원글 작성 결과
<img src="https://github.com/w086286/TisIntraNet/blob/master/images/10%20board_reply_write.png" width="90%">
댓글을 작성할 대상 원글 클릭 후 좌측 하단 답글 버튼 클릭, 댓글 작성
<img src="https://github.com/w086286/TisIntraNet/blob/master/images/11%20board_reply_result.png" width="90%">
댓글 작성 결과
<img src="https://github.com/w086286/TisIntraNet/blob/master/images/14%20board_searchResult.png" width="90%">
게시글 검색 결과
<img src="https://github.com/w086286/TisIntraNet/blob/master/images/12%20board_del.png" width="90%">
삭제 대상 게시글 클릭 후 게시글 삭제 버튼 클릭시 확인 메세지 박스 출력
<img src="https://github.com/w086286/TisIntraNet/blob/master/images/13%20board_del_result.png" width="90%">
삭제 결과: 원글 이하의 댓글까지 연쇄적으로 삭제 처리
            
<h6>관리자 모드</h6>
<img src="https://github.com/w086286/TisIntraNet/blob/master/images/19%20admin.png" width="90%">
좌측 메뉴 패널의 "관리자 모드" 라벨 클릭시 진입: 관리자에 한하여 접근 가능
<img src="https://github.com/w086286/TisIntraNet/blob/master/images/20%20admin_reg.png" width="90%">
중앙 하단의 추가 버튼 클릭시 입사자 등록
<img src="https://github.com/w086286/TisIntraNet/blob/master/images/21%20admin_edit.png" width="90%">
중앙 하단의 변경 버튼 클릭시 기존 사원 정보 수정
<img src="https://github.com/w086286/TisIntraNet/blob/master/images/22%20admin_del.png" width="90%">
중앙 하단의 삭제 버튼 클릭시 기존 사원 정보 삭제
<img src="https://github.com/w086286/TisIntraNet/blob/master/images/23%20msg.png" width="90%">
우측 상단의 쪽지함 버튼 클릭시 개인쪽지함이 열림
<img src="https://github.com/w086286/TisIntraNet/blob/master/images/24%20msg_read.png" width="90%">
쪽지를 선택하고 내용보기 버튼 클릭시 쪽지 읽기창
<img src="https://github.com/w086286/TisIntraNet/blob/master/images/25%20msg_sendTab.png" width="90%">
보낸쪽지함 탭을 누르면 보낸쪽지함 창으로 전환
<img src="https://github.com/w086286/TisIntraNet/blob/master/images/26%20msg_write.png" width="90%">
쪽지보내기 버튼을 누르면 쪽지보내기 창으로 천환
<img src="https://github.com/w086286/TisIntraNet/blob/master/images/27%20msg_write_result.png" width="90%">
답장 버튼 누르면 쪽지 전송
<img src="https://github.com/w086286/TisIntraNet/blob/master/images/28%20logout.png" width="90%">
우측 상단의 로그아웃 버튼이나 윈도우 창끄기 버튼을 누를시 로그아웃 확인

</pre></div>

이상입니다
