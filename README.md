# BaseballGame

## 규칙설명
#### 1. 숫자 1부터 9까지 중복되지 않는 3개의 난수를 생성.
#### 2. 사용자한테서 숫자 3개를 입력받는다. (1부터 9까지 입력 가능, 중복 x)
#### 3. 생성된 난수와 입력받은 숫자를 비교한다.
#### 4. 숫자와 위치가 같을 경우 스트라이크 (Strike).
#### 5. 숫자는 같지만, 위치가 틀릴 경우 볼 (Ball).
#### 6. 못 맞췄을 경우 게임이 끝나지 않고 카운트가 증가함. (최대 10번)

## 코드
### 난수 생성
#### ● do~while문을 이용하여 무조건 한 번은 난수 생성 후 중복 확인.
#### ● 난수 생성을 하여 중복되지 않으면 그 값을 반환해줌.

![image](https://user-images.githubusercontent.com/93521099/173283498-74dc20b5-5d02-442a-a50a-fa34bd7688eb.png)

#### ● 넘겨받은 값을 배열에 저장.
#### ● 사용자가 입력한 값을 저장할 배열 생성.
![image](https://user-images.githubusercontent.com/93521099/173283733-9be7abb0-c907-489b-9e95-70dcaaf48a6f.png)
#### ● 중첩 do ~ while문을 이용하여 사용자의 입력값을 받음.
![image](https://user-images.githubusercontent.com/93521099/173283859-3b626bd9-f124-42bd-a2fc-88fe719e2661.png)
#### ●1부터 9까지의 숫자를 입력하였는지와 중복값을 입력했는지 확인.
#### ● 숫자값 확인이 끝난 후 첫 번째 do~while문 종료.
![image](https://user-images.githubusercontent.com/93521099/173284433-a65396b3-cb5c-4055-8f16-82ef80727aef.png)
#### ● 4번, 5번 규칙처럼 입력 값과 난수 값을 비교.
#### ● 3개다 맞췄을 경우 두 번째 do~while문 종료.
#### ● 몇번만에 맞췄는지 확인을 위해 count값을 반환해줌.
![image](https://user-images.githubusercontent.com/93521099/173289565-7de4d6a4-c243-47b5-98ab-08b2ce37e636.png)
#### ● args(아규먼트)에 값이 있을 경우 그 값으로 난수값을 대체.
#### ● args(아규먼트)에 값이 없을 경우 난수생성.
#### ● 게임이 끝난 후 반환된 count값이 result에 저장.
#### ● result값에 따라 등급이 정해짐.("최상", "보통", "하", "최하")
![image](https://user-images.githubusercontent.com/93521099/173284875-2ec11d3b-d0f9-4074-a44d-b8d003ecc6f0.png)
