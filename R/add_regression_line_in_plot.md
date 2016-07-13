# Add a regression line into plot

R 에서는 lm 함수를 통해 선형 회귀 모델(Linear Regression)을 생성하고, 해당 내용을 plot한 경우에는 회귀 모델의 선이 출력되지 않고, model을 구축하기 위한 여러가지 plot들이 보여지게 된다.

Regression line 을 보고자 하는 경우 다음의 코드를 수행하면 된다.

```
plot(sorted_ss3_test_data$lin_spearman_coef, xlab="", ylab="", pch=2, cex=1.2, col="blue", cex.axis=1.5) # LR SCC Coef
points(sorted_ss3_test_data$trans_spearman_coef, pch=1, cex=1.2, col="red") # Trans SCC Coef

title(xlab="Class #", ylab="Spearman correlation coefficient",
      cex.lab=1.5)

abline(h=mean(sorted_ss3_test_data$lin_spearman_coef), lty=2, col='blue')
abline(h=mean(sorted_ss3_test_data$trans_spearman_coef), lty=1, col='red')

```

abline 함수가 plot을 통해 표현된 scatter plot에 regression line을 추가해 준다.
