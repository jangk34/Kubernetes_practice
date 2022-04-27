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

crul = 서버와 통신할 수 있는 커맨드 명령어 툴. 웹개발에 매우 많이 사용되고 있는 무료 오픈소스, curl의 특징으로는 수 많은 프로토콜을 지원한다는 장점이 있다.

 
