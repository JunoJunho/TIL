# Create Train and Test(validation) Data Set

Machine Learning에서 많이 사용되는 모델을 만들기 위한 training set과 만들어진 모델을 테스트 하기 위한 test set을 나누는 방법이다.

```
library(caret)

trainIndex <- createDataPartition(df, p=.9, list=F)
    df.train <- tmp_df[trainIndex, ]
    df.test <- tmp_df[-trainIndex, ]

```
