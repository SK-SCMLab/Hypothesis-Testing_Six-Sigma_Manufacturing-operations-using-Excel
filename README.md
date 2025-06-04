# ⏳ Hypothesis-Testing_Six-Sigma_Manufacturing-operations-using-Excel (Error detection)
This repository contains case studies from real-world manufacturing environments, demonstrating how hypothesis testing can be applied to assess process changes, quality improvements, and machine performance using Excel. Each study includes the full hypothesis setup, test selection, and interpretation

--- 

## 💽 Hypothesis testing
Hypothesis testing is used to prove or disprove a theory or claim by comparing two or more samples or comparing a signel sample to a defined value
- Six Sigma methodologies produce significant improvements in average performance
- The product quality is independent of supplier
- The average cycle time for processing similar products is the same between two different facilities

*Benefits*
- Handle uncertainty in data
- Minimize subjectivity
- Question assumptions
- Manage decision error risk

*Steps involved in Hypothesis testing*
1. Determine what to compare and assume that there is no difference
2. Decide how much risk of being wrong is acceptable
3. Use data to calculate a test statistic
4. Compare the test statistic to a critical test statistic
5. Make a decision by comparing p-value to accepted risk value

| *Null Hypothesis* | *Alternative Hypothesis* |
|-------------------|--------------------------|
| 1. Represented as H₀ | 1. Represented as Hₐ |
| 2. Statement of no change or difference | 2. Statement of change or difference |
| 3. Cannot be proved, only rejected | 3. Challenges the null hypothesis |

- Null states that there is no difference in means (H₀: μₐ = μ₆)
- Alternative is stating there is a difference in means

| *Type 1 error* | *Type 2 error* |
|----------------|----------------|
| 1. Rejected a null hypothesis when it is true | 1. Accepting a null hypothesis when it is false |
| 2. False positive | 2. False negative |
| 3. Also known as 'Producers Risk' | 3. Also known as 'Consumers Risk' |
| 4. Significane level or α is the chance of committing Type 1 error | 4. β is the chance of committing a Type 2 error |
| 5. The value of α is 5% or 0.05 | 5. The value of β is 20% or 0.2 |
| 6. N.A | 6. Any experiment should have a less β value as possible |

---

## 🔮 Power of a test
- The probability of correctly rejecting the null hypothesis when it is false
- The complement to Type 2 error and represented as 1-β
- The probability of not committing a Type 2 error
- It helps in improving the advantages of hypothesis testing
- The highest value should be preferred when given a choice of tests

---

## 🛎 Confidence level
- The probability of correctly failing to reject the null hypothesis when it is true
- The complement to Type 1 error and represented as 1-α
- The probability of not committing a Type 1 error

---

## ☠️ Case Study: Hypothesis testing on the machine dimensions and the processing time
### 🤏 Objectives
- Effect of change in machine dimensions
- Error detection of the time and dimensional attributes
- Data quality check - Ensure the data is statistically significant or not
- Process control

### 🧜‍♂️ Interpretation
From the excel analysis: 
*At Significance level α =0.05*
