¨Association rule: is an implication of the form

  X → Y where X is the antecedent and Y is the   consequent of the rule.

¨Ex: Basket analysis

¨People who buy/click/visit/enjoy X are also likely to buy/click/visit/enjoy Y.

¨A rule implies association, not necessarily causation.

An **association rule** has the form:

**{A} → {B}**

This means, if item **A** is purchased, then item **B** is likely to be purchased as well.
- **Support**: The proportion of transactions that contain both **A** and **B**.
- **Confidence**: The likelihood that **B** is purchased when **A** is purchased. It is calculated as:
- **Lift**: The increase in the probability of buying **B** when **A** is purchased, compared to the independent probability of buying **B**. 
![[Pasted image 20241112171256.png]]

## Example:

Imagine a retail store's transaction data contains the following transactions:

- Transaction 1: {Milk, Bread}
- Transaction 2: {Milk, Diapers, Beer}
- Transaction 3: {Bread, Diapers, Beer}
- Transaction 4: {Milk, Bread, Diapers, Beer}

#### Step 1: Calculate Support

Let’s calculate the support for different items and pairs of items:

- Support for **{Milk, Bread}** = 2 transactions out of 4, so **Support(Milk, Bread) = 0.5**.

#### Step 2: Calculate Confidence

Let’s calculate the confidence of the rule **Milk → Bread** (i.e., if a customer buys Milk, will they also buy Bread?):

- **Support(Milk, Bread) = 0.5**
- **Support(Milk) = 0.75** (Milk appears in 3 out of 4 transactions)
- Confidence(Milk → Bread) = 0.5 / 0.75 = **0.67**.

This means that 67% of the time when a customer buys Milk, they also buy Bread.

#### Step 3: Calculate Lift

Now, let’s calculate the lift for the rule **Milk → Bread**:

- **Support(Milk) = 0.75**
- **Support(Bread) = 0.75**
- Lift(Milk → Bread) = **Support(Milk, Bread) / (Support(Milk) * Support(Bread)) = 0.5 / (0.75 * 0.75) = 0.89**.

This indicates that the probability of buying Bread when buying Milk is only slightly greater than the independent probability of buying Bread.