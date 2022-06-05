# 오픈소스SW개론 과제2_컴퓨터공학과 20200128 노슬기
## 리눅스 명령어 top, ps, jobs, kill
 1. top
 * 현재 os 상태를 나타내주는 CLI 어플리케이션임
 * 시스템 현재 시간, 유저,로드 애버리지, 메모리 사용량, CPU 사용량 등 시스템의 상태를 실시간으로 파악할 수 있음
 
 |명령어|설명|
 |:---:|:---:|
 |shift + p|CPU 사용률을 내림차순으로 표시|
 |shitf + m|메모리 사용률을 내림차순으로 표시|
 |shift+ t|프로세스가 돌아가고 있는 사간 순으로 표시|
 |k|kill processd의 약자, k 입력 후 종료할 PID(프로세스ID)를 입력, kill signal 9|

2. ps
* process status의 약자
* 현재 실행 중인 프로세스 목록과 상태를 보여줌
* 특정 프로세스를 확인할 때 grep 명령어와 함께 사용함

|명령어|설명|
|:---:|:---:|
|ps -a|모든 프로세스를 출력|
|ps -e|커널 프로세스를 제외한 모든 프로세스를 출력|
|ps -f|프로세스를 풀 포맷으로 출력|
|ps -l|프로세스를 긴 포맷으로 출력(-f보다 상세한 정보)|
|ps -p|특정 PID의 프로세스를 출력|
|ps -u { } |{ }계정의 프로세스 정보를 출력|

3. jobs
* 작업이 중지된 상태나 백그라운드로 진행 중인 작업의 상태를 표시하는 명령어임

|명령어|설명|
|:---:|:---:|
|jobs -l|프로세스 그룹 ID를 state 필드 앞에 출력|
|jobs -n|대표 프로세스 ID를 출력|
|jobs -p|각 프로세스 ID에 대해 한 행씩 출력|

4. 


