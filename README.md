# android-omok-precourse
# 결과
<img src="https://github.com/user-attachments/assets/c443617c-5f11-4412-b543-ef37fa08567c" width="30%">

# 기능 목록
## 돌 두기
### 1. 돌 번갈아 가며 두기
- ImageView 클릭 시 돌이 있는지 없는지 확인한다.
- 돌이 없으면 둔다.
  - 턴이 짝수면(0, 2, 4, ...) 검정 돌을 둔다.
  - 턴이 홀수면(1, 3, 5, ...) 흰 돌을 둔다.
  - 
### 2. 승리 조건 검사하기
- 해당 돌이 승리 조건에 해당하는지 검사한다.
  - (row, column)
    - (0,1), (0,-1)
    - (1,0), (-1,0)
    - (1,1), (-1,-1)
    - (1,-1), (-1,1)
    - 8개의 방향을 각각 확인해서 연속된 돌의 개수를 센다.
  - 개수가 5개면 승리로 판정한다.
  - 6개인 경우도 승리로 판정한다.(장목)
- 종료 다이얼로그를 띄운다.
  - 게임 종료, 00 돌이 이겼습니다.

### 3. 무승부 검사하기
- 만약 오목판 모든 위치에 돌이 놓였는데 승리자가 없다면, 게임을 종료한다.
- 종료 다이얼로그를 띄운다.
  - 게임 종료, 무승부 입니다.
