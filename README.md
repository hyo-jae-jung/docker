[도커 교과서]  

wsl환경에서 도커를 사용하려면
wsl 설치(https://learn.microsoft.com/ko-kr/windows/wsl/install) powershell에 wsl --install 입력하면 됨  
windows도커 설치(https://learn.microsoft.com/ko-kr/windows/wsl/tutorials/wsl-containers)  

책에서 설치하라는 패키지들과 도커 패키지 저장소 인증키 설치 안해도 일단 됨. 왜 하는지 아직 모름  

docker container rm $(docker container ls -aq) / image도 동일하게 적용 가능하고 명령어는 help로 확인 가능  $()이거 사용하는건 리눅스 명령어 같음...  

docker container run (도커허브에 있는 이미지 주소) / 해당 명령어는 이미지 다운로드(pull), 도커 시작(start)을 같이 진행함  

docker exec -it (이름 혹은 ID) (shell종류 ex: /bin/sh)  / 실행중인 컨테이너에 접속  
docker desktop의 GUI 환경에서도 해당 작업 가능  

docker container commit 

도커 이미지 저장하는 방법도 알아야 할 듯  

diamol/ch03-lab 연습문제 푸는 중 실행이 안되는 컨테이너가 만들어지는 경우가 있다. 왜?  
-> 빌드가 안돼서 그런가? -> 아님 컨테이너가 실행된건 빌드가 돼서 그럼.  
-> docker run 사용 방법을 받아들이기. 컨테이너의 사용이 생각보다 유연함.  

Chapter 4 연습문제 준비...  

docker image ls  
docker system df  

최적화 말고 기본적인 도커파일 작성을 이해함.  일단 간단한 API만들어서 도커로 실행시켜보자  
