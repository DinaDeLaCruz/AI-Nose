# AI-Nose

Law enforcement has increasingly adopted electronic nose (e-nose) technology, a type of artificial "smell" detection
system, to bolster
security efforts against the illegal trafficking of explosives. While hardware advancements have received significant
attention, less focus has been placed on the development of robust classification and quantification models for these
prototypes.

This research project aims to address this gap by creating machine learning and deep learning models capable of
distinguishing explosive materials (including different types of gunpowder and TNT) from non-explosive substances.
Additionally, the models will predict the concentration of these materials. To achieve this, we
employed two linear techniques (Partial Least Squares and Logistic Regression) alongside two non-linear approaches
(Multilayer Perceptron Neural Network and Long Short-Term Memory network).

---

### Experiment Description

To assess the e-nose prototype's ability to identify and measure explosive substances, two separate databases were used.
Each database entry represents an experiment where the responses of six chemical sensors were recorded over a specific
time period.

<div style="margin: 0 auto; width: fit-content; text-align: center;">
    <img src="Files\Fig0.svg" style="height:20%;width:90%">
</div>

#### Table Summary:
<table style="font-size: 11px;text-align: center">
<thead>
  <tr>
    <th >Feature</th>
    <th >Database 1 (Low Concentration & Mixtures)</th>
    <th >Database 2 (High Concentration)</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td >Goal</td>
    <td >Assess e-nose performance for low explosive concentrations and complex mixtures.</td>
    <td >Evaluate e-nose's ability to predict explosives at higher concentrations.</td>
  </tr>
  <tr>
    <td >Substances</td>
    <td >TNT, Gunpowder, Alcohol (2ml), Toothpaste & Soap</td>
    <td >TNT, Gunpowder, Alcohol (1ml)</td>
  </tr>
  <tr>
    <td >Concentration range</td>
    <td >0.1g to 3g</td>
    <td >3g to 5g</td>
  </tr>
  <tr>
    <td >Total experiments</td>
    <td >142</td>
    <td >63</td>
  </tr>
  <tr>
    <td >Number of samples per experiment</td>
    <td >650</td>
    <td >1800</td>
  </tr>
  <tr>
    <td >Number of chemical sensors per experiment</td>
    <td >6</td>
    <td >6</td>
  </tr>
  <tr>
    <td >Sampling frequency per experiment</td>
    <td >1Hz</td>
    <td >10Hz</td>
  </tr>
  </tbody>
</table>

---

### Data preprocessing 

The quality of the training data will determine how effectively the machine learning algorithms can learn from it. Therefore, it is essential to examine and preprocess the data before the learning stage (Raschka & Mirjalili, 2017).

For this reason, the data from both database 1 and database 2 were first examined. A Python algorithm was then developed for the preprocessing of the training data. This algorithm consists of the following steps:

- Implementation of a filter
<div style="margin: 0 auto; width: fit-content; text-align: center;">
    <img src="Files\Fig1.svg" style="height:20%;width:90%">
</div>
- Baseline correction
<div style="margin: 0 auto; width: fit-content; text-align: center;">
    <img src="Files\Fig2.svg" style="height:20%;width:60%">
</div>
- Peak alignment
<div style="margin: 0 auto; width: fit-content; text-align: center;">
    <img src="Files\Fig3.svg" style="height:20%;width:90%">
</div>
- Sensor concatenation
<div style="margin: 0 auto; width: fit-content; text-align: center;">
    <img src="Files\Fig4.svg" style="height:20%;width:90%">
</div>
- Outlier detection and removal
<div style="margin: 0 auto; width: fit-content; text-align: center;">
    <img src="Files\Fig5.svg" style="height:20%;width:90%">
</div>

---

### Models

---

### User interface

<div style="margin: 0 auto; width: fit-content; text-align: center;">
    <img src="Files\HMI.png" style="height:20%;width:90%">
</div>
