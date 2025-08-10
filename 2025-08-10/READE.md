2025-07-27

# [Level 0] 공배수

## 1. 문제 설명

- 양의 정수 n이 매개변수로 주어질 때, n이 홀수라면 n 이하의 홀수인 모든 양의 정수의 합을 return 하고 n이 짝수라면 n 이하의 짝수인 모든 양의 정수의 제곱의 합을 return 하는 solution 함수를 작성해 주세요.



## 2. 제한사항

- 1 ≤ n ≤ 100

## 3. 입출력 예

|n | result |
|---|------|
|7|16|
|10|220|

### 입출력 예 설명

입출력 예 #1

- 예제 1번의 n은 7로 홀수입니다. 7 이하의 모든 양의 홀수는 1, 3, 5, 7이고 이들의 합인 1 + 3 + 5 + 7 = 16을 return 합니다.

입출력 예 #2

- 예제 2번의 n은 10으로 짝수입니다. 10 이하의 모든 양의 짝수는 2, 4, 6, 8, 10이고 이들의 제곱의 합인 22 + 42 + 62 + 82 + 102 = 4 + 16 + 36 + 64 + 100 = 220을 return 합니다.

## 4. 제공코드

```shell
function solution(n) {
    var answer = 0;
    return answer;
}
```

## 5. 풀이코드

```shell
function solution(n) {
    let answer = 0;
    
    // n이 홀수일 경우
    if (n % 2 !== 0) {
        for (let i = 1; i <= n; i += 2) {
            answer += i;
        }
    } 
    // n이 짝수일 경우
    else {
        for (let i = 2; i <= n; i += 2) {
            answer += i * i;
        }
    }

    return answer;
}
```
