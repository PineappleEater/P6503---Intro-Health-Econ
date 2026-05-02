# Health Economics -- Assignment 4

**Name:** Xuange Liang  
**UNI:** xl3493

## 1. Design a Simple CEA

### 1a. Perspective
I would use a **health care payer perspective**. A national health technology assessment agency usually decides whether the health system should pay for the drug, so it mainly cares about costs borne by the insurer or government. That makes the payer perspective the most relevant for this decision.

### 1b. Time horizon
I would use a **lifetime time horizon**. Drug X may affect both survival and quality of life beyond the trial period, so a short horizon could miss part of its benefits and later costs. A lifetime horizon is more appropriate for capturing the full value of treatment.

### 2a. Comparator
The comparator should be **standard chemotherapy as the current active standard of care**. In a cost-effectiveness analysis, the main question is whether Drug X improves on what patients already receive in practice. A placebo comparator would be less realistic and could overstate the incremental benefit.

### 2b. Outcome type
My primary outcome would be **QALYs**. For metastatic breast cancer, treatment can change both length of life and quality of life, so QALYs are more informative than life-years alone. They are also the standard outcome used in many HTA decisions.

### 3a. Total QALYs for Drug X
\[
\text{QALYs}_{Drug X} = (3 \times 0.75) + (2 \times 0.50) = 2.25 + 1.00 = 3.25
\]

**Answer:** **3.25 QALYs**

### 3b. Total QALYs for comparator
\[
\text{QALYs}_{Comp} = 4 \times 0.60 = 2.40
\]

**Answer:** **2.40 QALYs**

### 3c. Incremental QALYs
\[
\Delta \text{QALYs} = 3.25 - 2.40 = 0.85
\]

**Answer:** **0.85 QALYs**

**Interpretation:** Drug X generates **0.85 additional QALYs per patient** relative to standard chemotherapy.

## 2. Base-Case ICER and Discounting

### 1a. Incremental cost
\[
\Delta C = \$200{,}000 - \$120{,}000 = \$80{,}000
\]

**Answer:** **\$80,000**

### 1b. Base-case ICER
\[
ICER = \frac{\Delta C}{\Delta E} = \frac{\$80{,}000}{0.85} = \$94{,}117.65 \text{ per QALY}
\]

**Answer:** **\$94,117.65 per QALY**

### 1c. Is Drug X cost-effective at \$100,000 per QALY?
**Yes.** Drug X is cost-effective in the base case because its ICER of **\$94,117.65 per QALY** is below the **\$100,000 per QALY** willingness-to-pay threshold.

### 2a. Present value formula for 1 QALY 30 years from now
\[
PV = \frac{1}{(1+0.03)^{30}}
\]

### 2b. Numerical present value
\[
PV = \frac{1}{(1.03)^{30}} \approx 0.41
\]

**Answer:** **0.41 QALYs**

### 2c. Discounting and the prevention paradox
Discounting reduces the weight placed on health gains that occur far in the future. As a result, preventive or long-horizon interventions can look less cost-effective even when they generate large total benefits. This is related to the prevention paradox because important population health gains may be undervalued when they arrive later.

## 3. Obesity Case: ICERs and Frontier

### 1a. Ordering by QALYs
The strategies are already correctly ordered from least to most effective:

- A: 6.20 QALYs
- B: 6.50 QALYs
- C: 6.65 QALYs
- D: 7.40 QALYs

### 1b. Incremental ICERs

**B vs A**

\[
\Delta C = \$18{,}000 - \$12{,}000 = \$6{,}000
\]
\[
\Delta E = 6.50 - 6.20 = 0.30
\]
\[
ICER = \frac{\$6{,}000}{0.30} = \$20{,}000 \text{ per QALY}
\]

**Answer:** **\$20,000 per QALY**

**C vs B**

\[
\Delta C = \$28{,}000 - \$18{,}000 = \$10{,}000
\]
\[
\Delta E = 6.65 - 6.50 = 0.15
\]
\[
ICER = \frac{\$10{,}000}{0.15} \approx \$66{,}666.67 \text{ per QALY}
\]

**Answer:** **\$66,666.67 per QALY**

**D vs C**

\[
\Delta C = \$95{,}000 - \$28{,}000 = \$67{,}000
\]
\[
\Delta E = 7.40 - 6.65 = 0.75
\]
\[
ICER = \frac{\$67{,}000}{0.75} \approx \$89{,}333.33 \text{ per QALY}
\]

**Answer:** **\$89,333.33 per QALY**

### 2a. Strict dominance
**No.** None of the strategies is strictly dominated because no strategy has both higher cost and lower QALYs than another strategy.

### 2b. Extended dominance and frontier
Compute **D vs B** directly:

\[
\Delta C = \$95{,}000 - \$18{,}000 = \$77{,}000
\]
\[
\Delta E = 7.40 - 6.50 = 0.90
\]
\[
ICER = \frac{\$77{,}000}{0.90} \approx \$85{,}555.56 \text{ per QALY}
\]

Because the ICER of **C vs B** is **\$66,666.67/QALY**, which is **lower** than the direct ICER of **D vs B** at **\$85,555.56/QALY**, **C is not extended-dominated**. Therefore, **C remains on the efficient frontier**, and the frontier is **A-B-C-D**.

## 4. Threshold-Based Decisions and Equity

### 1a. Threshold = \$50,000 per QALY
At **\$50,000/QALY**, the preferred strategy is **B: Lifestyle counseling**. Its ICER relative to A is only **\$20,000/QALY**, which is below the threshold, while the next incremental step, **C vs B**, costs **\$66,666.67/QALY**, which is above the threshold.

### 1b. Threshold = \$100,000 per QALY
At **\$100,000/QALY**, the preferred frontier strategy is **D: Branded GLP-1 agonist**. All frontier ICERs (**\$20,000**, **\$66,666.67**, and **\$89,333.33** per QALY) are below the threshold, so the most effective strategy on the frontier should be chosen.

### 1c. Threshold = \$3,000 per QALY
At **\$3,000/QALY**, **none of the active interventions** is cost-effective. Even the least expensive improvement, **B vs A**, has an ICER of **\$20,000/QALY**, which is well above the threshold, so **A: No intervention** would be chosen.

### 2. Equity and global thresholds
These results show that cost-effectiveness depends heavily on local budget constraints. A strategy that looks acceptable in a high-income country may be unaffordable in a low-income country, even when the health need is the same. That creates an equity problem because access to effective care depends partly on national income. GDP-per-capita-based thresholds try to reflect affordability, but they can also reinforce these global differences.

## 5. PrEP Case: Trial vs Real-World ICERs

### 1a. Trial data: ICER for B vs A
\[
ICER_{B vs A} = \frac{\$8{,}000{,}000 - 0}{180 - 0} = \frac{\$8{,}000{,}000}{180} \approx \$44{,}444.44 \text{ per QALY}
\]

**Answer:** **\$44,444.44 per QALY**

### 1b. Trial data: ICER for C vs B
\[
ICER_{C vs B} = \frac{\$28{,}000{,}000 - \$8{,}000{,}000}{210 - 180} = \frac{\$20{,}000{,}000}{30} \approx \$666{,}666.67 \text{ per QALY}
\]

**Answer:** **\$666,666.67 per QALY**

### 1c. Preferred strategy at \$100,000 per QALY under trial assumptions
The preferred strategy is **B: Daily oral TDF/FTC**. It is cost-effective relative to no PrEP at about **\$44,444.44/QALY**, while moving from B to C costs about **\$666,666.67/QALY**, far above the threshold.

### 2a. Real-world data: ICERs

**B vs A**

\[
ICER_{B vs A} = \frac{\$6{,}000{,}000 - 0}{105 - 0} = \frac{\$6{,}000{,}000}{105} \approx \$57{,}142.86 \text{ per QALY}
\]

**Answer:** **\$57,142.86 per QALY**

**C vs B**

\[
ICER_{C vs B} = \frac{\$27{,}000{,}000 - \$6{,}000{,}000}{200 - 105} = \frac{\$21{,}000{,}000}{95} \approx \$221{,}052.63 \text{ per QALY}
\]

**Answer:** **\$221,052.63 per QALY**

**C vs A**

\[
ICER_{C vs A} = \frac{\$27{,}000{,}000 - 0}{200 - 0} = \frac{\$27{,}000{,}000}{200} = \$135{,}000 \text{ per QALY}
\]

**Answer:** **\$135,000 per QALY**

### 2b. Preferred national strategy under real-world effectiveness
At a threshold of **\$50,000/QALY**, I would choose **A: No PrEP**, because **B vs A** already costs about **\$57,142.86/QALY**, which is above the threshold. At a threshold of **\$150,000/QALY**, I would choose **B: Daily oral PrEP**, because it is cost-effective relative to A, while moving from B to C still costs about **\$221,052.63/QALY**. Even though **C vs A** is **\$135,000/QALY**, the incremental rule still favors B over C.
