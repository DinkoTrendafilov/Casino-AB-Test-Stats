# 🎰 Gaming A/B Test Analyzer

A simple yet powerful Python script for analyzing A/B test results in the gaming and gambling industry. Performs statistical significance testing on conversion rates between two groups.

## 📊 What It Does

This tool helps you determine if changes in your game features, promotions, or interfaces actually make a statistically significant difference. It's perfect for:
- Testing new slot machine features
- Comparing different bonus offers
- Evaluating UI/UX changes in casino apps
- Analyzing conversion rates for different player groups

## 🔧 Requirements

```bash
pip install statsmodels numpy

🚀 How to Use

    Run the script:

bash

python gaming_ab_test_analyzer.py

    Enter your A/B test data:

text

Enter success of group A: 450
Enter total visitors of group A: 10000
Enter success of group B: 530
Enter total visitors of group B: 10000

    Get immediate results:

text

----------------------------------------------------------------
Results:
    Group A: 450 / 10,000 = 4.50%
    Group B: 530 / 10,000 = 5.30%
    Difference (B-A): +0.80%
----------------------------------------------------------------
Statistical Test:
    z-score = 2.5586
    p-value = 0.0105 --- 1.0510% | 1 From 95.1 trials
----------------------------------------------------------------
SIGNIFICANT! (p < 0.05)
     → Group B WINS by 0.80% points!
----------------------------------------------------------------

📈 Statistical Method

The script uses two-proportion z-test from statsmodels to calculate:

    Conversion rates for each group

    Absolute difference between groups

    z-score and p-value for statistical significance

    Interpretation at 95% confidence level (α = 0.05)


📋 Input Parameters
Parameter	Description
Group A Success	Number of successful events (conversions, wins, purchases)
Group A Visitors	Total number of visitors/players exposed
Group B Success	Same for the test/variation group
Group B Visitors	Total in the test group


📊 Output Interpretation
Significant Result (p < 0.05)

    Positive difference: Group B performs better

    Negative difference: Group A performs better

    Action: Implement the winning variation

Not Significant (p > 0.05)

    Difference could be due to random chance

    Action: Continue testing or revert to original

🎯 Use Cases in Gaming Industry

    Feature Testing

        Test new bonus game mechanics

        Compare different jackpot structures

    Marketing Optimization

        Evaluate promotional email campaigns

        Test different welcome bonus amounts

    UI/UX Improvements

        Compare different button placements

        Test color schemes for better engagement

    Monetization Testing

        Different pricing for in-game purchases

        Various subscription models

📦 Dependencies

    statsmodels - Statistical tests and models

    numpy - Numerical operations (usually installed with statsmodels)

🤝 Contributing

Feel free to fork and enhance! Some ideas:

    Add confidence interval calculations

    Include sample size calculator

    Add visualization of results

    Create web interface version

⚠️ Important Notes

    Results are valid only with proper random sampling

    Ensure adequate sample size before testing

    Consider practical significance alongside statistical significance

    Always follow responsible gambling guidelines

📄 License

MIT License - free for commercial and personal use.

👤 Author  -   Dinko Trendafilov


Created for data-driven decision making in gaming industry analytics.
