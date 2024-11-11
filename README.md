# prophet-challenge
This project is my Module 8 challenge in the AI Bootcamp. It focuses on investigating whether there is a meaningful relationship between search traffic and stock prices.


## Dependencies
- **pandas** : Used for data analysis and manipulation.
- **prophet** : Used for forecasting patterns based on historical data.

## Project Details

- **Input Data:**
    - [MercadoLibre Data](https://static.bc-edx.com/ai/ail-v-1-0/m8/lms/datasets/google_hourly_search_trends.csv)

    - [Stock Price Data]("https://static.bc-edx.com/ai/ail-v-1-0/m8/lms/datasets/mercado_stock_price.csv)

## Project Structure

```bash
prophet-challenge
|__ README.md
|__ forecasting_net_prophet.ipynb
```

---

### Project Breakdown

- **Part 1: Find unusual patterns in hourly Google search traffic.**

    - We closely analyzed search traffic for May 2020, the month when MercadoLibre released its quarterly financial results. During this time, we observed that traffic increased by approximately 8.55% compared to the average monthly traffic.

- **Part 2: Mine the search traffic data for seasonality.**

Key questions and insights from the seasonality analysis:

- **Question:** Does search traffic peak at specific times of day, or is it relatively consistent?

    - **Answer**: Traffic generally increases from 8 a.m. to 11 p.m., with peak activity occurring in the evening.

- **Question:** Does search traffic spike on particular days of the week?

    - **Answer:** Traffic is highest at the start of the week, particularly from Monday to Wednesday, with lower levels observed over the weekend.

- **Question:** Does search traffic tend to increase during the winter holiday period (weeks 40–52)?

    - **Answer:** While traffic fluctuates, there is a slight upward trend, with more peaks than valleys, suggesting increased interest during the holiday season.


- **Part 3: Relate the search traffic to stock price patterns.**

In this part, we examined:

- Stock volatility and hourly stock returns.

- The relationship (or lack thereof) between lagged search traffic and stock returns.

**Observation:** We found minimal to no correlation between search traffic and stock price returns.

**Question:** What is the near-term forecast for MercadoLibre's popularity?

- **Answer:** The forecast suggests a stable trend with no significant changes, indicating that MercadoLibre’s popularity is expected to remain steady.

- **Part 4: Develop a Time Series Model with Prophet**

    Questions explored with the Prophet model:

    - **Question:**  What time of day exhibits the greatest popularity?
    **Answer**: Around Midnight

    - **Question:**  Which day of week gets the most search traffic?
    **Answer**: Tuesday

    - **Question:**  What's the lowest point for search traffic in the calendar year?
    **Answer**: October

---

## Installation

To run this project, ensure you have python installed (version 3.8 or higher). Follow these steps:

1. **Clone the repository**:

```bash
git clone https://github.com/veenauppalapati/prophet-challenge.git
```
2. **Navigate to the project directory:**

```bash
cd prophet-challenge
```

3. **Open the project folder in visual studio code**
```bash
code .
```
4. **Run the notebook**: Open and execute the code in `forecasting_net_prophet.ipynb` to explore and analyze the dataset.

### Alternative: Run in Google Colab

To run the notebook in Google Colab:

1. Go to [Google Colaboratory](https://colab.research.google.com/).
2. Click on the `Open Notebook` button.
3. In the left sidebar, go to the `Upload` tab.
4. Click `Browse` and select the `forecasting_net_prophet.ipynb` notebook from the downloaded project directory.
5. Run the code in the notebook.