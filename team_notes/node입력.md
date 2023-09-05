## fs모듈

* 모범
```
const fs = require('fs')
const input = fs.readFileSync('/dev/stdin').toString.split('\n') /// repl.it에서는 dev/stdin 으로 디버깅
```
* Short Code
```
i=(reqires.readFileSync(0)+"").split`
`
```
## process 모듈
process.stdin.on('data',c=>{
    c.split(' )
})
### Short Code
* input이 한 글자인 경우, input을 여러번 사용하는 경우 process가 더 짧다.

## readline 모듈
* 숏코딩은 포기한 모듈. 백준에서 '/dev/stdin' 으로 읽어오는 경우 런타임 에러 난다고 겁줘서 한번씩 해보는 방법.
* 실제로 이것 때문에 에러난 적은 없었고, 나의 실수로 케이스에 따라 에러 나온 게 전부다.
```
const readline = require("readline")
const rl = readline.createInterface({
    input:process.stdin,
    output:process.stdout,
})
let input = []
rl.on("line", line=>{
    input.push(line)
}),on("close", ()=>{
    //알아서 줄 나눔 됨
    process.exit()
})
```