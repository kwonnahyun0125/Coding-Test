2025-06-28
# [Level 0] 문자열 붙여서 출력하기
## 1. 문제 설명

문자열 붙여서 출력하기기

## 2. 입출력 예

### 2-1. 입력 #1

`apple pen`

### 2-2. 출력 #1

`applepen`

### 2-3. 입력 #2

`Hello World!`

### 2-4. 출력 #2

`HelloWorld!`

## 3. 제공코드

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
    str1 = input[0];
    str2 = input[1];
});
```

## 4. 풀이코드

```shell
const readline = require('readline'); 
const rl = readline.createInterface({
    input: process.stdin,
    output: process.stdout
});

let input = [];

rl.on('line', function (line) {
    input = line.split(' ');
    rl.close(); // 입력이 한 줄이므로 바로 종료해줍니다.
}).on('close', function () {
    const str1 = input[0];
    const str2 = input[1];
    console.log(str1 + str2); // 두 문자열을 붙여서 출력
});
```


