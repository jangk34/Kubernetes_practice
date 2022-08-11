Kubernetes Start !!

[ 용량 조회 ]

전체용량
df -P | grep -v ^Filesystem | awk '{sum += $2} END { print sum/1024/1024 " GB" }'

전체사용량 
df -P | grep -v ^Filesystem | awk '{sum += $3} END { print sum/1024/1024 " GB" }'

전체남은용량
df -P | grep -v ^Filesystem | awk '{sum += $4} END { print sum/1024/1024 " GB" }

[ 개념 ]

CLI(Command-line interface) = 터미널상 입력과 출력을 하는 명령어 인터페이스 ex) cmd, 리눅스 ssh모드

GUI(Graphical user interface) = 그래픽 인터페이스 ex) 윈도우 바탕화면

[ 명령어 ]

crul = 서버와 통신할 수 있는 커맨드 명령어 툴. 웹개발에 매우 많이 사용되고 있는 무료 오픈소스, curl의 특징으로는 수 많은 프로토콜을 지원한다는 장점이 있음.

[ vi 에디터 사용 ++ ]

1. 먼저 첫줄(g)이나 끝줄(G)로 이동
2.  shift + v + g (전체선택)
3.  d = 전체 삭제
    y = 복사
    p = 붙여넣기

[ git reset ] - 잘못된 커밋 되돌리기
reset하고자하는 commit으로 돌아간 후(git log로 확인), 저장소는 해당 commit으로 재설정되고, 이후 commit을 전부 삭제

명령어는 아래와 같이 사용한다.
 
git reset [--option(hard/soft/mixed)] [commit]
 
option : 

--hard : 돌아간 커밋 이후의 변경 이력을 전부 삭제
--soft : 변경 이력 삭제, 변경 내용은 남아있음, 인덱스 초기화(git add가 안되어 있는 상태)
--mixed : 변경 이력 삭제, 변경 내용은 남이있음, 인덱스도 유지(git add까지 되어 있음) 

[[ 통신 조회 ]]
1. ping
2. nslookup
3. telnet
