# DoWell-Normality-test

Welcome to the Dowell Normality Test API documentation! Uncover the secrets hidden within your datasets with our powerful API that performs a rigorous normality test using the a combination of standard statistical test method. Whether you're a data enthusiast, researcher, or analyst, this API empowers you to understand the distribution characteristics of your data like never before.

## Features

The Dowell Normality Test API offers an array of features tailored to your data analysis needs:

1. **Precise Normality Assessment**: Curious about the normality of your dataset? Our API employs the Dowell method to precisely determine whether your data follows a normal distribution.

2. **Customizable Parameters**: Adjust key parameters like allowable error, individual deviation, and more to tailor the test to your dataset's unique characteristics.

3. **Comprehensive Analysis**: Dive into the nitty-gritty details! Get a comprehensive analysis of your dataset, including insights on normality status, curve alignment, slope deviations, and evidence counters. Obtain a comprehensive analysis of the normality test, including various metrics for each series in the dataset. Metrics include:
   - **Normality Status**: Indicates whether the dataset follows a normal distribution.
   - **Area Under the Curve (AUC) Z-Scores**: The area under the curve (AUC) Z-scores.The Z-score represents the number of standard deviations a data point is away from the mean.
   - **Actual Area**: The area under the dataset's probability density function curve.
   - **Rectangle Area**: The area under the histogram of the dataset. The total area under the normal distribution curve is equal to 1. Since the curve extends infinitely in both directions, it's not possible to compute the area for the entire curve.
   - **Individual Deviation**: An individual deviation in this context would refer to how much a single data point differs from the mean, in terms of standard deviations.A positive score indicates that the data point is above the mean, while a negative score indicates that the data point is below the mean.
   - **Kurtosis Classification**: Classification of the dataset's kurtosis (peakedness) as "Leptokurtic," "Platykurtic," or "Mesokurtic."
   - **Slopes and Slope Percentage Deviations**: Slopes of the cumulative distribution function and their deviation percentages.
   - **Evidence Counters**: Statistical checks for various features, including:
       - Mean equals to Median, with deviations considered.
       - Mean equals to Mode, with deviations considered for both.
       - Mode equals to Median.
       - Skewness equals to 0, with standard deviation deviation considered.
       - Kurtosis curve alignment.
       - Points in Range1, Range2, and Range3 checks.
       - Satisfies sigmoid function whose mirror image will give a bell-shaped curve.
       - Rotational Symmetry check.
`
## Authentication

This API does requires authentication for access.

# Getting started

**Step 1: Obtain the API key**

Before diving into the API integration, make sure that you have the necessary API key. You can generate your API key through the [DoWell API Key](https://ll05-ai-dowell.github.io/100105-DowellApiKeySystem/) Software

**Step 2: Set the base URL**

To make requests to the API, set the base url as `https://100023.pythonanywhere.com/public`

**Syep 3: Structure Your Requests**

Craft your API requests by refering to the guidelines mentioned in the [Postman Documentation](https://documenter.getpostman.com/view/24860974/2s9Y5YRN6r)

**Step 4: Handle Errors Gracefully**
The API follows standard HTTP status codes for error handling. Be sure to implement error handling in your code to gracefully manage potential errors and informative error messages.

**Step 5: Parse API Responses**
When you receive a response from the API, ensure you parse the data accurately to extract the relevant information you need.

## Error Handling

The API may return the following error responses:

- `400 Bad Request`: If the request payload is invalid or missing required fields.
- `500 Internal Server Error`: If an unexpected error occurs during the calculation process.

## Conclusion

The Dowell Normality Test API offers a powerful tool to assess the normality of datasets. It provides customizable parameters and detailed analysis, enabling you to gain valuable insights into the distribution of your data. To explore the API's capabilities, including endpoint testing and real-world examples, please visit our [Postman Documentation](https://documenter.getpostman.com/view/24860974/2s9Y5YRN6r).

If you have any further questions or need assistance, please don't hesitate to contact our support team. We are here to help you make the most of the API service.
