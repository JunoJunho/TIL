# Draw Pie Chart

R에서는 다양한 방식으로 데이터를 표현할 수 있음.
그 중 한가지 방법으로 파이 차트 (Pie chart)가 있으며, 주어진 그룹 데이터들이 어떻게 분포하고 있는지를 확인할 수 있음.

```
ds <- data.frame(labels = c("Group A", "Group B", "Group C")
      vales = c(2, 9, 12))
pie(ds$values, labels = ds$labels)
```
