# Test Independence of the errors

선형 회귀 모델을 쓰기에 앞서서 여러가지 가정이 존재함. 그중 하나가 각각의 에러가 변수들의 값에 대하여 독립적임을 가정할 수 있어야함.

많은 테스팅 기법으로 만족하고, 다음 코드와 같이 durbinWatsonTest 함수를 사용하여도 시험이 가능하다.

```
LR_total <- lm(bug ~ wmc + dit + noc + cbo + rfc + lcom + ca + ce
                 + ce + npm + lcom3 + loc + dam + moa + mfa + cam
                 + ic + cbm+ amc + max_cc, data=df)
dw_LR <- durbinWatsonTest(LR_total)
# 실제 논문의 실험에 사용된 코드입니다.
```
