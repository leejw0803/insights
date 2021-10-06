### NestJs

express 기반으로 제작되었으며, node.js에 백엔드를 구성할 수 있도록 해준다.<br />
기본적으로 typescript를 지원하며, javascript로 어플리케이션을 작성하는 것도 가능하다.<br />
다른 node.js의 프레임워크에는 없는 구조를 가지고 있다.<br />
nest.js는 구조를 갖고 있고, 그 구조 덕분에 순서와 룰도 있어서 이를 따르기만 하면 큰 규모의 백엔드를 쉽게 만들 수 있다.(미리 셋팅된 여러 기능들을 제공하기 때문에 수동으로 생성하지 않아도 된다.)<br /><br />
node.js 어플리케이션을 빌드하는데 유용하며, 객체지향 프로그래밍(Object Oriented Programming)과 함수형 프로그래밍(Functional Programming), 함수 반응형 프로그래밍(Functional Reactive Programming)의 요소도 일부분 사용한다.<br /><br />

| 구분        | 설명                                                                                                   |
| ----------- | ------------------------------------------------------------------------------------------------------ |
| providers   | Nest injector 에 의해 인스턴스화되고 적어도 이 모듈에서 공유될 수 있는 제공자                          |
| controllers | 인스턴스화해야 하는 이 모듈에 정의된 컨트롤러 세트                                                     |
| imports     | 이 모듈에 필요한 공급자를 내보내는 가져온 모듈 목록                                                    |
| exports     | 그 하위 집합은 providers이 모듈에서 제공하며 이 모듈을 가져오는 다른 모듈에서 사용할 수 있어야 합니다. |

controllers -> 기본적인 라우트정보를 담는다.
providers -> service.ts 구체적인 로직을 가짐 : 기존 프로젝트의 ctrl 느낌

#### Ref

<a href="https://darrengwon.tistory.com/965">dotenv를 nest에서 안쓰는 이유</a>
