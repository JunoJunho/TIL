# String concatenation

R에서 스트링을 붙이는 방법은 파이썬과 같은 스크립트 언어와 같이 + 연산자를 통해서 간단하게 해결되지는 않습니다.

대신 R에서는 'paste' 라는 함수를 지원합니다.

```
str <- paste("###", "ABC", sep = "_")
print(str) # Output: '###_ABC'
```
