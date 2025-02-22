## MVC 패턴, 의식하며 구현할 수 있도록 노력하자!

- Model은 Controller와 View에 의존하지 않아야 한다.
- View는 Model에만 의존해야 하고, Controller에는 의존하면 안 된다.
- View가 Model로부터 데이터를 받을 때는, 사용자마다 다르게 보여주어야 하는 데이터에 대해서만 받아야 한다.
- Controller는 Model과 View에 의존해도 된다.
- View가 Model로부터 데이터를 받을 때, 반드시 Controller에서 받아야 한다.

## < 기능 구현 목록 >

### User

- 사용자가 입력한 3자리수를 관리하는 클래스
- [x] 입력된 3자리수를 저장한다.

### Computer

- 랜덤한 3자리수를 관리하는 클래스
- [x] 랜덤하게 생성된 3자리수를 저장한다.

### Judgement

- 유저의 수와 컴퓨터의 수를 숫자야구 로직으로 판단하는 클래스
- [x] 스트라이크의 개수를 판단한다.
- [x] 볼의 개수를 판단한다.
- [x] 낫싱을 판단한다.
- [x] 스트라이크와 볼의 개수 혹은 낫싱을 반환한다.

### Random

- 랜덤한 3자리수를 생성하는 클래스
- [x] 랜덤하면서 서로 다른 3자리수를 생성한다.

### GameController

- 전체적인 숫자야구 게임의 흐름을 관리하는 클래스
- [x] 게임을 시작/재시작시키거나, 종료시킨다.

### InputView

- 유저의 입력을 받을 때 필요한 UI를 제공하는 클래스
- [x] 유저에게 서로 다른 3자리수를 입력 받는다.
- [x] 유저에게 재시작/종료에 대한 입력을 받는다.

### OutputView

- 유저에게 게임 진행 상황을 보여주기 위한 UI를 제공하는 클래스
- [x] 게임 시작에 대한 문구를 출력한다.
- [x] 게임 종료에 대한 문구를 출력한다.
- [x] 스트라이크와 볼의 개수 혹은 낫싱을 출력한다.

### InputException

- 입력된 값이 유효한지 확인하는 클래스
- [x] 서로 다른 3자리수인지 확인한다.
- [x] 게임 재시작/종료를 구분하는 숫자인지 확인한다.