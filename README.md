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
    <th style="font-size: 13px;text-align: center">Feature</th>
    <th style="font-size: 13px;text-align: center">Database 1 (Low Concentration & Mixtures)</th>
    <th style="font-size: 13px;text-align: center">Database 2 (High Concentration)</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td style="font-size: 11px;text-align: center">Goal</td>
    <td style="font-size: 11px;text-align: justify">Assess e-nose performance for low explosive concentrations and complex mixtures.</td>
    <td style="font-size: 11px;text-align: justify">Evaluate e-nose's ability to predict explosives at higher concentrations.</td>
  </tr>
  <tr>
    <td style="font-size: 11px;text-align: center">Substances</td>
    <td style="font-size: 11px;text-align: justify">TNT, Gunpowder, Alcohol (2ml), Toothpaste & Soap</td>
    <td style="font-size: 11px;text-align: justify">TNT, Gunpowder, Alcohol (1ml)</td>
  </tr>
  <tr>
    <td style="font-size: 11px;text-align: center">Concentration range</td>
    <td style="font-size: 11px;text-align: center">0.1g to 3g</td>
    <td style="font-size: 11px;text-align: center">3g to 5g</td>
  </tr>
  <tr>
    <td style="font-size: 11px;text-align: center">Total experiments</td>
    <td style="font-size: 11px;text-align: center">142</td>
    <td style="font-size: 11px;text-align: center">63</td>
  </tr>
  <tr>
    <td style="font-size: 11px;text-align: center">Number of samples per experiment</td>
    <td style="font-size: 11px;text-align: center">650</td>
    <td style="font-size: 11px;text-align: center">1800</td>
  </tr>
  <tr>
    <td style="font-size: 11px;text-align: center">Number of chemical sensors per experiment</td>
    <td style="font-size: 11px;text-align: center">6</td>
    <td style="font-size: 11px;text-align: center">6</td>
  </tr>
  <tr>
    <td style="font-size: 11px;text-align: center">Sampling frequency per experiment</td>
    <td style="font-size: 11px;text-align: center">1Hz</td>
    <td style="font-size: 11px;text-align: center">10Hz</td>
  </tr>
  </tbody>
</table>



