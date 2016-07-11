# 데이터 프레임을 column name 기준으로 row 자르기

데이터 프레임의 데이터를 열 이름을 기준으로 자르고 싶을 때, 다음과 같은 코드를 사용한다.

```
data <- read.xlsx(...) # data : dataFrame
data.subset <- subset(data, colName == "name") # Data frame내의 열 이름이 'colName'의 항목중 값이 'name'인 행만 subset한 내용을 data.subset에 저장한다.
```
