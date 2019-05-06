1.apt-get [option] 에 대하여 알아보자
===
### apt-get update : 패키지 인덱스의 인덱스 정보를 업데이트하는 기능을 수행
###이 인덱스는 /etc/apt/sources.list에 있음
![3](https://user-images.githubusercontent.com/49421109/57212234-0ebb5a80-701e-11e9-8f69-05d107d6973e.JPG)
### apt-get upgrade : 설치되어 있는 패키지를 모두 새버전으로 업그레이드 수행
![4](https://user-images.githubusercontent.com/49421109/57216101-d3bf2400-7029-11e9-8ad6-1536881c6f4d.JPG)
### apt-get  install [패키지명] : 패키지 설치하기
![5](https://user-images.githubusercontent.com/49421109/57216264-5811a700-702a-11e9-9f27-d173f3e59425.JPG)
### apt-get  remove [패키지명] : 패키지 제거하기(설정 파일은 제거하지 않음)
![6](https://user-images.githubusercontent.com/49421109/57223561-7636d180-7041-11e9-8d66-a9a20edd447a.JPG)
![8](https://user-images.githubusercontent.com/49421109/57223571-7cc54900-7041-11e9-9291-f0a9d3ffb6c4.JPG)
### apt-get  purge [패키지명] : 패키지 제거하기(설정 파일까지 제거)
![9](https://user-images.githubusercontent.com/49421109/57223598-8cdd2880-7041-11e9-897c-b01c2ce77160.JPG)
### apt-get  autoremove : 사용하지 않는 패키지를 찾아서 자동 제거하기
![10](https://user-images.githubusercontent.com/49421109/57223655-b9914000-7041-11e9-9cc9-6411dbbf4989.JPG)

2.apt-cache [option] 에 대하여 알아보자
===
### apt-cache search [패키지 명] : 해당 패키지와 관련된 패키지들의 정보를 알려줌
![13](https://user-images.githubusercontent.com/49421109/57223737-0d038e00-7042-11e9-9cc6-cb72f7b78bce.JPG)
### apt-cache show [패키지 명] : 해당 패키지와 관련된 패키지들의 정보를 알려줌
![14](https://user-images.githubusercontent.com/49421109/57223791-36bcb500-7042-11e9-865b-d406157a9283.JPG)






참조
https://blog.outsider.ne.kr/346
