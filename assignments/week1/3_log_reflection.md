**CHECK (AI_USE_LOG.md equivalent)**
* AI Challenge: The AI noted that "staples" is subjective. It pointed out that comparing the "earliest" to "most recent" date ignores seasonal fluctuations.
* AI Alternative 1: What is the month-over-month inflation rate for food items? -> **Rejected.** The data dictionary only contains ['date', 'item', 'city', 'price', 'unit', 'data_label']. It does not contain a pre-calculated inflation rate variable.
* AI Alternative 2: How does the price of chicken correlate with fuel over time? -> **Rejected.** The dataset only covers 4 specific consumer goods; there is no `fuel` variable included in the data.
* AI Alternative 3: Which specific item experienced the highest standard deviation in price? -> **Accepted.** This can be calculated using the existing `price` and `item` variables.


The data can show recorded retail prices of 4 specific items across 12 specific dates to establish trends. However, it cannot tell us *why* prices changed (e.g., supply chain issues, tax changes), nor can it measure overall household purchasing power. The most tempting AI suggestion was analyzing the correlation between food and fuel prices. It makes economic sense, but I rejected it because the dataset focuses strictly on consumer goods and lacks macroeconomic indicators like fuel costs.
