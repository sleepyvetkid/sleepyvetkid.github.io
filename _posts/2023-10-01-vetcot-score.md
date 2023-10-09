---
title: Veterinary Committee on Trauma (VetCOT) Score
date: 2023-10-01 00:00:00 +1000
categories: [Emergency & Critical Care, Triage]
tags: [canine, feline, ecc, triage]     # TAG names should always be lowercase
---

## VetCOT score<sup>1</sup>

<pre style="text-align:center;background-color:rgba(0,0,0,0.05);padding:20px">
γ = 0.700473 + 0.342245 (<i>lactate</i>) − 3.89630 (<i>iCa</i>)
    + 1.42343 (<i>head trauma</i>) + 2.01600 (<i>spinal trauma</i>)
</pre>

where;

<p style="margin-left: 25px;">
γ represents the log of the odds ratio of the outcome (death or euthanasia),
</p>
<p style="margin-left: 25px;">
<i>lactate</i> is the plasma lactate concentration in mmol/L, obtained within 6 hours of admission,
</p>
<p style="margin-left: 25px;">
<i>iCa</i> is the blood ionized calcium concentration in mmol/L, obtained within 6 hours of admission,
</p>
<p style="margin-left: 25px;">
<i>head trauma</i> is the presence of head trauma (0 = no, 1 = yes), and
</p>
<p style="margin-left: 25px;">
<i>spina trauma</i> is the presence of spinal trauma (0 = no, 1 = yes).
</p>

<p>
Conversion into a risk probability percentage of mortality risk (from 0 to 1) can then be obtained by the following equation:
</p>

<pre style="font-size:medium;text-align:center;background-color:rgba(0,0,0,0.05)">
  <math display="block">
    <mrow>
      <mn>Risk of probability of mortality (VetCOT score)</mn>
      <mo>=</mo>
      <mfrac>
        <msup><mi>e</mi><mi>γ</mi></msup>
        <mrow><mn>1</mn><mo>+</mo><msup><mi>e</mi><mi>γ</mi></msup></mrow>
      </mfrac>
    </mrow>
  </math>
</pre>

## How to Use / Interpretation

Table 1. Varying mortality risk cutoffs of the VetCOT score and their associated sensitivity and specificity, and percentile of the patient population that would meet the cutoff. 

<table style="width:100%">
  <tr>
    <td style="width:25%;white-space:normal"><b>Risk probability cutoff</b></td>
    <td style="width:25%;white-space:normal"><b>Sensitivity (%)</b></td>
    <td style="width:25%;white-space:normal"><b>Specificity (%)</b></td>
    <td style="width:25%;white-space:normal"><b>Percentile of patients ≥ cutoff (%)</b></td>
  </tr>
  <tr>
    <td>0.5</td>
    <td>29.0</td>
    <td>98.0</td>
    <td>5.0</td>
  </tr>
  <tr>
    <td>0.25</td>
    <td>57.9</td>
    <td>94.2</td>
    <td>11.5</td>
  </tr>
  <tr>
    <td>0.1</td>
    <td>76.6</td>
    <td>82.0</td>
    <td>21.3</td>
  </tr>
  <tr>
    <td>0.05</td>
    <td>86.9</td>
    <td>62.3</td>
    <td>43.1</td>
  </tr>
</table>

<p>
A VetCOT score (mortality risk) cutoff of 0.05 is recommended for triage purposes, while a cutoff of 0.5 might be used to consider euthanasia given the guarded prognosis.
</p>

---

## Description

Developed in 2018 using the American College of Veterinary Emergency and Critical Care's (ACVECC) Veterinary Committee on Trauma (VetCOT) registry consisting of 9 emergency centres over several years, a large-scale retrospective cohort study of dogs with trauma (n=2802) was used to identify independent variables that were associated with mortality. In the end, a model was built using 4 variables (lactate, iCa, the presence of head or spinal trauma) to predict the likelihood of not surviving to discharge.

## Pros

- In the original study<sup>1</sup>, the VetCOT score had comparable discriminatory performance for mortality to the Animal Trauma Triage (ATT) scores (AUROC = 0.87 for both), but the VetCOT had better fit of the data (Hosmer–Lemeshow goodness-of-fit test, P=0.93) compared to the ATT.
- Easy to use, very objective measures.
- Mortality risk is directly calculated from the score.

## Cons
- Only one retrospective internal validation study was done. No external validation.
- Venous blood gas must be performed to obtain lactate and iCa<sup>2+</sup> values.
- Despite the high overall predictive performance, at a mortality risk of 50%, the VetCOT score has bad sensitivity (29%) but excellent specificity (98%).<sup>1</sup> At this score, it is extremely likely that the patient has a 50:50 chance of survival, but most patients with similarly guarded prognosis will not reach this score.

## Recommendations

It is still early days for this scoring system, and external prospective validation studies are lacking. However, the method of development and the large database from which it was derived were scientifically sound.

The VetCOT score may be helpful, but the veterinarian should not rely on it solely for prognosis.

## References

1. Chik C, Hayes GM, Menard J. Development of a veterinary trauma score (VetCOT) in canine trauma patients with performance evaluation and comparison to the animal trauma triage score: A VetCOT registry study. *J Vet Emerg Crit Care*. 2021;31(6):708-717. doi:10.1111/vec.13135