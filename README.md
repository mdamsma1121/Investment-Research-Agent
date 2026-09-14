# Investment-Research-Agent

## Features

* **Orchestrator Agent:** Dynamically routes ticker symbols to specialized sub-agents and synthesizes conflicting signals into a cohesive investment recommendation.
* **Fundamental Agent:** Programmatically extracts financial statement data via the Wisesheets API and populates custom Discounted Cash Flow (DCF) valuation templates.
* **Technical Agent** Generates price action, volume, and momentum charts using Matplotlib and Seaborn, leveraging Claude's vision capabilities for autonomous pattern recognition.
* **Sentiment Agent** Aggregates and scores qualitative data from news sentiment and corporate filings.
* **Interactive UI:** A Streamlit-based web interface for querying tickers and viewing the generated research reports and visualizations.

## System Architecture

1. **User Input:** Ticker symbol entered via the Streamlit frontend.
2. **Orchestrator:** Formulates a step-by-step research plan and triggers parallel workers.
3. **Sub-Agents:**
   * *Fundamental:* Retrieves Wisesheets data → Executes custom DCF model.
   * *Technical:* Plots Seaborn/Matplotlib charts → Triggers vision model analysis.
   * *Sentiment:* Parses external news and SEC filings.
4. **Synthesis Hub:** Aggregates quantitative, visual, and qualitative data.
5. **Output:** Comprehensive equity research report displayed in the UI.
<img width="1416" height="868" alt="image" src="https://github.com/user-attachments/assets/fca94480-a037-495b-8957-5eb1f6d2275d" />
