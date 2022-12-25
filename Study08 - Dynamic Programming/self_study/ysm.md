# 알고리즘 스터디 8- 다이나믹 프로그래밍

- 하나의 문제는 단 한번만 풀도록 하는 알고리즘
- 정답을 구한 작은 문제를 어딘가 메모해놓는다
    
    → 중복 발생 방지
    
    → 메모이제이션 : 분할 정복과의 차이
    
- 재귀에 대한 최적화

## 구현방법

1. Bottom-up : 아래에서 부터 계산을 수행 하고 누적시켜서 전체 큰 문제를 해결하는 방식
2. Top-down : dp[0]의 기저 상태에서 출발하는 대신 dp[n]의 값을 찾기 위해 위에서 부터 바로 호출을 시작하여 dp[0]의 상태까지 내려간 다음 해당 결과 값을 재귀를 통해 전이시켜 재활용하는 방식

## DP 사용조건

1. 동일한 작은 문제들이 반복하여 나타나는 경우 사용
2. 부분문제의 최적 결과 값을 사용해 전체 문제의 최적 결과를 낼 수 있는 경우