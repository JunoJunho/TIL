# Create a struct type in golang

Go 언어에서 C 언어와 같은 사용자 정의 구조체를 만드는 방법은 다음과 같이 할 수 있다.

```
type node struct {
	data int
	next *node // 자기참조 구조체
}
```
