# hyperledger-fabric-medical


1. git을 command창을 활용하여 설치합니다. 

$ sudo apt-get install git -y 

1.1 git 설치 확인을 위해 다음의 명령어를 입력하여 2.7.4의 버전으로 알맞게 설치가 되었는지 확인합니다. 

$ git version 

2. cURL 설치 

$ sudo apt-get install curl -y 

2.1 cURL이 제대로 설치가 되었는지 확인하기 위해 다음의 명령어를 입력하여 버전이 7.47.0이 맞는 지 확인합니다. 

    		$ curl –version 

3. 다음의 명령어를 입력하여 Go 1.15 을 설치합니다. 

    	$ sudo wget https://golang.org/dl/go1.15.10.linux-amd64.tar.gz 

    	$ sudo tar -C /opt -xzf go1.15.10.linux-amd64.tar.gz 

    	$ sudo rm go1.5.10.linux-amd64.tar.gz 

3.1 go 언어가 잘 설치되었는지 확인하기 위해 아래의 명령어를 입력해서 go1.15.10의 버전을 확인합니다. 

    		$ go version 

4. 아래의 명령어를 입력하여 Docker을 설치합니다. 

    	$ sudo apt-get install apt-transport-https ca-certificates curl software-properties-common 

4.1 패키지 업데이트를 위해 다음의 명령어를 입력합니다. 

    		$ sudo apt-get update 

4.2 최신 버전 CE 설치를 위해 다음의 명령어를 입력합니다. 

    		$ sudp apt-get -y install docker-ce 

4.3 사용자에게 권한을 부여하기 위해 다음의 명령어를 입력합니다. 

    		$ sudo usermod -a -G docker $(id -un) 

4.4 docker의 설치 버전을 확인하기 위해 다음의 명령어를 입력하고 버전이 20.10.5가 맞는지 확인합니다. 

    		$ docker version 

5. 최신 버전의 docker-compose 를 설치하기 위해 다음의 명령어를 입력합니다. 

    $ sudo curl -L https://github.com/docker/compose/releases/download/1.27.2/docker-compose-$(uname -s)-$(unmae -m) -o /usr/local/bin/docker-compose  

5.1 바이너리에 실행 권한을 추가하기 위해 아래의 명령어를 입력합니다. 

    		$ sudo chomod +x /usr/local/bin/docker-compose 

5.2 설치 버전을 확인하기 위해 다음의 명령어를 입력한 후 버전이 1.27.2가 맞는지 확인합니다. 

               $ docker-compose -v 

6. jq를 설치하기 위해 아래의 명령어를 입력합니다. 

    $ sudo apt-get install jq -y 

6.1 설치 버전을 확인하기 위해 다음의 명령어를 입력한 후 버전이 jq-1.5-1-a5b5cbe 가 맞는지 확인합니다. 

    	     $ jq --version 

7. sample-network와 turorial을 진행하기 위해 Fabric-samples 설치를 아래의 명령어를 통해 진행합니다. 

    $ curl -sSL https://bit.ly/2ysbOFE | bash -s --2.2 1.4.9 

7.1 Fabric image를 확인하기 위해 아래의 명령어를 입력합니다. 

    	    $ docker images 
