# 구현할 기능

### 구분자를 통해 피연산자 추출

- 구분자 확인 및 설정
    - 기본 구분자(” : “, “ , “)
    - 커스텀 구분자 Z(//Z\n)
- 사용자 입력에서 연산식 추출
- arg: userInput ( "//Z\n1:2,3Z4" )
- return: String[] [1, 2, 3, 4]

### 문자열 피연산자를 정수형으로 변환

- String[] 피연산자들을 Integer형태로 변환
- `예외 IllegalArgumentException`
    - 음수인 경우
    - 양의 정수가 아닌 경우(문자)
- arg: String[] [1, 2, 3, 4]
- return: List<Integer> [1, 2, 3, 4]

### 연산

- 덧셈 연산
- arg: List<Integer> [1, 2, 3, 4]
- return: int 10

### 사용자 입/출력

- 입력
  - 확인 사항: Scanner close시점 필요한지 확인
