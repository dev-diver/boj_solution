[문제 보기](https://www.acmicpc.net/problem/1001)
```
print(eval('+0-'.join(input())))
```
* `eval()` 을 이용하기 위하여 중간에 `-` 를 끼워넣는다.
* 그냥 끼워넣으면 공백때문에 `- -` 가 되어 `+` 가 되기 때문에 `+0-` 로 버퍼해준다.