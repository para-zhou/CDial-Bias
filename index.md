---
title: Test
layout: template
filename: index
--- 



### Test data
**Release of test data**: Test data is avaliable at  [link](https://drive.google.com/drive/folders/1_bi9yw3LccAj4wy9naWmCSNMGtCU3Fvk?usp=sharing).

**Format of test data**：The test data is a .csv file. Each entry is a two turn dialog: 
```
idx,q,a
1,turn 1, turn 2
2,turn 1, turn 2
...
```

### Submission guideline
**Time**: We will only evaluate the **latest** submission by following timeslots and update the [leaderboard](#Leaderboard) coordinately.

1. May 11, 23:59
2. May 14, 23:59
3. May 17, 23:59
4. **Final submision**: May 20, 23:59


**Submission link**: Please submit your result to [link](https://forms.gle/JzmZUwd4u9Fv4wgB9).

**Format of submitted file**: Please name your file as
```
teamid_teamname.csv
e.g. 00_BiasEval.csv

```
The result file should be a .csv file in the form of:
```
idx,q,a,label
1,turn 1, turn 2, label
2,turn 1, turn 2, label
...
```
The label should be integers ranging from 0 to 3: 0 - NA (Irrelevant data); 1 - Anti-Bias; 2 - Neutral; 3 - Biased.


### Support or Contact

Having trouble with submission? Please contact us at *zhoujyan@link.cuhk.edu.hk* or join the Wechat Group by adding *Zzzmm-Zzzmm*.
