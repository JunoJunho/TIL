# Sort data

R에서 저장된 데이터를 정렬(sorting) 하기 위해서는 order method를 사용해서 데이터를 정렬 할 수 있습니다.

order 함수는 주어진 입력 데이터 셋에 대하여 정렬된 데이터의 인덱스를 리턴시켜줍니다.

```
test_data <- c(0, 2, 3, 5, 1)

print( test_data[order(test_data)] )
# 0 1 2 3 5

print( test_data[order(test_data, decreasing = TRUE)])
# 5 3 2 1 0
```
