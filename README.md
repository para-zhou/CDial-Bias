#  Towards Identifying Social Bias in Dialogue Systems

This repository contains detailed detailed description of the CDial-Bias Dataset.

This task aims to measure the social bias in dialogue scenario. Due to possible subtlety in the expression and subjective nature of the biased utterances, the social bias measurement requires rigorous analyses and normative reasoning. Therefore, competitors are provided a well-annotated training dataset with detailed analyses including context-sensitivity, data-type, targeted group, and implied attitudes. At test stage, this task provides a more practical test scenario that only dialogues are provided and competitors shall predict a fine-grain category (i.e. irrelevant, anti-bias, neutral, and biased) w.r.t. dialogue social bias.

**Authors:** Jingyan Zhou, Jiawen Deng, Fei Mi, Yitong Li, Yasheng Wang, Minlie Huang, Xin Jiang, Qun Liu, Helen M. Meng

## Detailed Dataset Descriptions and Baselines
http://arxiv.org/abs/2202.08011 (We refine the annotations and construct CDial-Bias Dataset 2.0. The statistics and baseline performances may differ to some extend.)

 
## Dataset

### Format
The Cdial-Bias Dataset 2.0 has follwoing entries.
<table>
   <tr>
      <th></th>
      <th>Explaination</th>
   </tr>
   <tr>
      <th>Q</th>
      <td>Dialogturn turn 1.</td>
   </tr> 
   <tr>
      <th>A</th>
      <td>Dialogturn turn 2. </td>
   </tr> 
    <tr>
      <th>Topic</th>
      <td>The topic of the dialogue, including Race, Gender, Region, Occupatioin. </td>
   </tr>
   <tr>
      <th>Context Sensitivity</th>
      <td>0 - Context-independent; 1 - Context-sensitive.</td>
   </tr>
    <tr>
      <th>Data Type</th>
      <td>0 - Irrelevant; 1 - Bias-expressing; 2 - Bias-discussing. </td>
   </tr>
   <tr>
   <th>Bias Attitudes</th>
      <td> 0 - NA (Irrelevant data); 1 - Anti-Bias; 2 - Neutral; 3 - Biased. </td>
   </tr>
   <tr>
   <th>Referrenced Groups</th>
      <td>Presented in freetext. Multiple groups are splited by '/'. </td>
   </tr>
</table>

### Statistics

<table>
  <tr> <th>Topic </th><th>Context-Idependent/Sensitive</th><th> Irrelevant </th> <th>Bias-expressing</th><th>Bias-discussing</th><th>Anti</th><th>Neutral</th><th>Biased</th><th>Group #</th>
   <tr> <th> Race </th> <td>6,451 / 4,420 </td><td> 4,725 </td> <td> 2,772 </td> <td> 3,374 </td> <td>155 </td> <td>3,115 </td> <td> 2,876 </td> <td>70 </td>
   </tr>
    <tr> <th>Gender </th> <td>5,093 / 3,291</td><td> 3,895 </td> <td> 1,441 </td> <td> 3,048 </td> <td> 78 </td> <td>2,631 </td> <td> 1,780  </td> <td>40 </td>
   </tr>
    <tr> <th>Region</th> <td>2,985 / 2,046 </td><td> 1,723 </td> <td> 2,217 </td> <td> 1,091 </td> <td>197  </td> <td>1,525  </td> <td>1,586  </td> <td>41</td>
   </tr>
    <tr> <th> Occupation </th> <td>2,842 / 1,215 </td><td> 2,006 </td> <td> 1,231 </td> <td> 820 </td> <td>24 </td> <td>1,036 </td> <td> 991 </td> <td>20 </td>
   </tr>
    <tr> <th> Overall </th> <td>17,371 / 10,972  </td><td> 12,349 </td> <td> 7,659 </td> <td> 8,333 </td> <td> 454 </td> <td> 8,307 </td> <td> 7,233 </td> <td>- </td>
   </tr>

</table>

The dataset is randomly shuffled and splited into training, validation, and testing data in the ratio of 8:1:1.

 
## Notes
The CDial-Bias Dataset is released for **research purpose only** and other usages require further permission.
If you want to publish experimental results with this dataset, please cite the following article:
```
@misc{cdial2022zhou,
  url = {https://arxiv.org/abs/2202.08011},
  author = {Zhou, Jingyan and Deng, Jiawen and Mi, Fei and Li, Yitong and Wang, Yasheng and Huang, Minlie and Jiang, Xin and Liu, Qun and Meng, Helen},
  title = {Towards Identifying Social Bias in Dialog Systems: Frame, Datasets, and Benchmarks},
  publisher = {arXiv},
  year = {2022}
}
```
Also, we held NLPCC 2022 Shared Task 7 based on the proposed resources, please see the task overview here:
```
@inproceedings{zhou2022overview,
  title={Overview of NLPCC 2022 Shared Task 7: Fine-Grained Dialogue Social Bias Measurement},
  author={Zhou, Jingyan and Mi, Fei and Meng, Helen and Deng, Jiawen},
  booktitle={CCF International Conference on Natural Language Processing and Chinese Computing},
  pages={342--350},
  year={2022},
  organization={Springer}
}
```
