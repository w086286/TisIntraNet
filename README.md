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

<h6>다. 시연</h6>
로그인
<img src="https://github.com/w086286/TisIntraNet/blob/master/images/01%20login.png" width="90%">
공지사항(로그인 후 진입시 메인화면)


<img src="" width="90%">
<img src="" width="90%">
<img src="" width="90%">
<img src="" width="90%">
<img src="" width="90%">
<img src="" width="90%">
<img src="" width="90%">
<img src="" width="90%">
<img src="" width="90%">
<img src="" width="90%">
<img src="" width="90%">
<img src="" width="90%">
<img src="" width="90%">
<img src="" width="90%">
<img src="" width="90%">
<img src="" width="90%">
<img src="" width="90%">
<img src="" width="90%">
<img src="" width="90%">
<img src="" width="90%">
<img src="" width="90%">
<img src="" width="90%">
<img src="" width="90%">
<img src="" width="90%">
<img src="" width="90%">
<img src="" width="90%">
<img src="" width="90%">
<img src="" width="90%">
<img src="" width="90%">
<img src="" width="90%">
<img src="" width="90%">
<img src="" width="90%">
<img src="" width="90%">
<img src="" width="90%">
<img src="" width="90%">
<img src="" width="90%">
<img src="" width="90%">
<img src="" width="90%">
<img src="" width="90%">
</pre></div>
