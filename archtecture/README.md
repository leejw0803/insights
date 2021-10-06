## MSA with Docker

### Docker

하나의 서버에 여러개의 컨테이너를 실행하면 서로 영향을 미치지 않고 독립적으로 실행되어 마치 가벼운 VMVirtual Machine을 사용하는 느낌을 줍니다. <br />
실행중인 컨테이너에 접속하여 명령어를 입력할 수 있고 apt-get이나 yum으로 패키지를 설치할 수 있으며 사용자도 추가하고 여러개의 프로세스를 백그라운드로 실행할 수도 있습니다. <br />
CPU나 메모리 사용량을 제한할 수 있고 호스트의 특정 포트와 연결하거나 호스트의 특정 디렉토리를 내부 디렉토리인 것처럼 사용할 수도 있습니다.<br /><br />

<b>이미지는 컨테이너 실행에 필요한 파일과 설정값등을 포함하고 있는 것</b>으로 상태값을 가지지 않고 변하지 않습니다(Immutable). <br />
컨테이너는 이미지를 실행한 상태라고 볼 수 있고 추가되거나 변하는 값은 컨테이너에 저장됩니다. <br />
같은 이미지에서 여러개의 컨테이너를 생성할 수 있고 컨테이너의 상태가 바뀌거나 컨테이너가 삭제되더라도 이미지는 변하지 않고 그대로 남아있습니다.<br /><br />

컨테이너의 생성은 기본적으로 ‘도커파일’이라는 것을 이용한다.<br />
가상화 할 프로그램들을 ‘도커파일’이란 DSL(Domain Specific Language)형태로 작성한다.<br />
컨테이너 생성과정은 다음과 같다.<br />
도커파일 -> (build) = 도커이미지 생성<br />
도커이미지 -> (run) = 도커컨테이너 생성<br />
도커 파일은 소스와 함께 버전관리도 된다.<br /><br />

### MSA

#### Ref. link

<a href="https://brunch.co.kr/@maengdev/3">마이크로 서비스 아키텍처와 개발문화</a> <br/>
<a href="https://subicura.com/2017/01/19/docker-guide-for-beginners-1.html">초보를 위한 도커 안내서</a> <br/>
<a href="https://pkh11.medium.com/docker-%EB%8F%84%EC%BB%A4%EB%9E%80-%EB%AC%B4%EC%97%87%EC%9D%B8%EA%B0%80-8b93d1a46aa8">도커란 무엇인가</a> <br/><br/>

<a href="https://www.44bits.io/ko/post/easy-deploy-with-docker">도커 입문편</a>