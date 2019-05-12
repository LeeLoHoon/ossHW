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

여섯번째로 해야할 일은 wordpress를 각각의 유저의 디렉터리에 각각의 유저 권한으로 설치하는 것이다.
##
![19](https://user-images.githubusercontent.com/49421109/57582681-b2b37300-7502-11e9-82fb-f7c29fd48111.JPG)
![20](https://user-images.githubusercontent.com/49421109/57582686-bd6e0800-7502-11e9-823c-b9e319ba161f.jpg)
![21](https://user-images.githubusercontent.com/49421109/57582689-c068f880-7502-11e9-9539-f72d8d9e5155.JPG)

이제 설치가 완료 되었고 각각의 유저가 firefox에서 도메인명/wordpress를 입력하면 다음과 같은 화면이 나온다.
###
![22](https://user-images.githubusercontent.com/49421109/57582700-d7a7e600-7502-11e9-8018-ea8614333c35.JPG)
![23](https://user-images.githubusercontent.com/49421109/57582719-01f9a380-7503-11e9-9687-c3392f4ca2c7.JPG)

필요한 정보를 입력하고 넘어가면
###
![24](https://user-images.githubusercontent.com/49421109/57582706-df678a80-7502-11e9-9ff6-7169c7d7749b.JPG)

이런 화면이 나오는데 이것은 필요한 파일과 파일 내용의 누락으로 생기는 메시지로 필요한 파일을 만들고 주황색 부분을 복사해서 붙여 넣어주면 된다.
![25](https://user-images.githubusercontent.com/49421109/57582721-0a51de80-7503-11e9-9b9c-799017f4275d.JPG)
![26](https://user-images.githubusercontent.com/49421109/57582722-0aea7500-7503-11e9-8c72-fec2ffc0bdae.JPG)

그 다음 진행을 클릭하면
###
![27](https://user-images.githubusercontent.com/49421109/57582727-15a50a00-7503-11e9-8925-a15fbe546f5d.JPG)
![28](https://user-images.githubusercontent.com/49421109/57582733-31101500-7503-11e9-8df1-810caf5675e7.JPG)

위와 같은 작업을 새로운 유저에서도 동일하게 적용하고 나면
###
![29](https://user-images.githubusercontent.com/49421109/57582786-e773fa00-7503-11e9-9302-b3edcdc3f06e.jpg)
![30](https://user-images.githubusercontent.com/49421109/57582787-e80c9080-7503-11e9-8a65-024698aef5be.JPG)

위와 같이 유저를 변경할 수 있다.
###
![33](https://user-images.githubusercontent.com/49421109/57582738-49802f80-7503-11e9-9370-8160583325a9.JPG)
![34](https://user-images.githubusercontent.com/49421109/57582739-4a18c600-7503-11e9-885b-e34a22ba82aa.JPG)

다음과 같이 두개의 웹 사이트 호스팅 및 wordpress설치가 완료 된다.

마지막으로 wordpress의 테마를 변경시키는 작업을 해보자.(1)
##
![35](https://user-images.githubusercontent.com/49421109/57582744-76ccdd80-7503-11e9-96eb-f20963333176.JPG)
![36](https://user-images.githubusercontent.com/49421109/57582745-77657400-7503-11e9-8369-f32f8546fb0b.JPG)
다음과 같이 wordpress 내에 설치되어 있는 테마들을 적용할 수 있다.
![37](https://user-images.githubusercontent.com/49421109/57582793-0f635d80-7504-11e9-894e-7c445272b628.JPG)

방문자 입장에서 접속하면 다음과 같은 활성화된 테마가 보여진다.
###

다른 wordpress의 테마를 변경시키는 작업을 해보자.(2)
##
![38](https://user-images.githubusercontent.com/49421109/57583556-7553e300-750c-11e9-99cb-9583633a4ec1.JPG)
![39](https://user-images.githubusercontent.com/49421109/57583558-771da680-750c-11e9-8ba8-43571413d3a8.JPG)
![40](https://user-images.githubusercontent.com/49421109/57583559-7ab12d80-750c-11e9-88d9-38565e4f7105.JPG)

다음과 같이 마음에 드는 테마를 선택하여 설치를 하면 다음과 같은 에러가 연속해서 나타난다.
###
![40-1](https://user-images.githubusercontent.com/49421109/57583567-94527500-750c-11e9-9a8b-dce0880215a8.JPG)
![40-2](https://user-images.githubusercontent.com/49421109/57583571-96b4cf00-750c-11e9-9033-782a1d638ef8.JPG)

첫번째 에러 해결방법은 다음과 같이 wp-config.php파일에 define을 추가하여 해결한다.
####
![41](https://user-images.githubusercontent.com/49421109/57583580-a502eb00-750c-11e9-9b1c-4a2c1b258e29.JPG)

두번째 에러는 권한의 문제로 발생하는 에러로 권한을 수정해 준다.
####
![42](https://user-images.githubusercontent.com/49421109/57583586-bfd55f80-750c-11e9-81bc-63d0a1c5d7e9.JPG)

설치를 완료하고 새로고침하면 다음과 같이 활성화 됨을 볼 수 있다.
####
![43](https://user-images.githubusercontent.com/49421109/57583597-e1cee200-750c-11e9-9b4c-2efbfede5b4d.JPG)
![44](https://user-images.githubusercontent.com/49421109/57583596-e0051e80-750c-11e9-8ec6-cf061a5daf3b.JPG)

또다른 wordpress의 테마를 변경시키는 작업을 해보자.(3)
##
![45](https://user-images.githubusercontent.com/49421109/57583601-f7440c00-750c-11e9-81af-2ea17383c025.JPG)
![46](https://user-images.githubusercontent.com/49421109/57583603-fb702980-750c-11e9-8d29-69463c83d11f.JPG)

다음과 같이 원하는 테마를 다운로드 (무료 or 유료 테마) 한 후
###
![47](https://user-images.githubusercontent.com/49421109/57583613-0e82f980-750d-11e9-8fba-5ed95a6b035a.JPG)
![48](https://user-images.githubusercontent.com/49421109/57583616-117dea00-750d-11e9-8d9b-6b6e2472aab4.JPG)

테마를 업로드 하여 설치를 누르면
###
![50](https://user-images.githubusercontent.com/49421109/57583626-2195c980-750d-11e9-9389-0675b24ae7ac.JPG)

다음과 같이 설치가 진행되고 완료되면 밑에 화면처럼 테마가 추가됨을 알 수 있다.
![51](https://user-images.githubusercontent.com/49421109/57583636-2fe3e580-750d-11e9-86c4-b207d9906128.JPG)

활성화 후 새로고침하면 다음과 같은 화면을 볼 수 있다.
![52](https://user-images.githubusercontent.com/49421109/57583637-31151280-750d-11e9-87e1-502233c63c84.JPG)



참조
https://swiftcoding.org/wp-config-file//wordpress FTP 우회 방법
https://kjcoder.tistory.com/tag/wordpress%20%EB%94%94%EB%A0%89%ED%84%B0%EB%A6%AC%EB%A5%BC%20%EC%83%9D%EC%84%B1%ED%95%A0%20%EC%88%98%20%EC%97%86%EC%8A%B5%EB%8B%88%EB%8B%A4 // wordpree 테마 설치를 위한 권한설정
https://studyforus.tistory.com/223 //루트 비밀번호 설정
