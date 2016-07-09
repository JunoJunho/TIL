# NA Value Handling

R에서 올바르지 아니한 값을 N/A (Not-available)한 값으로 표기하며, 통계를 사용할 때, 리스트 안에 포함되면, 계산이 되지 않음. 이런 경우 N/A 값을 영향력이 부족한 값으로 교체가 필요.

```
df.data[is.na(df.data)] <- 0
# NA value to 0 replaced.
```
