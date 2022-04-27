Kubernetes Start !!

[ 용량 조회 ]

전체용량
df -P | grep -v ^Filesystem | awk '{sum += $2} END { print sum/1024/1024 " GB" }'

전체사용량 
df -P | grep -v ^Filesystem | awk '{sum += $3} END { print sum/1024/1024 " GB" }'

전체남은용량
df -P | grep -v ^Filesystem | awk '{sum += $4} END { print sum/1024/1024 " GB" }

[ 개념 ]

crul = 서버와 통신할 수 있는 커맨드 명령어 툴. 웹개발에 매우 많이 사용되고 있는 무료 오픈소스, curl의 특징으로는 수 많은 프로토콜을 지원한다는 장점이 있다.
