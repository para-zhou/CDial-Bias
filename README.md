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

## Dataset

### Format
The Cdial-Bias Dataset has follwoing entries.
<table>
   <tr>
      <th></th>
      <th>Explaination</th>
   </tr>
   <tr>
      <th>q</th>
      <th>dialogturn turn 1 </th>
   </tr> 
   <tr>
      <th>a</th>
      <th>dialogturn turn 2 </th>
   </tr> 
    <tr>
      <th>topic</th>
      <th>The topic of the dialogue, including Race, Gender, Region, Occupatioin. </th>
   </tr>
   <tr>
      <td>Context Sensitivity</td>
      <td>0 - Context-independent; 1 - Context-sensitive</td>
   </tr>
    <tr>
      <td>Data Type</td>
      <td>0 - Irrelevant; 1 - Bias-expressing; 2 - Bias Discussing. </td>
   </tr>
   <tr>
   <td>Bias Attitudes</td>
      <td>1 - Anti-Bias; 2 - Neutral; 3 - Biased. </td>
   </tr>
   <tr>
   <td>Referrenced Groups</td>
      <td>Presented in freetext. Multiple groups are splited by '/'. </td>
   </tr>
</table>
### Statistics


## More Explainations and Baselines
http://arxiv.org/abs/2202.08011

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
