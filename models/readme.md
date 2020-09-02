# Comparison class models

All models in this folder are written in the probabilistic programming language WebPPL [(webppl.org)](http://webppl.org). These models can be run on the command line if WebPPL is installed.

## Online walk-through

You can read about the vague adjective model and the comparison class inference model in [Chapter 5 of the problang.org textbook](http://www.problang.org/chapters/05-vagueness.html). This walk-through includes runnable code-boxes with WebPPL code that can be run in your browser (no installation required).

## One-off models

- `ccrsa.wppl`: Comparison class inference model (listener model), for use with comparison class inference experiment
- `adj-endorsement.wppl`: Adjective endorsement speaker model, for use with adjective endorsement

#### to run:

- `webppl ccrsa.wppl --require adjectiveRSA`
- `webppl adj-endorsement.wppl --require adjectiveRSA`

## Full Bayesian Treatment (BDA with RSA)

- *coming soon*

### Adjective RSA package

The `node_modules/adjectiveRSA` folder holds much of the shared code for use with `ccrsa` and `adj-endorsement`.

Contents:
  - `utils.wppl`: helper functions (e.g., `KL`, `round`)
  - `prior.wppl`: `statePrior` and various discretizations
  - `language.wppl`: `utterancePrior` and `thresholdPrior`
