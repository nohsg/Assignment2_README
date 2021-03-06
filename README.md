# 오픈소스SW개론 과제2_컴퓨터공학과 20200128 노슬기
## 리눅스 명령어 top, ps, jobs, kill

 ***1. top***
 * 현재 os 상태를 나타내주는 CLI 어플리케이션임
 * 시스템 현재 시간, 유저, 로드 애버리지, 메모리 사용량, CPU 사용량 등 시스템의 상태를 실시간으로 파악할 수 있음
 
 |명령어|설명|
 |:---:|:---:|
 |shift + p|CPU 사용률을 내림차순으로 표시|
 |shift+ m|메모리 사용률을 내림차순으로 표시|
 |shift+ t|프로세스가 돌아가고 있는 사간 순으로 표시|
 |k|kill process의 약자, k 입력 후 종료할 PID(프로세스ID)를 입력, kill signal 9|


***2. ps***
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


***3. jobs***
* 작업이 중지된 상태나 백그라운드로 진행 중인 작업의 상태를 표시하는 명령어임

|명령어|설명|
|:---:|:---:|
|jobs -l|프로세스 그룹 ID를 state 필드 앞에 출력|
|jobs -n|대표 프로세스 ID를 출력|
|jobs -p|각 프로세스 ID에 대해 한 행씩 출력|


***4. kill***
* 프로세스에 signal을 보내 작업을 수행하게 하는 명령어임
* 종료되지 않는 프로세스를 종료시킬 때 주로 사용함

|명령어|설명|
|:---:|:---:|
|kill -l|signal 종류를 출력|
|kill -1|연결 끊기|
|kill -2|인터럽트|
|kill -3|종료+코어덤프|
|kill -9|강제 종료|
|kill -15|정상 종료|
|kill -18|정지된 프로세스 재실행|
|kill -19|정지|

---

## vim 에디터에서 매크로 사용방법

|명령어|설명|
|:---:|:---:|
|q + {문자}|특정 문자를 눌러 반복하고 싶은 동작 기록|
|q|특정 문자에 매크로 저장|
|@{문자}|특정 문자를 눌러 저장된 매크로 실행|

__* 매크로 반복__

> @{문자} : 저장된 매크로 1회 실행
> 
> @@ : 직전에 실행한 매크로 재실행
> 
> (반복횟수)@{문자} : 반복횟수만크 매크로 재실행





##### 출처 및 참고자료
[top 명령어](https://sabarada.tistory.com/146)

[top 명령어](https://ironmask84.tistory.com/355)

[top 명령어](https://dany-it.tistory.com/348)

[top 명령어](https://cheershennah.tistory.com/172)

[top 명령어](https://zzsza.github.io/development/2018/07/18/linux-top/)

[ps 명령어](https://jhnyang.tistory.com/268)

[ps 명령어](https://newstars.cloud/468)

[ps 명령어](https://arer.tistory.com/150)

[ps 명령어](https://tigris-data-science.tistory.com/entry/Linux-ps-%EB%AA%85%EB%A0%B9%EC%96%B4)

[jobs 명령어](https://hbase.tistory.com/265)

[jobs 명령어](https://shaeod.tistory.com/968)

[jobs 명령어](https://starrykss.tistory.com/1694)

[kill 명령어](https://velog.io/@ogu1208/Linux-kill-%EB%AA%85%EB%A0%B9%EC%96%B4)

[kill 명령어](https://bigsun84.tistory.com/355)

[kill 명령어](https://121202.tistory.com/45)

[vim macro](https://jmoon.co.kr/38)

[vim macro](https://coldmater.tistory.com/226)

[vim macro](https://stdout.tistory.com/46)

[vim macro](https://booolean.tistory.com/849)

[vim macro](https://tzara.tistory.com/150)

[vim macro](https://clem.tistory.com/29)
