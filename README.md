# CaffeineProto
게임 카페인(가제)의 MVP 프로토타입을 구현한 저장소

---

### 프로토타입 구현 목적
> 카페인(가제)의 최소 요구사항 및 로직을 도출해내고, 해당 요구사항과 로직을 구현할 수 있는 C++과 UE4의 기능들을 마스터한다.

---

### 게임 요구사항
> 다양한 머신을 통해 손님이 원하는 커피를 제작, 제공하고 돈을 번다.

### Screen
- 화면은 **CafeView**와 **MahcineView**로 나누어진다.
- **CafeView**는 카페내부의 모습과 **Customer**들을 보여준다.
- **MahcineView**는 커피를 만드는 **Machine**들을 보여준다.

### Customer
- 손님은 자신이 원하는 **Coffee**를 가진다.
- 손님을 클릭하면 **CurrentCoffee**를 손님에게 제공한다.
- **Coffee**와 **CurrentCoffee**가 일치하면 손님은 **Money**를 지불한다.
- 손님은 **FSM**을 가지고 카페의 내부를 움직이거나 서있을 수 있다.

### Machine
- 머신은 머신마다 다른 **ProcessCoffee로직**을 가진다.
- 머신을 클릭하면 **ProcessCoffee로직**을 실행, **CurrentCoffee**를 변환한다.
