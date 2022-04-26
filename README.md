Kubernetes Start !!

전체용량
df -P | grep -v ^Filesystem | awk '{sum += $2} END { print sum/1024/1024 " GB" }'

전체사용량 
df -P | grep -v ^Filesystem | awk '{sum += $3} END { print sum/1024/1024 " GB" }'

전체남은용량
df -P | grep -v ^Filesystem | awk '{sum += $4} END { print sum/1024/1024 " GB" }'

