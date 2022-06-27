# 예담 최종프로젝트, '스크린야구 예약 시스템'
### 예담직업전문학교에서 팀 단위로 실시한 최종프로젝트 결과물입니다.
### 저희팀은 '스크린야구 예약 시스템' 이라는 주제로 프로젝트를 만들게 되었습니다.
### 그 중 제가 맡은 역할은, 관리자 페이지에서 전반적인 매장관리 파트를 맡게되었습니다.

```sh
* 근무자 관리
* 매출관리
* TodoList 관리
```

## <span style="color:red">차별점</span>
### 저희는 학원에서 배우기만 한 기술스택이 아닌, 저희 스스로가 학습하여 새로운 기술스택을 활용해보았습니다. 
### 저희는 Spring Boot, thymeLeaf를 활용하여 서비스를 구축하였습니다. 
### 또한 저 개인적으로, 마크다운 이라는 언어를 스스로 공부하여 깃허브 데스크탑과 연동해 포트폴리오를 깃허브에 업로드 했습니다. 



## 사용한 기술스택

> - [Intellij] - IDE
> - [Java 11] - Language
> - [Github] - VCS
> - [Oracle, Oracle Cloud] - DB

### BackEnd
> - [Spring Boot] 
> - [Gradle] 
> - [Spring Secruity] 
> - [mybatis] 


### FrontEnd
> - [HTML, CSS, JS]
> - [jQuery]
> - [BootStrap]
> - [thymeLeaf]

### Collaborate
> - [Jira Software](https://luk2903201-jira.atlassian.net/jira/software/projects/YD/boards/3)


|                  | 수학                        | 평가              |  
|:--- | ---: | :---: |  
| 철수             | 90            | 참잘했어요. |
| 영희           | 50            | 분발하세요. |

# 페이지 소개
## 1. 대시보드
<img src="/images/5_매장관리/대시보드.png" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>

### 매장관리의 대시보드 페이지입니다. 
##### 대시보드 페이지에서는 현재 출근한 근무자의 이름, 남은시간을 계산해주는 차트, 타이머가 표시됩니다.
##### 또한 TodoList의 목록을 표시해줄 수 있으며, 현재 해당 할 일의 상태를 식별할 수 있습니다. 
##### 금일의 매출 부분입니다. 구글차트를 통해 차트를 표현했으며, 현재 차트가 표시되지 않는 이유는 당일날의 매출이 없기 때문입니다. 
##### 주간근무표 입니다. FullCalendar을 통해 월간 근무표를 생성할 수 있으며, 이번주 일요일 - 토요일 까지의 시간이 표시됩니다.

## 2. 근무자 상태관리
<img src="/gifImages/GIF 2022-06-27 오후 3-45-47.gif" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>

### 매장관리의 근무자 현황 페이지입니다.
##### 현재 페이지에선 근무자의 정보와, 지각, 결근, 지급 금액에 관한 정보를 식별할 수 있습니다.
##### 지각은 정해진 근무시간보다 20분 이상 늦게 출근 할 경우 카운트됩니다.
##### 결근은 정해진 근무시간보다 120분 이상 늦게 출근 할 경우 카운트됩니다.
##### 지급 금액은, 현재시간 기준 저번달의 급여를 총 합산하여 계산하여, 도중에 시급이 바뀌어도 예외사항 없이 적용됩니다.
##### 근무자의 상태를 변경할 경우, ajax를 이용하여 비동기방식으로 페이지의 일부분만이 새로고침이 적용됩니다.

## 3. 근무자 출퇴근
<img src="/gifImages/근무자출퇴근.gif" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>

### 매장관리의 근무자 출퇴근 페이지입니다.
##### 근무자의 출퇴근 정보를 기록할 수 있습니다.
##### 출근버튼을 클릭했을 때, 현재시간과 근무표에 기재되어있는 시간을 비교하여 지각, 결근, 정상출근으로 처리합니다.
##### 출근버튼을 누른 후, 대시보드 페이지로 돌아갈 때 기존에 조회되지 않던 근무자의 출근정보가 표시되는것을 식별할 수 있습니다.
##### 다시 출퇴근페이지로 돌아가서, 퇴근버튼을 눌렀을 때 정상적인 퇴근이 아닌 경우 confirm 메시지가 표시됩니다.
##### 정상적으로 퇴근 후, 다시 출근버튼을 클릭했을 때 이미 퇴근한 근무자는 금일 출근할 수 없다는 메시지가 표시됩니다.

## 4. 근무표 생성
<img src="/gifImages/근무표생성.gif" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>

### 근무표 생성 페이지입니다.
##### 비어있는 월의 근무표를 생성하거나, 수정, 삭제할 수 있는 페이지입니다.
##### 근무표를 생성하기 위해서는 1, 2부의 근무자가 같을 수 없으며, 해당 월이 비어있어야 합니다.
##### 근무표를 생성하게되면 해당 날짜의 1, 2부 근무자가 생성됩니다.

## 5. 매출정보 조회
<img src="/gifImages/매출정보 조회.gif" title="px(픽셀) 크기 설정" alt="RubberDuck"></img><br/>

### 매출정보 조회 페이지입니다.
##### 매출정보는 월별, 일별로 조회할 수 있습니다.
##### 조회할 수 있는 매출정보는 총 4가지로, 결제정보 및 총 매출 금액 회원 비회원 매출구분, 요일별 평균 매출량, 온,오프라인 매출구분 입니다.
##### 월정보를 선택할 떄, 이번달을 선택하게 되면 이번달의 오늘까지만 날짜가 선택되어 조회할 수 있습니다.
##### 요일별 평균 매출량은 요일 선택에 관계없이 월선택만 적용됩니다.
