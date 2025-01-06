# A-Stochastic-Oscillator-Based-Market-Maker-for-the-Bristol-Stock-Exchange
Enhancing Profitability and Risk Management: A Stochastic Oscillator-Based Algorithmic Market Maker for the Bristol Stock Exchange
----------------------

**Purpose**

The purpose of this project is to design and implement a new Algorithmic Market Maker (AMM) within the Bristol Stock Exchange (BSE) simulation environment and evaluate its performance. The key objectives are as follows:

--------------------------------
**Algorithm Development:**

Create a new trading robot (AMM) with a clear and well-defined strategy, either by developing a novel algorithm or adapting existing ones such as GD, MGD, or GDX.
Ensure the algorithm operates efficiently within the BSE framework, leveraging the Limit Order Book (LOB) and Matching Engine mechanics.

--------------------------------
**Behavioral Analysis:**

Explore and analyze the behavior of the new AMM under varying market conditions using structured experiments.
Understand how the AMM interacts with other trading robots and how its behavior affects market dynamics.

--------------------------------
**Performance Evaluation:**

Use appropriate metrics (e.g., profitability, market efficiency, price stability) to measure the performance of the AMM.
Conduct comparative experiments to benchmark the AMM against existing trading robots (e.g., ZIP, ZIC, Sniper).

-------------------------------
**Statistical and Visual Analysis:**

Apply statistical methods (e.g., hypothesis testing) to validate the results of the experiments.
Use visualization tools (e.g., graphs, tables) to communicate insights about the AMM's performance and market impact.

------------------------------

**DATA:**

https://github.com/davecliff/BristolStockExchange


------------------------------

**Conclusion**


This study evaluates the performance of TraderMMM02, a newly designed algorithmic market maker implemented in the Bristol Stock Exchange (BSE) simulation environment. By utilizing the Stochastic Oscillator (KD Line) with a simplified 14-period calculation and integrating a loss function, MMM02 aims to optimize profitability and risk management. However, some design decisions and evaluation methods warrant further clarification.

The experimental results highlight that MMM02 generally outperforms the baseline model, TraderMMM01, across diverse market conditions. Statistical tests, including the Wilcoxon-Mann-Whitney U Test, confirm significant differences in profitability, with MMM02 achieving higher returns. The Mean Squared Error (MSE) was employed to measure profit performance, and residual profit distributions further support MMM02’s superiority in varying environments.

Nevertheless, certain limitations and feedback suggest areas for improvement:

Short-Term Nature of the Stochastic Oscillator:

The modification of the RSV calculation from the traditional 14-day window to using only the past 14 prices creates a highly short-term strategy, especially given the fast trading pace in BSE simulations (e.g., trades occurring within 10 seconds). This design decision lacks a clear justification and raises concerns about its applicability to real-world scenarios where price trends develop over longer periods.
Choice of MSE for Performance Evaluation:

While MSE provides a measure of average differences, it does not capture the directionality of profit changes. The residuals  hold informative value, as their signs indicate whether MMM02 or MMM01 performs better. Future evaluations could incorporate metrics that better reflect this directional aspect to provide a more nuanced understanding of relative performance.
In conclusion, MMM02 demonstrates strong performance in simulations, supported by statistical tests and visualization methods. However, the reliance on short-term strategies and the evaluation approach require refinement to improve the model's robustness and real-world applicability. Future research should focus on exploring longer-term or adaptive parameters for the KD Line and adopting evaluation metrics that account for profit directionality. These adjustments could enhance both the interpretability and effectiveness of the proposed algorithm in practical trading environments.
