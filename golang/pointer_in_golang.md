# Create a struct type in golang

Go 언어에서는 포인터를 C언어와 같은 방식으로 사용할 수 있다.

```
var i int
i = 3
var ptr *int
ptr = &i # ptr도 i 의 메모리를 가리킨다.
fmt.Printf(*ptr) # 3
```

하지만, 포인터 연산은 Go언어에서 지원하지 않는다.

```
ptr++ # Not allowed
```
