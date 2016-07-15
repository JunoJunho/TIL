# Setting line thickness of abline

종종 논문을 쓰다 보면 regression line의 굵기가 너무 얇아서 잘 보이지 않는 경우가 발생함. 이런 경우 선의 굵기를 조절해서 선명하게 바꿀 수 있다.

```
abline(h=mean(sorted_ss3_test_data$lin_spearman_coef), lty = 2, col = 'blue', lwd = 2)
# 얻어온 데이터를 바탕으로 line type 2 (점선), 굵기(lwd) 2, 파란색의 선을 기존의 plot에 추가한다.
```
