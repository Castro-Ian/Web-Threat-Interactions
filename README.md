## Web-threat-Interactions

This project aims to analyze web traffic data to identify and predict suspicious activities. The following steps are performed in the script:

1. **Load and Preprocess Data:**
   - Load the web traffic data from a CSV file CloudWatch_Traffic_Web_Attack.
   - Convert timestamp columns to datetime format.
   - Set the timestamp column as the index for time series analysis.
   - Remove duplicate rows and standardize text data.

2. **Visualize Web Traffic:**
   - Plot the amount of data transferred (bytes in and bytes out) over time to understand traffic patterns.

3. **Feature Engineering:**
   - Calculate the duration of each web interaction.
   - Standardize numerical features and encode categorical features for machine learning models.

4. **Correlation Analysis:**
   - Compute and visualize the correlation matrix for numerical features to understand relationships between variables.

5. **Detection Types by Country:**
   - Create a stacked bar chart to visualize the frequency of different detection types by country.

6. **Network Graph:**
   - Create and visualize a network graph to show interactions between source and destination IP addresses.

7. **Machine Learning Model:**
   - Encode detection types into binary labels (suspicious or not).
   - Split the data into training and testing sets.
   - Train a neural network model to predict suspicious activities.
   - Evaluate the model's performance and visualize the training history.

## Real-World Applications

This project demonstrates several real-world applications of data analysis and machine learning in cybersecurity:

- **Anomaly Detection:** By visualizing web traffic and computing correlations, security analysts can identify unusual patterns that may indicate malicious activity.
- **Threat Detection:** The trained machine learning model can predict whether a web interaction is suspicious, helping to automate threat detection processes.
- **Network Analysis:** The network graph visualization aids in understanding the relationships and interactions between different IP addresses, which can be crucial for identifying compromised nodes in a network.
- **Proactive Security Measures:** By continuously analyzing web traffic data and updating the machine learning model, organizations can proactively detect and mitigate potential security threats.

This project serves as a foundation for developing advanced cybersecurity solutions that leverage data science and machine learning to enhance the detection and prevention of cyber threats.
