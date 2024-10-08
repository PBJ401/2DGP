# Mushroom Run

## 게임의 간단한 소개
버섯 캐릭터가 달리며 장애물을 피하는 간단한 런 게임입니다. 플레이어는 장애물을 피하면서 가능한 한 오랫동안 달려야 합니다.

## 게임 컨셉 및 핵심 메카닉
- **컨셉**: 버섯 캐릭터가 달리며 장애물을 피하는 간단한 런 게임.
- **핵심 메카닉**:
  - **자동 달리기**: 캐릭터가 자동으로 앞으로 이동합니다.
  - **장애물 피하기**: 플레이어는 점프키를 눌러 캐릭터를 점프시키고 장애물을 피합니다.
  - **목표**: 가능한 한 오래 달리며, 장애물에 부딪히지 않고 기록을 세웁니다.

## 스크린샷 혹은 그림판으로 끄적인 이미지 포함

## 예상 게임 실행 흐름
1. **시작 화면**: "Start" 버튼을 눌러 게임을 시작합니다.
2. **게임 진행**: 캐릭터는 자동으로 달리며, 플레이어는 점프키를 눌러서 장애물을 점프해 피합니다.
3. **게임 오버**: 장애물에 부딪히면 게임이 종료되고, 기록이 표시됩니다.

## 개발 내용
### Scene의 종류 및 전환 규칙
- **시작 화면 (Scene 1)**: 게임을 시작할 수 있는 메뉴입니다.
- **게임 화면 (Scene 2)**: 장애물이 등장하고, 플레이어가 캐릭터를 조작하는 메인 게임 화면입니다.
- **게임 오버 화면 (Scene 3)**: 장애물에 부딪힌 후 게임 결과를 보여주는 화면입니다.

### 각 Scene에 등장하는 GameObject의 종류 및 구성, 상호작용
- **MushroomCharacter**: 플레이어가 점프 동작으로 조작하는 캐릭터입니다.
- **RunObject**: 플레이어가 점프하여 피해야 하는 장애물 (예: 바위, 나무 등)입니다.

### 모든 클래스에 대한 언급
- **MushroomCharacter**: 캐릭터의 이동 및 점프 동작을 처리합니다.
- **RunObject**: 장애물 생성 및 충돌 처리를 담당합니다.
- **GameController**: 게임의 흐름을 제어하고 씬 전환을 처리합니다.

### Controller 객체에 대한 언급
- **GameController**: 게임의 상태를 관리하고 씬을 전환하며 게임 오버 상태를 처리합니다.

