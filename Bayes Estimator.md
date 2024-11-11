The **Bayes Estimator** is a concept from **Bayesian statistics**. In simple terms, it's a way of estimating unknown quantities (mean or variance) based on prior knowledge and new data.
1. **Prior beliefs** (what we already know or assume about the parameter).
2. **New data** (the evidence we collect).

**Example:**
You want to estimate the **average height** of students in a school. You don't know the average height exactly, but you have some prior knowledge about the heights of people in general and a sample of student heights.

- **Prior Knowledge (Prior Distribution)**:
    - From previous studies or general knowledge, you believe that the average height of students is around **170 cm**.
    - You also believe that the standard deviation (spread of heights) is about **10 cm**.
    - Therefore, you model the average height with a **normal distribution** N(170,10)
- **New Data (Sample)**:
    - You measure the heights of 5 students and find that their average height is **168 cm** with a **standard deviation of 8 cm** in the sample.
    - The sample mean gives you new evidence that you will combine with your prior knowledge.

#### Goal:
Using the **Bayes Estimator**, we will combine our prior belief (the normal distribution N(170,10) with the new data (sample mean of 168 cm from 5 students) to estimate the **true average height** of students.

**Prior Distribution** P(μ) = N (170,10)
**Likelihood** P(x∣μ) = N(168,3.58)

- The sample standard deviation is 8 cm, but since the sample size is small (5 students), we need to adjust for the sample size when calculating the likelihood. The **standard error** of the sample mean is calculated as:

Standard Error=σ/sqrt(n)=8 / sqrt(5) ≈3.58 


![[Pasted image 20241108142544.png]]

**Find the Posterior Mean and Variance**:

The **posterior mean** is the **weighted average** of the prior mean and the sample mean, where the weights depend on the respective variances. The formula for the posterior mean is:
![[Pasted image 20241108142728.png]]

![[Pasted image 20241108142752.png]]

### Final Estimate:

Based on the **Bayes Estimator**:

- The **estimated average height** of students is about **168.8 cm**.
- The **uncertainty** about this estimate (posterior standard deviation) is **3.75 cm**.

#### Conclusion:

The **Bayes Estimator** combines prior knowledge (prior distribution) and new data (sample mean) to give you an updated, more informed estimate. In this example, our prior belief about the average height (170 cm) was adjusted based on the new data (168 cm), leading to a more accurate estimate of **168.8 cm** for the true average height of students.