# WinBaramMacro

Login Macro

10/21 Github 처음 커밋완료.
 1. Git ignore 사용법 숙지 및 사용
 2. 

10/22 
1. stringParser Judge 부분 개선 진행 예정.  - 보류
 - sendkey할때 (,),[,], 등 해당 문자일 경우 안됨
 - 특수키 추가 예정 ( key down up 등.. )

2. Command 수행하는 부분 시간에 따라 반복 진행할 수 있는 부분 추가 예정. - 보류
 - Time간격, 반복진행 시작,멈춤 키 추가할 예정

3. Json Save or Load할때 데이터 없을경우 처리부분 안정화 예정. 
 - Command부분 수정. - 10/22 완료
 - ID 부분 Group 부분 미입력시 0으로 입력되도록 수정 - 해당부분 Cross Error 해결 필요.

4. Refresh 부분 업데이트 예정 - 보류
 - 현재는 Process만 켜져있으면 로그인으로 인식
  a. Process 존재하는지 확인.
  b. ID부분 비교하여 켜져있는지 확인.
  c. Reconnet Leave 창 떠있는지 확인.
  -> 위 순서대로 로그인 확인 예정
  + b, c에 해당될 경우 순서대로 진행하도록 하는 기능까지 구현 예정.
  
5. 명령어 (이전 명령어 수행한 아이디가 같을경우 Delay 줄것임. 10/22 완

6. 토로라비 고구려 대기중 -> 부여 이동시 문제 발생  - 10/22 완
 - 부여일경우 귀환 전 비영사천문 추가.

10/23
+ 로그인 이미지 crop 할경우 버그 수정
 : 생성자 static 으로 재설정하여 List Size Add 되도록 수정.
+ 토로라비 이동 개선
 : sendkey {enter}로 대체

1. Json Save or Load할때 데이터 없을경우 처리부분 안정화 예정. 
 - ID 부분 Group 부분 미입력시 0으로 입력되도록 수정 - 해당부분 Cross Error 처리.
 - Register에 마지막에 호출된 파일경로 저장하여 이후에 프로그램 실행시 해당경로로 불러와지도록 수정. - 완료
 - 현재 오픈된 파일 UI구현 - 완료

2. Refresh 부분 업데이트 예정
 - 현재는 Process만 켜져있으면 로그인으로 인식
  a. Process 존재하는지 확인.
  b. ID부분 비교하여 켜져있는지 확인.
  c. Reconnet Leave 창 떠있는지 확인.
  -> 위 순서대로 로그인 확인 예정
  + b, c에 해당될 경우 순서대로 진행하도록 하는 기능까지 구현 예정.
  
 + string 보간 적용 - 완료.
 + 프로그램 실행 후 로그인하면 명령수행의 연결ID 제대로 등록되지 않는 부분 수정. - 완료

10/25
 1. 명령어수행 Dialog 부분 새로고침 추가 ( 로그인추가OR 해제 시 껏다키는것 귀찮 )
  -명령어수행 Dialog 한개만 뜨도록 코드수정. - 완료.
  -Refresh부분 개선 ( 로그인 상태 변화 있을 경우에만 Table refresh) - 완료.
  
 2. 아이디 로그인 비밀번호 틀렸을 경우 재시도 과정 추가 (1번시도) 
  -> esc -> esc ->enter 후 다시시도. 완료
  
10/26
 1. Process Capture 후 Form생성, 해당 Form 에 출력해준 후 좌표 찾는 기능 추가 - 완료
 2. 연결됨 연결안됨 확인 시 Process 가 winbaram인지 체크하는 부분 추가. - 완료

10/30
 1. 명령어 반복수행 기능 추가. -완료
 2. 멀티로그인 개선 - 추후개선
  a. Sleep 시간 최소화 하는 방향으로 개선

11/4 진행예정 ( 현재시간 11/3 )
 10/30 코드 진행.
 1. 원하는 Process 띄운후 마우스 위치 좌표 출력하는 기능 공용화 할수 있도록 구현.
 2. ...
 
11/9
 1. Thread 종료 안정화
 2. 명령어 반복실행 일시중지 코드 추가
 3. winbaram 실행 후 위치 0,0으로 이동 
