2025-06-28
# [Level 0] 홀짝 구분하기
## 1. 문제 설명

자연수 n이 입력으로 주어졌을 때 만약 n이 짝수이면 "n is even"을, 홀수이면 "n is odd"를 출력하는 코드를 작성해 보세요.

## 2. 제한사항

1 ≤ n ≤ 1,000

## 3. 입출력 예

### 3-1. 입력 #1

`100`

### 3-2. 출력 #1

`100 is even`

### 3-3. 입력 #2

`1`

### 3-4. 출력 #2

`1 is odd`

## 4. 제공코드

```shell
const readline = require('readline');
const rl = readline.createInterface({
    input: process.stdin,
    output: process.stdout
});

let input = [];

rl.on('line', function (line) {
    input = line.split(' ');
}).on('close', function () {
    n = Number(input[0]);
});
```

## 5. 풀이코드

```shell
const readline = require('readline');
const rl = readline.createInterface({
    input: process.stdin,
    output: process.stdout
});

let input = [];

rl.on('line', function (line) {
    input = line.split(' ');
}).on('close', function () {
    let n = Number(input[0]);
    if (n % 2 === 0) {
        console.log(`${n} is even`);
    } else {
        console.log(`${n} is odd`);
    }
});
```

