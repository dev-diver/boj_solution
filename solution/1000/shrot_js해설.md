[문제 보기](https://www.acmicpc.net/problem/1000)

* 입력값을 반복사용 하는 경우에는 `process.stdin` 이 `fs.readFileSync` 보다 유리하다.

참고 - [Node JS 입력 코드](../../team_notes/node입력.md)

* `0<A,B<10` 이므로 split 없이 index로 두 문자를 가져올 수 있다.
* 가져온 문자는 서로 더할 수는 있지만 ASCII 값이므로, 96 (=48*2)을 빼준다.
* (각 숫자는 실제로 나타내는 값보다 ASCII 코드 값이 48 크다.)