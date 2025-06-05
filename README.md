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

### 🫸🏻 Dataset
CharacteristicsValue1.xlsx

### 🕴 Interpretation

*At significance level α = 0.05*

1. When Paired T.Test is conducted, it is observed a significant difference in the attributes Width, Length, Thickness, Edgecondition. Therefore, it is resulted as 'Reject H₀'.However, in case of Time, there is no significant difference in data, the result is 'Failed to reject H₀'
2. When Two sample T.Test is conducted with equal and unequal variances, there is no significant difference observed in the attributes Width, Length, Thickness which resulted as 'Failed to reject H₀'. However, the data showed a significant difference in Time and EdgeCondition resulting it as 'Reject H₀'

*At significance level α = 0.01*

1. When Paired T.Test is conducted, it is observed that there is no significant difference in the attributes Width, Length, Thickness, Time. Therefore, it is resulted as 'Failed to Reject H₀'. However, in case of EdgeCondition, there is no significant difference in data, the result is 'Reject H₀'
2. When Two sample T.Test is conducted with equal and unequal variances, there is no significant difference observed in the attributes Width, Length, Thickness which resulted as 'Failed to reject H₀'. However, the data showed a significant difference in Time and EdgeCondition resulting it as 'Reject H₀'

*At significance level α = 0.1*

1. When Paired T.Test is conducted, it is observed that there is a significant difference in the attributes Width, Length, Thickness, Time, EdgeCondtion. Therefore, it is resulted as 'Reject H₀'
2. When Two sample T.Test is conducted with equal and unequal variances, there is a significant difference observed in the attributes Width, Length, Time, EdgeCondition which resulted as 'Reject H₀'. However, the data showed no significant difference in Thickness resulting it as 'Failed to Reject H₀'

Throughout the data interpretation, if we include or exclude incorrect Test items, it may result in occurence of either Type 1 error or Type 2 error which can be decided in later steps. Conversely, the p-value of the attributes during Paired T.Test determine that there is a moderate to very strong evidence where 'Reject H₀' is positive. However, during the Two sample T.Test, there is either weak evidence or no evidence due to which it is recommeded to choose 'Fail to Reject H₀' is positive. 

*Z-Test and Power of a test*

As the population data is huge, Z-test is conduced at the population level instead of sample level. Ultimately, the power of the test is failed as the probability of correctly rejecting the null hypothesis (H₀) when it is false is very low. Also, as the population is large, effect size is also large; hence, the lower power. So, we need to focus on improving the test design by choosing good quality of data.

*β-value*

The β value is the probability of failing to reject the null hypothesis H₀ (Type 2 error) when it is actually false. In our case, β > 0.3 which evidently shows that the test that we conducted is weak and it is underpowered resulting in the risk of overlooking real effects.  The reason is the population size which we considered for analysis is large. It is recommended to choose sample size of 30>n>70 line items. 
There is higher probability of the occurence of Type 2 error by the user.

*Margin of error*

Margin of Error is high because there exists high variability due to the selection of random values in the dataset. The users are overconfident in making decisions despite inconsistent data. 

---

## 👜 Excel functionalities used
- T.TEST()
- IF() condition
- NORM.S.INV()
- ABS()
- SQRT()
- COUNT()
- NORM.S.DIST()
- T.INV.2T()
- RAND()
- RANDBETWEEN()

---

## 👞 Requirements
- Microsoft Excel 2016 or later
- Intermediate concepts of Business Statistics, Data analysis

---

*Data will talk if you're willing to listen - Jim Bergeson*
