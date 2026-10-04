# Multiple-Sclerosis-MoCA-Predictor
A lightweight web calculator that estimates the probability of cognitive
impairment in people with multiple sclerosis (MS) from the **raw MoCA score**
plus two demographic variables (**age** and **years of education**). These
are available in even the most basic clinical setting.


The underlying model and its validation are described in the accompanying
paper (see [Publication](#publication)).

---

## How to use

<table>
<tr>
<td width="50%" valign="middle">

1. Open the [web app](https://cognitivescreening4ms.dpdns.org/).
2. Enter **Age** (years), **Education** (years), and the **Raw MoCA score** (0–30).
3. Click **Predict**.

</td>
<td width="50%" valign="top">

<img width="916" height="301" alt="Screenshot of the app input section" src="https://github.com/user-attachments/assets/c7de2e83-0c29-4f58-87ac-31fbb792e731" />




</td>
</tr>
<tr>
<td width="50%" valign="middle">

**The calculator returns:**

- a binary label (**Impaired** / **Not impaired**), based on the model's
  decision threshold;
- the predicted **probability of belonging to the "Impaired" group**, shown
  against the distribution of probabilities in the validation sample.

The app displays a warning when an input falls outside the range covered by
the training data (age outside 30–65 years, education outside 7–18 years, or
a MoCA score at the ceiling of 30). Predictions for these inputs should be
read with extra caution.

</td>
<td width="50%" valign="top">

<img width="920" height="811" alt="Screenshot of the app results section" src="https://github.com/user-attachments/assets/647569fb-de2b-4f12-a0ef-6b9d8bc13a82" />

</td>
</tr>
</table>

## Publication

> **[PAPER TITLE — TBD]**
> [Author A], [Author B], ..., [Author N].
> *[Journal name — TBD]*, [Year]. DOI: [10.xxxx/xxxxx — TBD]

- Paper: [link to published article — TBD](#)

If you use this calculator or model in your work, please cite the paper above.

```bibtex
@article{TBD,
  title   = {[PAPER TITLE]},
  author  = {[Author A] and [Author B] and [Author N]},
  journal = {[Journal name]},
  year    = {[Year]},
  volume  = {[Volume]},
  pages   = {[Pages]},
  doi     = {[10.xxxx/xxxxx]}
}
```

## Disclaimer

This application is a research tool and **is not a medical device**. Do not
use it to make clinical decisions without oversight by qualified
professionals. Use it for research, or as clinical decision support where
appropriate.
