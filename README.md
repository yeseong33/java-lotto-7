# 로또 발매기 기능 구현

> 간단한 로또 발매기를 구현한다.

---

## 📋 기능 목록

1. [README.md](README.md) 작성
2. 다음 순서 대로, 테스트 코드를 작성한다.
3. 지시사항을 출력한다.
4. 구입 금액을 입력 받는다.
5. 금액 만큼 로또를 발행한다.
6. 구매한 로또 개수 및 번호를 출력한다.
7. 당첨 번호를 입력 받는다.
8. 보너스 번호를 입력 받는다.
9. 당첨을 확인한다.
10. 당첨 통계를 출력한다.
11. 입력의 예외사항을 추가한다.
12. 코드 구조를 리팩터링한다.

---

## 🔍 세부 기능

| **기능** | **구현 세부사항** |
| --- | --- |
| 테스트 코드 작성 | - 모든 테스트가 실패 상태에서 시작 |
| 지시사항 출력 | - 사용자가 구매 금액을 입력하도록 메시지 출력 |
| 구입 금액 입력 | - 사용자로부터 구입 금액을 입력 받음<br> - 입력의 유효성 검증 |
| 입력 유효성 검증 | - 입력이 숫자이며 양의 정수인지 확인 |
| 로또 발행 | - 구입 금액에 맞는 수량의 로또 발행 |
| 로또 개수 및 번호 출력 | - 구매한 로또 개수 출력<br> - 각 로또 번호 출력 |
| 당첨 번호 입력 | - 당첨 번호 입력받고 유효성 검증 |
| 당첨 확인 | - 입력한 번호와 로또 당첨 여부 확인<br> - 총 수익률 계산 |
| 당첨 통계 출력 | - 당첨 통계를 출력 |
| 입력 예외사항 처리 | - 입력의 예외사항 처리 |
| 코드 리팩터링 | - 객체 지향적으로 코드 구조를 개선 |

---

## 🚫 예외 사항

### 구입 금액 예외
- **1000원 단위가 아님** : `1220`
- **숫자가 아님** : `천원`
- **음수 입력** : `-1999`
- **빈 입력** : `""`
- **0원 입력**
    - 결과 : 0개 로또 구매 가능

### 당첨 번호 입력 예외
- **빈 입력** : `""`, `"1, 2, , 5"`
- **숫자가 아닌 요소** : `"a, 1, 2"`, `"?, 1, 2"`
- **허용된 범위 외 숫자** : `65`
- **허용된 공백 포함** : `"    12    , 1"` (허용)

### 보너스 숫자 입력 예외
- **빈 입력** : `""`
- **숫자가 아님** : `"일"`
- **음수 입력** : `-2`
- **허용된 범위 외 숫자** : `65`

--- 

### 🔄 개발 과정 요약

- 초기 테스트 코드 작성 후, 모든 테스트가 실패해야 함.
- 입력과 유효성 검증을 반복하며 기능을 추가하고 테스트 진행.
- 입력 예외 사항을 처리한 뒤, 전체 코드를 객체 지향적으로 리팩터링.
