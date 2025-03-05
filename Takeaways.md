# Own Progress
- Had a decently good pipeline
    - did xgboost with different folds
    - used ema lag sales (very important), ema zero sales (somewhat important) --> got ok score

- Things to improve on
    - iterated somewhat slowly (spent a full day trying to improve pipeline, spent a day getting split by store to work)
    - did not test many new features

    - did not know how robust predicts were to different time frames (only used last 28d val, and public lb to test)

# Other People's posts - takeaways
1. First place: uses recursive model (what is recursive??)
2. Uses some interesting stacking
- first predicts probability of item being bought
- uses multipliers (NBEATS to find what multipliers)

4. Simple LGBM models w/ features
- 40 models, 10 stores * 4 weeks
- used time series crossval (5 holdout sets)
- power of a simple, robust model (we could have done this)
