* Reference: 
* https://www.notion.so/b67ed727aea4467cbc3226bb0c8e8336
* https://fronquarry.tistory.com/28

- 목차

유투브 재생목록 바로가기

- [https://www.youtube.com/playlist?list=PLnIaYcDMsSczk-byS2iCDmQCfVU_KHWDk](https://www.youtube.com/playlist?list=PLnIaYcDMsSczk-byS2iCDmQCfVU_KHWDk)

# 1 도커와 컨테이너 소개

---

유투브 바로가기: [https://youtu.be/uE2MTTTG8uc](https://youtu.be/uE2MTTTG8uc)

## 1.1 왜 필요한지 알고 계신가요!!

- [https://www.youtube.com/watch?v=ePpiEy_C_jk](https://www.youtube.com/watch?v=ePpiEy_C_jk)
- [https://www.youtube.com/watch?v=EHCyO1G1q0U](https://www.youtube.com/watch?v=EHCyO1G1q0U)

<br/>

<p align="center"><img src="https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2Fba0cc71c-fc92-4001-beed-df7c9d580a14%2FUntitled.png?table=block&id=6d313f4e-48b7-4c9c-8f9f-a4a3e5757626&spaceId=6c6bc534-f820-444c-9de9-0ff0fe485f99&width=1710&userId=&cache=v2"></p>
<br/>

## 1.2 도커(Docker)

- 컨테이너 기술을지원하는 다양한 프로젝트 중에 하나
- 컨테이너 기술을 이전에도 있었으나 도커로 인해 알려짐
- 컨테이너 기술의 사실상 표준
- 2014 가장 인기 있는 클라우드 오픈 소스 2위(리눅스 재단 발표)
- 다양한 운영체제에서 사용 가능(리눅스, 윈도우, MacOS)
- 애플리케이션에 국한 되지 않고 의존성 및 파일 시스템까지 패키징하여 빌드, 배포, 실행을 단순
- 리눅스의 네임 스페이스와 cgroups와 같은 커널 기능을 사용하여 가상화

<br/>

<p align="center"><img src="https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F69cc3331-af46-44a7-8dec-35d0450af170%2FUntitled.png?table=block&id=7881cbaf-036b-4275-8e7f-21aacb0c89b8&spaceId=6c6bc534-f820-444c-9de9-0ff0fe485f99&width=1520&userId=&cache=v2"></p>
<br/>

도커는 다양한 클라우드 서비스 모델과 같이 사용 가능

- 이미지: 필요한 프로그램과 라이브러리, 소스를 설치한 뒤 만든 하나의 파일
- 컨테이너: 이미지를 격리하여 독립된 공간에서 실행한 가상 환경

<br/>

<p align="center"><img src="https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F4afc28bc-1717-4ee9-a2a3-cb2a6655d6f5%2FUntitled.png?table=block&id=19e1766b-2e48-48b4-a717-cb33958a126f&spaceId=6c6bc534-f820-444c-9de9-0ff0fe485f99&width=1750&userId=&cache=v2"></p>
<br/>

## 1.3 컨테이너가 해결한다!

- 동일 시스템에서 실행하는 소프트웨어의 컴포넌트가 충돌하거나 다양한 종속성을 가지고 있음
- 컨테이너는 가상머신을 사용해 각 마이크로 서비스를 격리(isolate)하는 기술
- 컨테이너는 가상머신처럼 하드웨어를 전부 구현하지 않기 때문에 매우 빠른 실행 가능
- 프로세스의 문제가 발생할 경우 컨테이너 전체를 조정해야 하기 때문에 컨테이너에 하나의 프로세스를 실행하도록 하는 것이 좋다. (브라우저와 비슷 !)

<br/>

<p align="center"><img src="https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F2b468f38-09c1-4b85-a86b-dbae70b7c8b9%2FUntitled.png?table=block&id=d5ac543e-495d-4a63-adb2-0477652a605b&spaceId=6c6bc534-f820-444c-9de9-0ff0fe485f99&width=1800&userId=&cache=v2"></p>
<br/>

하이퍼바이저의 필요 없는 공간을 활용하면 더 많은 자원을 앱에 투자 가능

## 1.4 컨테이너 성능 비교

<br/>

<p align="center"><img src="https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2Fc6390a16-1db7-4b8b-8aac-fed9de7771d2%2FUntitled.png?table=block&id=b3623c26-3e7b-4a51-b390-5de341b1b33a&spaceId=6c6bc534-f820-444c-9de9-0ff0fe485f99&width=1670&userId=&cache=v2"></p>
<br/>

VM으로 실행했을 때와 컨테이너로 실행했을 때 CPU 튀는 현상 비교

<br/>

<p align="center"><img src="https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F7d9aaf3e-5f85-4061-8890-656527470200%2FUntitled.png?table=block&id=be1dc584-fe94-44d7-ad2e-7bae3486c91f&spaceId=6c6bc534-f820-444c-9de9-0ff0fe485f99&width=1220&userId=&cache=v2"></p>
<br/>

네이티브, VM, 컨테이너로 G플롭스(GFLOPS, GPU FLoating point Operations Per Second)

 G플롭스(GFLOPS, GPU FLoating point Operations Per Second)는 컴퓨터의 성능을 수치로 나타낼 때 주로 사용되는 단위

## 1.5 컨테이너를 격리하는 기술

리눅스 네임 스페이스: 각 프로세스가 파일 시스템 마운트, 네트워크, 유저(uid), 호스트 네임(uts) 등 에 대해 시스템에 독립 뷰를 제공

<br/>

<p align="center"><img src="https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2Fe842f473-05ca-4c72-9a26-616af859fbfa%2FUntitled.png?table=block&id=f592f0d9-84c3-4797-8353-007ce10b8f95&spaceId=6c6bc534-f820-444c-9de9-0ff0fe485f99&width=1110&userId=&cache=v2"></p>
<br/>

리눅스 컨트롤 그룹: 프로세스로 소비할 수 있는 리소스 양(CPU, 메모리, I/O, 네트워크 대역대,device 노드 등)을 제한

<br/>

<p align="center"><img src="https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2Fbdebb13e-3718-4731-aab2-08f9391b2ee9%2FUntitled.png?table=block&id=3a731962-9689-4a52-9dd3-b4b7930e0033&spaceId=6c6bc534-f820-444c-9de9-0ff0fe485f99&width=1820&userId=&cache=v2"></p>
<br/>

## 1.6 도커의 한계

서비스가 커지면 커질 수록 관리해야 하는 컨테이너의 양이 급격히 증가
도커를 사용하여 관리를 한다 하더라도 쉽지 않은 형태
배포 및 컨테이너 배치 전략
스케일-인, 스케일-아웃이 어려움

<br/>

<p align="center"><img src="https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F4b022879-763c-44bc-aa09-a6a566f0d9d2%2FUntitled.png?table=block&id=46471b2b-677c-4876-a728-e4362da4cb4e&spaceId=6c6bc534-f820-444c-9de9-0ff0fe485f99&width=1390&userId=&cache=v2"></p>
<br/>

# 2 도커 설치하기

---

유투브 바로가기: [https://youtu.be/OrK3Z1CimuU](https://youtu.be/OrK3Z1CimuU)

## 2.1 이미지 파일 다운로드

실습 파일 (docker)ubuntu-18.04.2-desktop-amd64.ova 다운로드

- [https://drive.google.com/open?id=1JMs6Iw1_Ke7lz4g5tNqNE6ybA57CPVsD](https://drive.google.com/open?id=1JMs6Iw1_Ke7lz4g5tNqNE6ybA57CPVsD)
- ID:PW// server1 : test1234
- 관리자 전환: sudo -i

버츄얼 박스 다운로드

- [https://www.virtualbox.org/wiki/Downloads](https://www.virtualbox.org/wiki/Downloads)

## 2.2 리눅스 virtualbox에 준비하기

"파일 - 가상 시스템 가져오기"를 클릭하여 OVA 파일 가져오기 실행한다.

<br/>

<p align="center"><img src="https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F5b7d4a0e-daf8-49ac-ba13-d1429019a4cd%2FUntitled.png?table=block&id=2a5c094a-81d6-432e-bd75-b03da35d8b18&spaceId=6c6bc534-f820-444c-9de9-0ff0fe485f99&width=860&userId=&cache=v2"></p>
<br/>

 앞서 받은 ova를 선택하면 된다. 옵션에서는 건드릴 내용없이 진행하면 잘 실행된다.

<br/>

<p align="center"><img src="https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2Ffde70e1a-3dd7-4925-8d8e-e686af06889b%2FUntitled.png?table=block&id=57cc446e-f893-446c-9558-d031b49f28ea&spaceId=6c6bc534-f820-444c-9de9-0ff0fe485f99&width=1650&userId=&cache=v2"></p>
<br/>

## 2.3 apt로 도커 설치하기

바탕화면이 뜬 후에는 바탕화면의 빈부분을 우클릭하여 "터미널 열기"를 클릭한다.

<br/>

<p align="center"><img src="https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2Fd2b4e3d1-1720-4279-a434-f904710f5244%2FUntitled.png?table=block&id=acf1ae88-c3a2-46a8-90de-db71a8d4abdf&spaceId=6c6bc534-f820-444c-9de9-0ff0fe485f99&width=2000&userId=&cache=v2"></p>
<br/>

그 후 다음 명령을 실행한다. 만약 잠겨있는 자원이라면서 오류가 나온다면  reboot을 실행하고 다시 한번 시도한다.

```jsx
server1@server1-VirtualBox:~$ ***sudo -i***
[sudo] server1의 암호: <패스워드 입력 test1234>
root@server1-VirtualBox:~# 
root@server1-VirtualBox:~# ***apt install docker.io***
```

# 3 내가 원하는 이미지 찾기

---

유투브 바로가기: [https://youtu.be/Vz1ZVVP_KxM](https://youtu.be/Vz1ZVVP_KxM)

## 3.1 도커 레지스트리

도커 레지스트리에는 사용자가 사용할 수 있도록 데이터베이스를 통해 Image를 제공해주고 있음
누구나 이미지를 만들어 푸시할 수 있으며 푸시된 이미지는 다른 사람들에게 공유 가능

<br/>

<p align="center"><img src="https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F0d36530e-eadd-416a-b4c7-0987fd64f36a%2FUntitled.png?table=block&id=8b0f42d0-99bd-418e-88b3-149fc717db84&spaceId=6c6bc534-f820-444c-9de9-0ff0fe485f99&width=1550&userId=&cache=v2"></p>
<br/>


그림 출처: [https://github.com/dotnet-architecture/eShopModernizing/wiki/03.-Publishing-your-Windows-Container-images-into-a-Docker-Registry](https://github.com/dotnet-architecture/eShopModernizing/wiki/03.-Publishing-your-Windows-Container-images-into-a-Docker-Registry)

## 3.2 도커 퍼블릭 레지스트리 검색 및 확인

[https://hub.docker.com/](https://hub.docker.com/)

<br/>

<p align="center"><img src="https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2Fe501b756-c2e2-4459-9a91-174b6442ce23%2FUntitled.png?table=block&id=6090e4be-bd39-4529-b354-f77efe287a1c&spaceId=6c6bc534-f820-444c-9de9-0ff0fe485f99&width=2000&userId=&cache=v2"></p>
<br/>

## 3.3 도커 명령어로 검색

```jsx
sudo docker search tomcat
```

## 3.4 도커 이미지 다운로드하기

```jsx
sudo docker pull tomcat
```

## 3.5 로컬 시스템에 있는 도커 이미지 확인하기

```jsx
sudo docker images
```

# 4 도커 라이프 사이클 이해하기

---

유투브 바로가기: [https://youtu.be/1SPsdXzAtDE](https://youtu.be/1SPsdXzAtDE)

<br/>

<p align="center"><img src="https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F88036ed7-dde8-4f01-8ea9-4be6c7602f59%2FUntitled.png?table=block&id=72fbae41-53ec-4d94-b53d-a3536089b3f8&spaceId=6c6bc534-f820-444c-9de9-0ff0fe485f99&width=1800&userId=&cache=v2"></p>
<br/>

# 5 도커 라이프 사이클 명령어 실습

---

유투브 바로가기: [https://youtu.be/i-gP10UvrC8](https://youtu.be/i-gP10UvrC8)

## 5.1 도커 이미지 다운로드와 삭제

```bash
sudo docker pull consol/tomcat-7.0
sudo docker rmi consol/tomcat-7.0
```

## 5.2 톰캣 컨테이너 생성

```bash
sudo docker run -d --name tc tomcat # 톰캣 생성 및 실행
```

## 5.3 실행중인 컨테이너 확인

```bash
sudo docker ps # 톰캣 컨테이너 확인
CONTAINER ID        IMAGE               COMMAND             CREATED             STATUS              PORTS               NAMES
f6e513b399a6        tomcat              "catalina.sh run"   27 seconds ago      Up 26 seconds       8080/tcp            tc
```

## 5.4 모든 컨테이너 확인

```bash
sudo docker ps -a # 모든 컨테이너 확인
```

## 5.5 컨테이너 중지

```bash
sudo docker stop f6e513b399a6 # 컨테이너 실행 중지
f6e513b399a6

```

## 5.6 컨테이너 삭제

```bash
sudo docker rm f6e513b399a6 # 컨테이너 삭제
f6e513b399a6

```

# 6 이미지 비밀: 레이어

---

유투브 바로가기: [https://youtu.be/I07EGQaHT1E](https://youtu.be/I07EGQaHT1E)

## 6.1 레이어의 개념

<br/>

<p align="center"><img src="https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F7a08df28-55de-4645-9740-382e8dcabf5c%2FUntitled.png?table=block&id=93eca423-47a5-4232-97d9-b2011496c4e3&spaceId=6c6bc534-f820-444c-9de9-0ff0fe485f99&width=1800&userId=&cache=v2"></p>
<br/>

왼쪽: 이미지 A를 지운다 하더라도 이미지 B에서 레이어 A, B, C를 사용하고 있기 때문에 지워지지 않음

오른쪽: 이미 존재하는 레이어 A, B는 새로 다운로드 받을 필요가 없음

## 6.2 도커 이미지 정보 확인

```bash
sudo docker pull nginx
sudo docker inspect nginx
```

## 6.3 도커 이미지 저장소 위치 확인

```bash
sudo docker info
sudo -i
cd /var/lib/docker/overlay2

```

## 6.4 레이어 저장소 확인

```bash
root@server1-VirtualBox:/var/lib/docker/overlay2# ls
0cc29ea5605872d9c8291673064e85b07160203fbf04b34eeeed899731361960 # 레이어 변경 사항 저장
615767e7221dbc99b8e441e35a88df5d74c911f2674ceaa28001388535e95be2 # 레이어 변경 사항 저장
9f3bb671f38d7f61f661af369d420cdedb195e4d623bdb6ba8e3b045f72e8d69 # 레이어 변경 사항 저장
l # 원본 레이어 저장
```

## 6.5 도커 용량 확인하기

```bash
du -sh /var/lib/docker/ #도커가 설치된 환경 용량 확인
2.0G	/var/lib/docker/

du -sh /var/lib/docker/image/ # 도커 이미지에 대한 정보 저장 디렉토리
2.7M	/var/lib/docker/image/

du -sh /var/lib/docker/overlay2/ # 도커 이미지의 파일 시스템이 사용되는 실제 디렉토리
2.0G	/var/lib/docker/overlay2/

du -sh /var/lib/docker/containers/ # 도커 컨테이너 정보 저장 디렉토리
136K	/var/lib/docker/containers/
```

# 7 도커의 유용한 명령어

---

유투브 바로가기: [https://youtu.be/QLhpCbnoQkc](https://youtu.be/QLhpCbnoQkc)

## 7.1 포트포워딩으로 톰캣 실행하기

```bash
sudo docker run -d --name tc -p 80:8080 tomcat
firefox 127.0.0.1:80
```

## 7.2 컨테이너 내부 셸 실행

```bash
sudo docker exec -it tc /bin/bash
```

## 7.3 컨테이너 로그 확인

```bash
sudo docker logs tc # stdout, stderr
```

## 7.4 호스트 및 컨테이너 간 파일 복사

```bash
sudo docker cp <path> <to container>:<path>
sudo docker cp <from container>:<path> <path>
sudo docker cp <from container>:<path> <to container>:<path>
```

## 7.5 도커 컨테이너 모두 삭제

```bash
sudo docker stop `sudo docker ps -a -q`
sudo docker rm `sudo docker ps -a -q`
```

## 7.6 임시 컨테이너 생성

```bash
sudo docker run -d -p 80:8080 --rm --name tc tomcat 
```

# 8 도커 컨테이너 실행 연습문제

---

유투브 바로가기: [https://youtu.be/mOJA0_vmemQ](https://youtu.be/mOJA0_vmemQ)

1. 기존에 설치된 모든 컨테이너와 이미지 정지 및 삭제
2. 도커 기능을 사용해 Jenkins 검색
3. Jenkins를 사용하여 설치
4. Jenkins 포트로 접속하여 웹 서비스 열기
5. Jenkins의 초기 패스워드 찾아서 로그인하기

- 정답 및 해설
    
    
    1. 기존에 설치된 모든 컨테이너와 이미지 정지 및 삭제
        
        ```bash
        sudo docker stop `sudo docker ps -a -q`
        sudo docker rm `sudo docker ps -a -q`
        sudo docker rmi `sudo docker images -q`
        ```
        
    2. 도커 기능을 사용해 Jenkins 검색
        
        ```bash
        sudo docker search jenkins
        ```
        
    3. Jenkins를 사용하여 설치
        
        ```bash
        sudo docker pull jenkins
        sudo docker inspect jenkins
        sudo docker run -d -p 8080:8080 --name jk jenkins test
        ```
        
    4. Jenkins 포트로 접속하여 웹 서비스 열기
        
        ```bash
        firefox 127.0.0.1:8080
        브라우저에 캐시가 남아있는 경우에는 ctl + shift + del
        ```
        
    5. Jenkins의 초기 패스워드 찾아서 로그인하기
        
        ```bash
        sudo docker exec -it jk cat /var/jenkins_home/secrets/initialAdminPassword
        sudo docker logs jk
        ```
        
    

# 9 환경 변수 사용해 MySQL 서비스 구축하기

---

유투브 바로가기: [https://www.youtube.com/watch?v=bjDMnnAkz3U](https://www.youtube.com/watch?v=bjDMnnAkz3U)

## 9.1 docker hub에서 mysql 검색

- https://hub.docker.com/search?q=mysql&type=image
- [https://hub.docker.com/_/mysql](https://hub.docker.com/_/mysql)

<br/>

<p align="center"><img src="https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F2c955b1a-8968-4cf8-817c-01d5900db9cb%2FUntitled.png?table=block&id=188bb385-5638-46e4-9f7a-d9f3efb2a6fc&spaceId=6c6bc534-f820-444c-9de9-0ff0fe485f99&width=2000&userId=&cache=v2"></p>
<br/>

## 9.2 환경 변수 사용해 데이터 전달하기

```bash
$ docker run -d --name nx -e env_name=test1234 nginx
/# printenv env_name
```

## 9.3 MySQL 서비스 구축하기

```bash
$ docker run --name some-mysql -e MYSQL_ROOT_PASSWORD='!qhdkscjfwj@' -d mysql
$ docker exec -it some-mysql mysql
password: !qhdkscjfwj@
mysql>
```

# 10 볼륨 마운트하여 Jupyter LAB 서비스 구축

---

유투브 바로가기: [https://www.youtube.com/watch?v=kv8HF_ahW5k](https://www.youtube.com/watch?v=kv8HF_ahW5k)

## 10.1 docker hub에서 Jupyter notebook 검색

- [https://hub.docker.com/r/jupyter/datascience-notebook](https://hub.docker.com/r/jupyter/datascience-notebook)

<br/>

<p align="center"><img src="https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2Ff9c2889a-9686-43c6-9312-8e425f342d1c%2FUntitled.png?table=block&id=3e494912-7e46-4474-be43-4ef1e7eef056&spaceId=6c6bc534-f820-444c-9de9-0ff0fe485f99&width=2000&userId=&cache=v2"></p>
<br/>

## 10.2 볼륨 마운트 옵션 사용해 로컬 파일 공유하기

- 명령어 형식

```bash
docker run -v <호스트 경로>:<컨테이너 내 경로>:<권한> # /tmp:home/user:ro
```

- 권한의 종류
    - ro: 읽기 전용
    - rw: 읽기 및 쓰기

nginx로 볼륨마운트하기 

```bash
sudo docker run -d -p 80:80 --rm -v /var/www:/usr/share/nginx/html:ro nginx
curl 127.0.0.1
echo 1234 > /var/www/index.html
curl 127.0.0.1
```

## 10.3 데이터 분석가를 위한 Jupyter LAB 환경 구축하기

현재 디렉토리를 사용하여 notebook 컨테이너 실행

```bash
mkdir ~/jupyternotebook
chmod 777 ~/jupyternotebook
cd ~/jupyternotebook
sudo docker run --rm -p 8080:8888 -e JUPYTER_ENABLE_LAB=yes -v "$PWD":/home/jovyan/work:rw jupyter/datascience-notebook:9b06df75e445
```

실행하면 나오는 링크를 통해 접속한다. 

```bash
http://127.0.0.1:8080/token=??????????????????
```

주피터랩 서버로 접속해서 work으로 접속하고 새 노트북 생성하고 코드를 작성한다.

```python
print("Hello Python Jupyter Notebook")
```

타이핑 후 shift + Enter를 누르면 실행한다.

<br/>

<p align="center"><img src="https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F4cc0bae9-ed42-4044-9a22-6a90ca83b588%2FUntitled.png?table=block&id=2b27ca8d-73a1-4639-bb26-ec9c8afc3acc&spaceId=6c6bc534-f820-444c-9de9-0ff0fe485f99&width=2000&userId=&cache=v2"></p>
<br/>

# 11 직접 도커 이미지 빌드하기

---

유투브 바로가기: [https://youtu.be/59P19DFB0sc](https://youtu.be/59P19DFB0sc)

## 11.1 도커 빌드할 프로그램 준비

python를 사용해 단순한 서비스를 시작 작성한다. 다음 파일을 작성하여 test_server.py로 저장한다.

```python
# test_server.py
import socket

with socket.socket() as s:
  s.bind(("0.0.0.0", 12345))
  s.listen()
  print("server is started")
  conn, addr = s.accept()
  # conn 클라이언트와 통신할 소켓
  # addr 클라이언트의 정보가 들어있음
  with conn:
    print("Connected by", addr)
    while True:
      data = conn.recv(1024)
      if not data: break
      conn.sendall(data)
```

```bash
python3 test_server.py

---

nc 127.0.0.1 12345
```

## 11.2 도커 파일 생성

별도의 디렉토리를 생성하고 dockfile과 위에서 생성한 python파일을 새 디렉토리에 배치한다.

```bash
mkdir my_first_project
mv test_server.py ./my_first_project/
cd my_first_project/
gedit dockerfile
```

dockerfile

```docker
FROM python:3.7

RUN mkdir /echo
COPY test_server.py /echo

CMD ["python", "/echo/test_server.py"]
```

빌드 후 테스트

```bash
ls 
dockerfile test_server.py

sudo docker build -t ehco_test .
sudo docker images
sudo docker run -t -p 12345:12345 --name et --rm echo_test
```

```bash
nc 127.0.0.1 12345
```

# 12 도커 이미지 푸시

---

유투브 바로가기: [https://youtu.be/ORLVnVKrNfs](https://youtu.be/ORLVnVKrNfs)

## 12.1 도커 이미지 태그 변경 후 푸시

먼저 회원가입을 하도록 한다.

[https://hub.docker.com/](https://hub.docker.com/) 

회원가입한 정보를 토대로 다음 내용을 작성한다. login을 하지 않으면 정상 동작하지 않는다. gasbugs라는 문자열은 여러분이 사용하는 아이디로 바꿔서 실행해야만 한다.

```bash
sudo docker login
sudo docker tag echo_test ***gasbugs***/echo_test
sudo docker images
sudo docker push ***gasbugs***/echo_test
```

[https://hub.docker.com/](https://hub.docker.com/) 에 접속하여 내 레파지토리에 도커가 잘 등록됐는지 확인해본다.

모든 이미지 삭제 후 다시 gasbugs/echo_test 실행하여 잘 다운로드돼 실행되는지 테스트한다.

```bash
sudo docker rmi `docker images -q` -f
sudo docker run -t -p 12345:12345 --name et --rm gasbugs/echo_test:v3.7
```

## 12.2 도커 이미지 히스토리 확인

다음 명령을 사용하면 도커 이미지가 어떤 히스토리를 가졌는지 확인할 수 있다. 제일 상단에 앞서 우리가 dockerfile을 빌드해서 추가한 정보가 있다.

```bash
docker history ***gasbugs/echo_test***
```

# 13 프라이베이트 레지스트리 구현 및 사용

유투브 바로가기: [https://youtu.be/W1p5-CWlhV0](https://youtu.be/W1p5-CWlhV0)

private registry 만들기

```bash
docker run -d --name docker-registry -p 5000:5000 registry
```

브라우저를 켜서 127.0.0.1:5000/v2/ 서비스 접속 가능한지 확인

<br/>

<p align="center"><img src="https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2Fe1615f6f-32a7-4d11-bcd8-9ea9187e797a%2FUntitled.png?table=block&id=1564166d-8f20-4497-92d7-0ecec31cea7b&spaceId=6c6bc534-f820-444c-9de9-0ff0fe485f99&width=1340&userId=&cache=v2"></p>
<br/>

프라이베이트 레지스트리에 이미지 푸시하기

```bash
sudo docker tag echo_test 127.0.0.1:5000/echo_test
sudo docker push 127.0.0.1:5000/echo_test
```

도커 API 관련 링크: [https://docs.docker.com/registry/spec/api/](https://docs.docker.com/registry/spec/api/)

인증 관련 참고 링크: [https://docs.docker.com/registry/configuration/#auth](https://docs.docker.com/registry/configuration/#auth)

# 14 워드프레스 도커 이미지 만들기 프로젝트

---

유투브 바로가기: [https://youtu.be/FSqBdXHDwgE](https://youtu.be/FSqBdXHDwgE)

도커에서 제공하는 워드프레스와 MySQL은 따로 떨어진 형태로 존재한다. 여기서는 하나의 컨테이너에서 워드프레스와 MySQL을 동작시킬 수 있도록 만들어본다. 일단 가장 먼저 할 일은 PHP와 DB가 공존하는 환경을 찾는 것이다. 다양한 솔루션들이 있는데 그중에 XAMPP는 도커로 이미 만들어져있어 유용하게 사용할 수 있다. xampp는 apache, MariaDB, php가 설치돼 있다. 여기에 워드프레스만 올리면 바로 컨테이너를 만들 수 있다.

먼저 도커 허브에서 다음 사이트를 찾아내자.

[https://hub.docker.com/r/tomsik68/xampp](https://hub.docker.com/r/tomsik68/xampp)

이 사이트의 컨테이너를 불러온 뒤 워드프레스 설치 과정을 진행하도록 한다. 컨테이너에서 SSH와 다앙한 포트를 지원하지만 우리는 80포트만 사용할 예정이다.

```bash
sudo docker run --name WP -p 80:80 -d tomsik68/xampp
```

이제 가상환경은 준비됐으니 워드프레스를 설치하는 작업만 남았다. "워드프레스 다운로드"를 검색하자. 

워드프레스 바로가기: [https://ko.wordpress.org/download/](https://ko.wordpress.org/download/)

wget을 사용해 다운로드하고 압축을 푼다.

```bash
wget https://ko.wordpress.org/latest-ko_KR.tar.gz
tar -xf latest-ko_KR.tar.gz

```

컨테이너 내의 웹 파일 정리

```bash
sudo docker exec -it WP bash
chown daemon. /opt/lampp/htdocs 
cd /opt/lampp/htdocs/
mkdir backup
mv * ./backup/
exit

```

워드프레스 파일을 컨테이너에  복사하고 웹 루트 디렉토리에 배치

```python
sudo docker cp wordpress WP:/opt/lampp/htdocs
sudo docker exec -it WP bash
mv /opt/lampp/htdocs/wordpress/* /opt/lampp/htdocs/
exit
sudo docker restart WP

```

127.0.0.1/phpmyadmin으로 접속해서 wordpress 데이터베이스 생성한다.

<br/>

<p align="center"><img src="https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2Fe75ebd68-2a16-4990-9bc8-3899c259608a%2FUntitled.png?table=block&id=88a1cda8-d0cc-4d1c-8683-c774b435a5fa&spaceId=6c6bc534-f820-444c-9de9-0ff0fe485f99&width=1770&userId=&cache=v2"></p>
<br/>

마지막으로 127.0.0.1로 접속하여 워드프레스 설치를 웹 브라우저 화면으로 진행하면 된다.
