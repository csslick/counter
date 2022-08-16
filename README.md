# counter.js
## Update
```
data-speed 속도 설정 옵션 추가
함수 사용법 단순화
```
```
Author: CSSLICK
```

## Demo 
https://csslick.github.io/counter/

## Usage 
```
  counter_ani(class name)
```

## Example
```
    <section id="count">
      <div class="text-box">
        <h1>Counter</h1>
        <!-- data-num에 숫자값 설정 -->
        <!-- data-speed 속도 설정(1 ~ 10, 높으면 느려짐) -->
        <p class="count" data-num="10" data-speed="10">0</p>
        <p class="count" data-num="70" data-speed="2">0</p>
        <p class="count" data-num="200" data-speed="1">0</p>
      </div>
    </section>
    
    <!-- 문서 아래에 추가 -->
    <script src="counter.js"></script>
    
    <script>
      // 설정 옵션: el - 요소명, offset - 카운트 시작 위치 조절
      playCount({
        el: '.count',
        offset: 300
      })
    </script>

```

