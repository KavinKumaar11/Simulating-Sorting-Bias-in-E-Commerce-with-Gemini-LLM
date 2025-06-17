# 🧠 AI-Simulated A/B Testing: The Impact of Sorting on Shopper Behavior

This project replicates and extends the findings of the academic paper _“Designing Product Lists for E-commerce: The Effects of Sorting on Consumer Decision Making”_ (Cai & Xu, 2008) using modern generative AI. By leveraging Google’s **Gemini Flash LLM**, we simulate how consumers behave under different product list sorting strategies (Ascending, Descending, and Random).

## 📌 Objective

Explore how **sorting order** affects consumer decision-making by:
- Generating **synthetic personas** with varied preferences.
- Presenting them with **sorted product lists** (digital cameras).
- Capturing which product they choose and why.
- Analyzing how sorting order **biases choices**, even when preferences are predefined.

## 💡 Key Concepts

- **RIQP**: Ratio of Importance of Quality to Price.
- **Satisficing Behavior**: Shoppers tend to settle for "good enough" choices.
- **Position Bias**: Early items in a list are disproportionately chosen.
- **Behavioral Drift**: Actual decisions deviate from stated preferences.

## 🧪 Methodology

- **Camera List Creation**: 9 synthetic digital cameras with quality scores and prices.
- **Persona Generation**: 90 AI-generated shoppers with varying budgets and sensitivities.
- **Prompted Simulation**: Gemini LLM chooses a product based on sorted product lists.
- **Behavioral Analysis**: Kruskal-Wallis tests, histogram visualizations, and inferred RIQP metrics to analyze decision patterns.

## 📊 Key Findings

- Sorting order **significantly influences** inferred preferences (p-value = 0.0007).
- Shoppers exhibit strong **top-down scanning bias**.
- Declared preferences often **diverge from actual behavior**.
- AI personas replicate real-world satisficing behavior under UI constraints.

## 🔧 Installation

Clone the repo and install dependencies:

```bash
git clone https://github.com/your-username/ai-sorting-abtest.git
cd ai-sorting-abtest
pip install -r requirements.txt
```
⚠️ Requires access to Google’s generativeai API and an API key (Gemini Flash 1.5 or later).

## 📁 File Structure

- `LLM_Sorting_Bias_Simulation` – Main Google Colab notebook containing the full simulation pipeline
- `requirements.txt` – All Python dependencies required to run the project
- `gemini_abtest_cameralist.csv` – CSV export of the generated camera product list
- `gemini_abtest_results.csv` – Final output of persona decisions and inferred behavioral metrics

## 🧠 Future Enhancements

- Introduce **price promotions** or **urgency signals** to simulate real-world marketing triggers
- Implement **multi-turn decision-making**, where personas revisit or compare products
- Extend the analysis by **comparing LLM behavior with actual e-commerce user logs**
- Build an interactive **Streamlit dashboard** for real-time persona simulation

## 📜 License

This project is licensed under the [MIT License](LICENSE).  
Feel free to fork, modify, or reuse with proper attribution.

---

**Author**: R.T.Kavin Kumaar
**Connect**: [LinkedIn](https://www.linkedin.com/in/rtkavinkumaar22/) | [GitHub](https://github.com/KavinKumaar11)
