# Add a new row to a data frame

R에서 Data frame에 새로운 행(record)를 넣는 방법은 다음과 같이 할 수 있다.

```
newRow <- NULL
newRow <- data.frame(name=project_name,
                         trial=a,
                         lin_pearson_coef = pe1$r[2],
                         lin_pearson_p = pe1$P[2],
                         lin_spearman_coef = sp1$r[2],
                         lin_spearman_p = sp1$P[2],
                         lin_r2 = as.numeric(lr.r2),
                         lin_rmse = as.numeric(lr.rmse),
                         lin_mae = as.numeric(lr.mae),
                         mlp_pearson_coef = pe2$r[2],
                         mlp_pearson_p = pe2$P[2],
                         mlp_spearman_coef = sp2$r[2],
                         mlp_spearman_p = sp2$P[2],
                         mlp_r2 = as.numeric(mlpt.r2),
                         mlp_rmse = as.numeric(mlpt.rmse),
                         mlp_mae = as.numeric(mlpt.mae)
    )
results_df <- rbind(results_df, newRow)
```
