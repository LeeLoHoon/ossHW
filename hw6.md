1.apt-get [option] 에 대하여 알아보자
===
apt-get update : 패키지 인덱스의 인덱스 정보를 업데이트하는 기능을 수행
### 
이 인덱스는 /etc/apt/sources.list에 있음
###
![3](https://user-images.githubusercontent.com/49421109/57212234-0ebb5a80-701e-11e9-8f69-05d107d6973e.JPG)
apt-get upgrade : 설치되어 있는 패키지를 모두 새버전으로 업그레이드 수행
### 
![4](https://user-images.githubusercontent.com/49421109/57216101-d3bf2400-7029-11e9-8ad6-1536881c6f4d.JPG)
apt-get  install [패키지명] : 패키지 설치하기
### 
![5](https://user-images.githubusercontent.com/49421109/57216264-5811a700-702a-11e9-9f27-d173f3e59425.JPG)
apt-get  remove [패키지명] : 패키지 제거하기(설정 파일은 제거하지 않음)
### 
![6](https://user-images.githubusercontent.com/49421109/57223561-7636d180-7041-11e9-8d66-a9a20edd447a.JPG)
![8](https://user-images.githubusercontent.com/49421109/57223571-7cc54900-7041-11e9-9291-f0a9d3ffb6c4.JPG)
apt-get  purge [패키지명] : 패키지 제거하기(설정 파일까지 제거)
### 
![9](https://user-images.githubusercontent.com/49421109/57223598-8cdd2880-7041-11e9-897c-b01c2ce77160.JPG)
apt-get  autoremove : 사용하지 않는 패키지를 찾아서 자동 제거하기
### 
![10](https://user-images.githubusercontent.com/49421109/57223655-b9914000-7041-11e9-9cc9-6411dbbf4989.JPG)

2.apt-cache [option] 에 대하여 알아보자
===
apt-cache search [key word] : 해당 key word와 관련된 패키지들의 정보를 알려줌
### 
![13](https://user-images.githubusercontent.com/49421109/57223737-0d038e00-7042-11e9-9cc6-cb72f7b78bce.JPG)
apt-cache show [패키지 명] : 해당 패키지에 해당하는 소프트웨어에 대한 정보를 알려줌
### 
![14](https://user-images.githubusercontent.com/49421109/57223791-36bcb500-7042-11e9-865b-d406157a9283.JPG)
apt-cache stats  : 설치된 모든 패키지에 대한 상태정보를 알려줌
### 
![15](https://user-images.githubusercontent.com/49421109/57224056-193c1b00-7043-11e9-99e2-63b13c36fd07.JPG)
apt-cache pkgnames  : 시스템에 설치되어 있는 모든 패키지 목록을 알려줌
### 
![16](https://user-images.githubusercontent.com/49421109/57224195-9cf60780-7043-11e9-9b2d-b34df92bd276.JPG)
![17](https://user-images.githubusercontent.com/49421109/57224197-9d8e9e00-7043-11e9-9532-d8a160d0e581.JPG)

3.PHP , MYSQL, Phpmyadmin을 설치한 후 잘 설치 되었는지 확인해 보자.
===
PHP를 설치하고 apache2와 연동이 되는지 확인해보자
###

php와 apache2의 연동을 확인하기 위해 index.html파일을 수정하고 index.php파일 생성하기
####
![18](https://user-images.githubusercontent.com/49421109/57226500-2d374b00-704a-11e9-90b2-b17a2358872d.JPG)
![19](https://user-images.githubusercontent.com/49421109/57226502-2dcfe180-704a-11e9-9ec9-9be52cd546ea.JPG)
![20](https://user-images.githubusercontent.com/49421109/57226527-3c1dfd80-704a-11e9-9c74-eedeeeebaa18.JPG)
![21](https://user-images.githubusercontent.com/49421109/57226531-3f18ee00-704a-11e9-995f-2fd431670d59.JPG)
![22](https://user-images.githubusercontent.com/49421109/57226537-404a1b00-704a-11e9-819b-303b97f6f9c1.JPG)
![23](https://user-images.githubusercontent.com/49421109/57226565-4c35dd00-704a-11e9-8950-6187ea93c605.JPG)
![28](https://user-images.githubusercontent.com/49421109/57226752-a20a8500-704a-11e9-974a-669c20c04580.JPG)
![24](https://user-images.githubusercontent.com/49421109/57226570-4f30cd80-704a-11e9-901f-dbc3f7504c26.JPG)
![25](https://user-images.githubusercontent.com/49421109/57226574-51932780-704a-11e9-83bd-d83e7291f926.JPG)

MYSQL을 설치하고  설치가 정상적으로 완료되었는지, 작동하고 있는지 확인하기
####
![26](https://user-images.githubusercontent.com/49421109/57226668-7a1b2180-704a-11e9-88dc-0a6beeaa474d.JPG)
![27](https://user-images.githubusercontent.com/49421109/57226675-7be4e500-704a-11e9-8b79-665b5a241d61.JPG)

###Phpmyadmin을 설치하고 정상적으로 완료되었는지, 작동하고 있는지 확인하기
![phpmy0](https://user-images.githubusercontent.com/49421109/57226911-062d4900-704b-11e9-8bc2-b44d886a3944.JPG)
![phpmu 01](https://user-images.githubusercontent.com/49421109/57226912-06c5df80-704b-11e9-8345-bb281793d2d1.JPG)
![phpmyadmin 설치](https://user-images.githubusercontent.com/49421109/57226914-07f70c80-704b-11e9-816f-85af4986458c.JPG)
![phpmy 설치2](https://user-images.githubusercontent.com/49421109/57226917-09283980-704b-11e9-8c91-615f15a2c981.JPG)
![phpmy 3](https://user-images.githubusercontent.com/49421109/57226924-0d545700-704b-11e9-8662-b3a83b7ca36d.JPG)
![phpmy4](https://user-images.githubusercontent.com/49421109/57226927-0fb6b100-704b-11e9-84b7-e013a8b39252.JPG)
![phpmy5](https://user-images.githubusercontent.com/49421109/57226931-12b1a180-704b-11e9-9649-6b0bb3a3e7e8.JPG)

4.apache 서버의 상태확인 및 시작과 중지 그리고 재시작하는 방법을 알아보자.
===
apache 재시작 하기 및 상태 확인
###
![29](https://user-images.githubusercontent.com/49421109/57227003-4b517b00-704b-11e9-8b37-ff95b9e5a230.JPG)
apache 중지 했다가 시작하기
###
![30](https://user-images.githubusercontent.com/49421109/57227020-573d3d00-704b-11e9-8a50-ccc7d03efb2e.JPG)
![31](https://user-images.githubusercontent.com/49421109/57227026-5b695a80-704b-11e9-9264-8d3b24ca9f01.JPG)

5.홈 디렉터리 변경하기
===
기존의 홈 디렉터리는 /var/www/html/ 인데 이것을 바꾸는 방법에 대해서 알아보자.
###
![32](https://user-images.githubusercontent.com/49421109/57227131-9b304200-704b-11e9-8b23-d0c7488dace0.JPG)
![33](https://user-images.githubusercontent.com/49421109/57227212-c7e45980-704b-11e9-8e10-5292c4120854.JPG)
![41](https://user-images.githubusercontent.com/49421109/57227292-fcf0ac00-704b-11e9-953a-60c607a10109.JPG)
![42](https://user-images.githubusercontent.com/49421109/57227300-02e68d00-704c-11e9-846e-ebbdf75d9e19.JPG)
![34](https://user-images.githubusercontent.com/49421109/57227219-cadf4a00-704b-11e9-8dbb-f9e2cf98d1c3.JPG)
![35](https://user-images.githubusercontent.com/49421109/57227233-d0d52b00-704b-11e9-8cd6-588526bae6bc.JPG)
![36](https://user-images.githubusercontent.com/49421109/57227238-d599df00-704b-11e9-83ea-1c42e8786009.JPG)
![37](https://user-images.githubusercontent.com/49421109/57227244-db8fc000-704b-11e9-99c0-c8461aff2489.JPG)
오류 발견
####
![38](https://user-images.githubusercontent.com/49421109/57227256-e5192800-704b-11e9-9c6e-b6c5a8c98729.JPG)
해결 방법
####
![39](https://user-images.githubusercontent.com/49421109/57227261-e9454580-704b-11e9-9a83-94c4b69cc977.JPG)
![40](https://user-images.githubusercontent.com/49421109/57227268-efd3bd00-704b-11e9-8959-dfe05aee1a18.JPG)
![28](https://user-images.githubusercontent.com/49421109/57227338-1b56a780-704c-11e9-8639-c18414833726.JPG)
해결한 후 화면
####
![43](https://user-images.githubusercontent.com/49421109/57227321-0da12200-704c-11e9-865a-cc00b31bfb61.JPG)

6.도메인 이름 세팅하기 및 호스트 변경하기
===
도메인 이름 세팅하기
###
내 이름을 딴 easy.com이라는 도메인을 세팅하고 싶지만 이미 easy.com이라는 사이트는 존재한다.
![1](https://user-images.githubusercontent.com/49421109/57227524-9455ff00-704c-11e9-8dd7-f2014adcdfec.JPG)
이때 /etc/hosts로 들어가서 easy.com 이라는 사이트를 추가하면 기존의 사이트가 아닌 내가 만든 easy.com 도메인으로 들어갈 수 있게 된다.(DNS 서비스 특성상 제일 먼저 내 도메인 서버에서 물어보기 때문)
![2](https://user-images.githubusercontent.com/49421109/57230691-e6e6e980-7053-11e9-8f65-4f0f019a4fee.JPG)



7.DB 계정 만들어 wordpress 설치 및 확인하기

![3](https://user-images.githubusercontent.com/49421109/57230694-eb130700-7053-11e9-91fa-dc65d58a18c4.JPG)

![4](https://user-images.githubusercontent.com/49421109/57230711-f1a17e80-7053-11e9-88f8-9a71e7c78b4e.JPG)

![6](https://user-images.githubusercontent.com/49421109/57230749-03832180-7054-11e9-8d28-156c83377594.JPG)
![7](https://user-images.githubusercontent.com/49421109/57230757-067e1200-7054-11e9-80c5-f453ca075f81.JPG)
![8](https://user-images.githubusercontent.com/49421109/57230760-0847d580-7054-11e9-81da-ae6583b92c78.jpg)
![9](https://user-images.githubusercontent.com/49421109/57230764-0bdb5c80-7054-11e9-8e86-6ac3da986d50.JPG)
![10](https://user-images.githubusercontent.com/49421109/57231500-95d7f500-7055-11e9-958d-1056499d2bf0.JPG)
![11](https://user-images.githubusercontent.com/49421109/57231853-62e23100-7056-11e9-99ac-fd0019562692.JPG)
![12](https://user-images.githubusercontent.com/49421109/57231866-6b3a6c00-7056-11e9-9ef0-23c3ece3050b.JPG)
![13](https://user-images.githubusercontent.com/49421109/57231875-6e355c80-7056-11e9-9a43-af629e0616cd.JPG)
이 내용이 없어서 오류
####
![14](https://user-images.githubusercontent.com/49421109/57231876-6f668980-7056-11e9-9fc6-2379a9596e17.JPG)
필요한 파일 만들기
####
![15](https://user-images.githubusercontent.com/49421109/57231878-7097b680-7056-11e9-9439-da9395f4982e.JPG)
붙여넣기
####
![16](https://user-images.githubusercontent.com/49421109/57231884-72fa1080-7056-11e9-9add-cec509ad3a32.JPG)
설치실행
####
![17](https://user-images.githubusercontent.com/49421109/57231894-768d9780-7056-11e9-9285-3174bac1ac1b.JPG)



8.웹 호스팅 Virtual Host 세팅 방법(여러가지 가상의 호스트 세팅하기)
===
포트로 구분하여 두개의 가상 호스트 추가하기
###
![18](https://user-images.githubusercontent.com/49421109/57233292-51e6ef00-7059-11e9-92b3-f31591728c3b.JPG)
![19](https://user-images.githubusercontent.com/49421109/57233293-53181c00-7059-11e9-9857-7fd02a252792.JPG)
새로운 계정을 복사하여 2개더 만들기
###
![20](https://user-images.githubusercontent.com/49421109/57233333-675c1900-7059-11e9-9550-3201274bd753.JPG)
각각의 html파일 만들기
###
![21](https://user-images.githubusercontent.com/49421109/57233353-6dea9080-7059-11e9-833a-e9a4b94683dc.JPG)

위에서 처럼 각각의 계정 별로 wordpress만들기
###
![555](https://user-images.githubusercontent.com/49421109/57233409-89ee3200-7059-11e9-8843-034a1b7a3113.png)




참조
https://blog.outsider.ne.kr/346
https://thebook.io/006718/part02/ch08/03/01/
https://storycompiler.tistory.com/118
https://all-record.tistory.com/96
