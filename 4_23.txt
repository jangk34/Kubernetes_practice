<<<< Kubernetes 실습 환경 >>>>

[상식] 

tty - tty는 프로세스가 실행된 터미널 포트를 가리킨다.

[ 컨테이너 생성 및 접속 방법 ]

  1. docker pull (이미지 없을떄 가져오기) -> docker create -> docker start -> docker attach 

★2. docker run (이미지 없을떄 가져오기)  

docker run -i -t ubuntu20.04 = 도커 생성후 컨테이너 내부 접속

docker images = 도커 목록 확인

docker create -i -t --name "컨테이너 이미지 이름" "os명" = 도커 생성후 컨테이너 접속 x

docker start "이미지 이름" = 컨테이너 시작  

docker attach "이미지 이름" = 컨테이너 내부 접속

exit (컨테이너 정지시키고 나가기 )  <--> ctrl + p,q =  ( 컨테이너 정지 없이 나가기 )

docker ps = 컨테이너 목록 확인 ( 정지되지 않은 컨테이너만 출력 )

docker ps -a = 모든 컨테이너 목록 확인 ( 정지 포함 )

docker stop "컨테이너 이미지 이름" = 컨테이너 정지 ( 컨테이너 수정/삭제 불가시 정지시키고 해야함 )

docker rename "기존이름" "바꿀이름" = 컨테이너 이름 변경 (run으로 생성시 무작위 이름 생기기때문에 바꿔줌)

docker rm "컨테이너 이미지 이름" = 컨테이너 삭제

docker rm -f "컨테이너 이미지 이름" = 실행중인 컨테이너 삭제

docker container prune = 컨테이너 모두 삭제














