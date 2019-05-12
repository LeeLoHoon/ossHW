하나의 서버(가상 머신의 내 우분투 서버)에서 서로 다른 유저에게 웹을 호스팅 해주려면 어떤 설정이 필요할까?
====
한번에 3개의 가상 웹을 세명의 유저에게 호스팅 한다고 생각하고 단계별로 해야할 일을 알아보자.
#
첫번째 해야 할 일은 /var/www/html에 주어져 있던 권한을 각각의 유저의 home 디렉터리에 있는 html이라는 디렉터리로 권한을 주는 일을 해야한다.
##
![1](https://user-images.githubusercontent.com/49421109/57582375-04f29500-74ff-11e9-81b2-18b16a5b6f66.JPG)
두번째 해야 할 일은 두개의 유저를 만들고 그안에 html이라는 디렉터리 그리고 그 안에 index.html 파일을 만드는 것이다.
##
![8](https://user-images.githubusercontent.com/49421109/57582466-230cc500-7500-11e9-98b4-cebbc6ece997.JPG)
![9](https://user-images.githubusercontent.com/49421109/57582473-3ae44900-7500-11e9-8ccf-2e934c53562c.JPG)
![10](https://user-images.githubusercontent.com/49421109/57582474-3d46a300-7500-11e9-82a0-6951e5e49092.JPG)
![11](https://user-images.githubusercontent.com/49421109/57582475-4172c080-7500-11e9-8536-d6bef98ce595.JPG)
![12](https://user-images.githubusercontent.com/49421109/57582476-433c8400-7500-11e9-8a48-32323a24a477.JPG)
세번째로 해야 할 일은 각각의 유저들의 html안에 있는 index.html과 연결할 사이트를 만드는 것이다.
##
![3](https://user-images.githubusercontent.com/49421109/57582496-8696f280-7500-11e9-8a77-a75e9183b11a.JPG)
이렇게 각각의 유저를 위한 conf 파일을 만든 후(default는 easy를 위한 conf파일로 남겨둔다.)
###
![2](https://user-images.githubusercontent.com/49421109/57582516-b34b0a00-7500-11e9-9ef2-5f888eee316f.JPG)
![4](https://user-images.githubusercontent.com/49421109/57582517-b514cd80-7500-11e9-9614-c68bbb8cf7ef.JPG)
![5](https://user-images.githubusercontent.com/49421109/57582518-b6de9100-7500-11e9-9f69-12e41782b21d.JPG)
네번째로 해야할 일은  위에서 만든 사이트들이 현실에서 내가 구매한 도메인이 아니기 때문에 DNS server ip로 request를 던지기 전에 hosts를 조정함으로써 차단 및 자신의 ip로의 request를 유도해야 한다.
##
![6](https://user-images.githubusercontent.com/49421109/57582567-3f5d3180-7501-11e9-8c0f-a26576ed0ef3.JPG)
![7](https://user-images.githubusercontent.com/49421109/57582571-5439c500-7501-11e9-8408-a1c3b34be17c.JPG)
이제 연결이 완료 되었는지 확인을 해보아야 한다.
###
![14](https://user-images.githubusercontent.com/49421109/57582578-60be1d80-7501-11e9-865c-f192b5bf1db5.JPG)
![15](https://user-images.githubusercontent.com/49421109/57582579-6156b400-7501-11e9-9692-d09890fda823.JPG)
![16](https://user-images.githubusercontent.com/49421109/57582582-6451a480-7501-11e9-94cb-a109e44c2ac9.JPG)
잘 연결 되었음을 알 수 있다.
###

다섯번째로 해야할 일은 mysql를 통해 DB를 3개 만들어야 한다.(각각의 웹 사이트를 수정 및 저장하기 위해)
##
![17](https://user-images.githubusercontent.com/49421109/57582596-9d8a1480-7501-11e9-844e-abae941a0c2b.JPG)
![18](https://user-images.githubusercontent.com/49421109/57582600-aaa70380-7501-11e9-8256-fef3f648013a.JPG)







두번째는 각각의 유저들이 가지고 싶어하는 도메인 이름의 웹 사이트를 만들고 활성화 해야한다.
(이때, 아직 유저들을 만들고 DB를 만들지는 않았지만 만들 것이라는 가정하에 진행한다.) 
