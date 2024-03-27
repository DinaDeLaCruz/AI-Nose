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
    <img src="Files\Fig1.svg" style="height:20%;width:90%">
</div>

#### Table Summary:
<table>
<thead>
  <tr>
    <th style="font-size: 13px;">Feature</th>
    <th style="font-size: 13px;">Database 1 (Low Concentration & Mixtures)</th>
    <th style="font-size: 13px;">Database 2 (High Concentration)</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td style="font-size: 12px;">Goal</td>
    <td style="font-size: 12px;">Assess e-nose performance for low explosive concentrations and complex mixtures.</td>
    <td style="font-size: 12px;">Evaluate e-nose's ability to predict explosives at higher concentrations.</td>
  </tr>
  <tr>
    <td style="font-size: 12px;">Substances</td>
    <td style="font-size: 12px;">TNT, Gunpowder, Alcohol (2ml), Toothpaste & Soap</td>
    <td style="font-size: 12px;">TNT, Gunpowder, Alcohol (1ml)</td>
  </tr>
  <tr>
    <td style="font-size: 12px;">Concentration range</td>
    <td style="font-size: 12px;">0.1g to 3g</td>
    <td style="font-size: 12px;">3g to 5g</td>
  </tr>
  <tr>
    <td style="font-size: 12px;">Total experiments</td>
    <td style="font-size: 12px;">142</td>
    <td style="font-size: 12px;">63</td>
  </tr>
  <tr>
    <td style="font-size: 12px;">Number of samples per experiment</td>
    <td style="font-size: 12px;">650</td>
    <td style="font-size: 12px;">1800</td>
  </tr>
  <tr>
    <td style="font-size: 12px;">Number of chemical sensors per experiment</td>
    <td style="font-size: 12px;">6</td>
    <td style="font-size: 12px;">6</td>
  </tr>
  <tr>
    <td style="font-size: 12px;">Sampling frequency per experiment</td>
    <td style="font-size: 12px;">1Hz</td>
    <td style="font-size: 12px;">10Hz</td>
  </tr>
  </tbody>
</table>



