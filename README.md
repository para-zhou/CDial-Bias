#  NLPCC 2021 Shared Task 7 - Fine-Grain Dialogue Social Bias Measurement

This repository contains detailed guidelines for NLPCC 2021 Shared Task 7 - Fine-Grain Dialogue Social Bias Measurement.

This task aims to measure the social bias in dialogue scenario. Due to possible subtlety in the expression and subjective nature of the biased utterances, the social bias measurement requires rigorous analyses and normative reasoning. Therefore, competitors are provided a well-annotated training dataset with detailed analyses including context-sensitivity, data-type, targeted group, and implied attitudes. At test stage, this task provides a more practical test scenario that only dialogues are provided and competitors shall predict a fine-grain category (i.e. irrelevant, anti-bias, neutral, and biased) w.r.t. dialogue social bias.

**Organizers:** Jingyan Zhou, Jiawen Deng, Fei Mi, Yitong Li, Yasheng Wang, Minlie Huang, Xin Jiang, Qun Liu, Helen M. Meng

## Important Dates
* **April 6, 2022** Training data would be released by then.
* **May 5,2022** Registration deadline.
 

## Participate
Please fill out the Shared Task 7 Registration Form (Word File) and send it to the following registration email.
Registration Email: jyzhou@se.cuhk.edu.hk

## Detailed Dataset Descriptions and Baselines
http://arxiv.org/abs/2202.08011 (We refine the annotations and construct CDial-Bias Dataset 2.0 for this shared task. The statistics and baseline performances may differ to some extend.)

## Task
<table>
   <tr>
      <th>Goal</th>
      <td>measure the social bias in dialogue scenario. </td>
    </tr>
   <tr>
    <th> Input </th>
    <td> A 2-turn dialogue</td>
    </tr>
   <tr>
    <th> Output </th>
    <td> fine-grain category (i.e. 0 - irrelevant, 1 - anti-bias, 2 - neutral, and 3 - biased) w.r.t. dialogue social bias.</td>
   </tr>
 </table>
 
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
      <td>dialogturn turn 1 </td>
   </tr> 
   <tr>
      <th>A</th>
      <td>dialogturn turn 2 </td>
   </tr> 
    <tr>
      <th>Topic</th>
      <td>The topic of the dialogue, including Race, Gender, Region, Occupatioin. </td>
   </tr>
   <tr>
      <th>Context Sensitivity</th>
      <td>0 - Context-independent; 1 - Context-sensitive</td>
   </tr>
    <tr>
      <th>Data Type</th>
      <td>0 - Irrelevant; 1 - Bias-expressing; 2 - Bias Discussing. </td>
   </tr>
   <tr>
   <th>Bias Attitudes</th>
      <td> NA; 1 - Anti-Bias; 2 - Neutral; 3 - Biased. </td>
   </tr>
   <tr>
   <th>Referrenced Groups</th>
      <td>Presented in freetext. Multiple groups are splited by '/'. </td>
   </tr>
</table>
### Statistics
<table>
   <tr>
      <th>CDial-Bias-2.0</th>
 </tr>
  <tr> <th>Topic </th><th>Context-Idependent/Sensitive</th><th> Irrelevant </th> <th>Bias-expressing</th><th>Bias-discussing</th><th>Anti</th><th>Neutral</th><th>Biased</th><th>Group #</th>
   <tr> <th> Race </th> <th>6,451 / 4,420 </th><th> 4,725 </th> <th> 2,772 </th> <th> 3,374 </th> <th>155 </th> <th>3,115 </th> <th> 2,876 </th> <th>70 </th>
   </tr>
    <tr> <th>Gender </th> <th>5,093 / 3,291</th><th> 3,895 </th> <th> 1，441 </th> <th> 3,048 </th> <th> 78 </th> <th>2,631 </th> <th> 1,780  </th> <th>40 </th>
   </tr>
    <tr> <th>Region</th> <th>2,985 / 2,046 </th><th> 1,723 </th> <th> 2,217 </th> <th> 1,091 </th> <th>197  </th> <th>1,525  </th> <th>1,586  </th> <th>41</th>
   </tr>
    <tr> <th> Occupation </th> <th>2,842 / 1,215 </th><th> 2,006 </th> <th> 1,231 </th> <th> 820 </th> <th>24 </th> <th>1,036 </th> <th> 991 </th> <th>20 </th>
   </tr>
    <tr> <th> Overall </th> <th>17,371 / 10,972  </th><th> 12,349 </th> <th> 7,659 </th> <th> 8,333 </th> <th> 454 </th> <th> 8,307 </th> <th> 7,233 </th> <th>70 </th>
   </tr>
</table>

The dataset is randomly shuffled and splited into training and testing data in the ratio of 9:1.


 

## Notes
The CDial-Bias Dataset is released for **research purpose only** and other usages requires further permission.
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
