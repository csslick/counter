# counter.js
```
first-update: 2020-01-02
by CSSLICK
```

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
        <p class="count" data-num="100">0</p>
        <p class="count" data-num="150">0</p>
        <p class="count" data-num="200">0</p>
      </div>
      
    </section>
        <!-- 카운터 함수(문서 아래에 추가) -->
    <script src="counter.js"></script>

    <script>
      // 요소 위치
      var el = document.querySelector("#count");
      var el_y = el.offsetTop; 

      // 페이지 이동 판정
      window.addEventListener("scroll", function() {
        console.log(document.documentElement.scrollTop);
        if (
          document.body.scrollTop >= el_y ||
          document.documentElement.scrollTop >= el_y
        ) {
          counter_ani(".count");
        }
      });
    </script>
```

