
### Summary:
- Binary Classification task .
- Transactions count is small (len(*) <  285000) .
- F1 - F30 seems to be a result of some transformation (PCA ?).
- Some Values is null or NaN ,filled by feature mean value.
- Target class count is < 1% i.e. dataset highly imbalanced  <-- Key Point.
- Timestamp interval is  0 - 175000 ,max value is 172792 ~ 2 days (48 hours or 172800 sec)
- Zero correlation between F1 - F30 features

### Train RandomForestClassifier,CatBoostClassifier,XGBoost on:
- default data 
- under sampled data

- Default metric - ROC AUC
- Also explore most valuable features for alg

[Dataset](https://drive.google.com/file/d/1ayulWYHwWAHBbPF6UOTqhnAjYNonPmjY/view?usp=sharing)
