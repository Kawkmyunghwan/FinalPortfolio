# 예담 최종프로젝트, 'BAT-HUB'
### 예담직업전문학교에서 팀 단위로 실시한 최종프로젝트 결과물입니다.
### 저희팀은 '스크린야구 예약 시스템' 이라는 주제로 프로젝트를 만들게 되었습니다.

## <a href="https://youtu.be/wsCW0oRwgWA?t=8195" target="_blank">시연영상 바로 보기 ▶️</a>
## <a href="https://github.com/YOONHEECHEOL/tfprj" target="_blank">전체 프로젝트 바로 보기 ▶️</a>

## 개요
### BAT-HUB란?
* 스크린 야구장에 필요한 서비스를 통합적으로 제공하는 관리 시스템

## 설계의 주안점
1. <b>스프링 시큐리티</b>를 이용한 로그인으로 유저 인증과 권한 검사, 비밀번호 암호화, 보안성 강화
2. <b>Lombok</b>을 이용하여 어노테이션 설정으로 간단하게 VO 객체를 생성하여 코드를 간결화 시켜줌.
3. <b>Google Chart</b>를 이용하여 각 매출에 반영되는 그래프를 가시적으로 표현함.
4. <b>FullCalendar</b> 라이브러리를 이용해 월간 근무표 생성, 수정, 삭제할 수 있는 캘린더를 구현함.
5. <b>AJAX</b>를 통해 페이지 로딩속도 및 클라이언트에게 편리성 제공.
6. <b>BootStrap</b>을 활용한 반응형 페이지 제작 및 Modal 활용.
7. <b>DevTools</b>의 Live Reload 기능 활성화를 통한 생산성 및 개발 효율성 증대.
8. <b>thymeleaf-layout-dialect</b> 라이브러리를 이용해 중복 코드를 최소화.
## Contens
```sh
* 예약
* 매장관리
* 매출관리
* 커뮤니티
* 회원관리
```

## <span style="color:red">차별점</span>
### 저희는 학원에서 배우기만 한 기술스택이 아닌, 저희 스스로가 학습하여 새로운 기술스택을 활용해보았습니다. 
### 이 프로젝트는 Spring Boot, thymeLeaf를 활용하여 서비스를 구축하였습니다. 
### 또한 저 개인적으로, 마크다운 이라는 언어를 스스로 공부하여 깃허브 데스크탑과 연동해 포트폴리오를 깃허브에 업로드 했습니다. 



## 사용기술 및 개발환경

<img src="/stack.png" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>
<hr>

|Category|Detail|
|:---:|:---:|
|OS|Windows 10 pro|
|개발언어|Java(11), Servlet, SpringBoot, Mybatis, HTML5, Javascript, CSS|
|데이터베이스|Oracle Database Express Edition 11g Release 2|
|서버|TOMCAT 9.0|
|IDE|IntelliJ|
|빌드 배포|Gradle, jenkins|
|테스트 툴|Junit|
|프로세스|Intel(R) Core  i7-10700 CPU @ 2.90GHz|
|메모리|16GB RAM|
|보조 기억장치|SSD 250GB|
|형상관리|GitHub|
|협업|[Jira Software](https://luk2903201-jira.atlassian.net/jira/software/projects/YD/boards/3)|

## 프로젝트 기능 구현

<ul>
  <li>근무자 관리</li>
    <ul><li>근무자 상태 조회 및 변경</li></ul>
    <ul><li>근무자 등록 및 수정, 총 근무자 엑셀 다운로드</li></ul>
    <ul><li>현재 출근한 근무자 조회, 주간근무표 조회</li></ul>
    <ul><li>월간 근무표 CRUD </li></ul>
    <ul><li>근무자 출퇴근</li></ul>
  <li>매출관리</li>
    <ul><li>금일 매출 조회</li></ul>
    <ul><li>비회원/회원 매출 조회</li></ul>
    <ul><li>요일별 평균 매출 조회</li></ul>
    <ul><li>온/오프라인 구분 매출 조회</li></ul>
  <li>TodoList 관리</li>
    <ul><li>TodoList CRUD</li></ul>
    <ul><li>할 일의 사진 업로드 및 댓글 CRUD</li></ul>
    <ul><li>체크리스트 체크, 해결, 삭제</li></ul>
</ul>


# 페이지 소개
## 1.1 대시보드
<img src="/images/5_매장관리/대시보드.png" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>

### 매장관리의 대시보드 페이지입니다. 
##### 대시보드 페이지에서는 현재 출근한 근무자의 이름, 남은시간을 계산해주는 차트, 타이머가 표시됩니다.
##### 또한 TodoList의 목록을 표시해줄 수 있으며, 현재 해당 할 일의 상태를 식별할 수 있습니다. 
##### 금일의 매출 부분입니다. 구글차트를 통해 차트를 표현했으며, 현재 차트가 표시되지 않는 이유는 당일날의 매출이 없기 때문입니다. 
##### 주간근무표 입니다. FullCalendar을 통해 월간 근무표를 생성할 수 있으며, 이번주 일요일 - 토요일 까지의 시간이 표시됩니다.

## 1.2 근무자 상태관리
<img src="/gifImages/GIF 2022-06-27 오후 3-45-47.gif" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>

### 매장관리의 근무자 현황 페이지입니다.
##### 현재 페이지에선 근무자의 정보와, 지각, 결근, 지급 금액에 관한 정보를 식별할 수 있습니다.
##### 지각은 정해진 근무시간보다 20분 이상 늦게 출근 할 경우 카운트됩니다.
##### 결근은 정해진 근무시간보다 120분 이상 늦게 출근 할 경우 카운트됩니다.
##### 지급 금액은, 현재시간 기준 저번달의 급여를 총 합산하여 계산하여, 도중에 시급이 바뀌어도 예외사항 없이 적용됩니다.
##### 근무자의 상태를 변경할 경우, ajax를 이용하여 비동기방식으로 페이지의 일부분만이 새로고침이 적용됩니다.

## 1.3 근무자 출퇴근
<img src="/gifImages/근무자출퇴근.gif" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>

### 매장관리의 근무자 출퇴근 페이지입니다.
##### 근무자의 출퇴근 정보를 기록할 수 있습니다.
##### 출근버튼을 클릭했을 때, 현재시간과 근무표에 기재되어있는 시간을 비교하여 지각, 결근, 정상출근으로 처리합니다.
##### 출근버튼을 누른 후, 대시보드 페이지로 돌아갈 때 기존에 조회되지 않던 근무자의 출근정보가 표시되는것을 식별할 수 있습니다.
##### 다시 출퇴근페이지로 돌아가서, 퇴근버튼을 눌렀을 때 정상적인 퇴근이 아닌 경우 confirm 메시지가 표시됩니다.
##### 정상적으로 퇴근 후, 다시 출근버튼을 클릭했을 때 이미 퇴근한 근무자는 금일 출근할 수 없다는 메시지가 표시됩니다.

## 1.4 근무표 생성
<img src="/gifImages/근무표생성.gif" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>

### 근무표 생성 페이지입니다.
##### Full Calendar API를 활용하여 달력을 통해 근무표를 관리할 수 있는 페이지입니다.
##### 비어있는 월의 근무표를 생성하거나, 수정, 삭제할 수 있는 페이지입니다.
##### 생성 버튼을 클릭했을 때, 해당 캘린더의 월 정보를 활용해 일수를 구해 DB에 데이터를 저장하는 방식을 사용했습니다.
##### 근무표를 생성하기 위해서는 1, 2부의 근무자가 같을 수 없으며, 해당 월이 비어있어야 합니다.
##### 근무표를 생성하게되면 해당 날짜의 1, 2부 근무자가 생성됩니다.

## 1.5 매출정보 조회
<img src="/gifImages/매출정보 조회.gif" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>

### 매출정보 조회 페이지입니다.
##### 매출정보는 월별, 일별로 조회할 수 있고, 조회결과는 텍스트 및 구글차트로 표현했습니다.
##### 조회할 수 있는 매출정보는 총 4가지로, 결제정보 및 총 매출 금액 회원 비회원 매출구분, 요일별 평균 매출량, 온,오프라인 매출구분 입니다.
##### 월정보를 선택할 떄, 이번달을 선택하게 되면 이번달의 오늘까지만 날짜가 선택되어 조회할 수 있습니다.
##### 요일별 평균 매출량은 요일 선택에 관계없이 월선택만 적용됩니다.

# 소스코드 소개
## 2.1 출퇴근시간을 계산해서 percent로 보여주는 쿼리

```xml:workerAttendance_mapper.xml

<select id="getPercent" resultType="com.yedam.tfprj.admin.workerAttendance.service.WorkerAttendanceVO">
        SELECT W.WORKER_ID,
               S.ATT_DT,
               W.GOING_TIME,
               QUITTING_TIME,
               TO_DATE(S.IN_TIME, 'YY-MM-DD HH24:MI') AS inMTime,
               S.OUT_TIME,
               ROUND(((current_date - TO_DATE(S.IN_TIME, 'YY-MM-DD HH24:MI')) *24)/((QUITTING_TIME - GOING_TIME) *24),2) * 100  AS percent,
               ROUND((W.QUITTING_TIME - current_date) * 24 * 60 * 60, 2) AS getMTime
        FROM WORKSHEET W, STAFF_ATTENDANCE S
        WHERE W.WORKER_ID = S.WORKER_ID
               AND S.ATT_DT = TO_CHAR(current_date, 'YY-MM-DD')
               AND TO_CHAR(W.GOING_TIME, 'YY-MM-DD') = S.ATT_DT
               AND W.WORKER_ID = #{workerId}
    </select>
```

## 2.2 회원, 비회원의 매출을 구분하여 보여주는 쿼리

```xml:workerAttendance_mapper.xml

<select id="findMemNonMem" resultType="map">
        SELECT CASE WHEN MEMBER_ID = '0' THEN '비회원' ELSE '회원' END AS "member", SUM(PAYMENT_AMOUNT) AS "paymentAmount"
        FROM PAYMENT
        where TO_CHAR(PAYMENT_DATE, 'YYYY-MM-DD') BETWEEN #{firstDate} AND #{lastDate}
        <if test='day != 0'>
            AND TO_CHAR(PAYMENT_DATE, 'D') = #{day}
        </if>
        GROUP BY CASE WHEN MEMBER_ID = '0' THEN '비회원' ELSE '회원' END
    </select>

```

## 2.3 현재 출근한 근무자의 정보를 조회할 수 있는 쿼리

```xml:workerAttendance_mapper.xml
<select id="getNowWorker" resultType="com.yedam.tfprj.admin.workerAttendance.service.WorkerAttendanceVO">
        SELECT A.WORKER_ID,
               A.IN_TIME,
               A.OUT_TIME,
               A.IS_LATE,
               A.IS_ABSENCE,
               I.WORKER_NAME, W.GOING_TIME, W.QUITTING_TIME, A.ATT_DT ,I.POSITION_CD, I.USERTYPE, I.STARTDAY, I.ALLPAY
        FROM STAFF_ATTENDANCE A
                 INNER JOIN STAFF_INFORMATION I
                            ON A.WORKER_ID = I.WORKER_ID
                 INNER JOIN WORKSHEET W
                            ON I.WORKER_ID = W.WORKER_ID
        WHERE TO_CHAR(current_date, 'yy-MM-dd hh24:mi') BETWEEN A.IN_TIME AND TO_CHAR(W.QUITTING_TIME, 'yy-MM-dd hh24:mi')
          AND TO_DATE(A.ATT_DT, 'yy-MM-dd') = TO_DATE(current_date, 'yy-MM-dd')
          AND A.OUT_TIME IS NULL
          and to_char(w.going_time, 'yy-MM-dd') = a.att_dt
    </select>
```




#### 해당 내용은 프로젝트의 일부분을 소개한 것입니다. 포트폴리오를 더 상세하게 조회하고 싶으시면
#### 메인 브랜치의 pdf를 참고 해 주시면 감사하겠습니다.

#### 감사합니다.

