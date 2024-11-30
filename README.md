# Healthcare Screening Data Analysis

This project focuses on analyzing healthcare screening data, specifically measuring the percentage of members who received and did not receive screening, and providing insights based on the data. The project uses Power BI or another data analytics platform to perform calculations and visualize the results.

## Project Overview

The main goal of this project is to track and analyze screening data for healthcare members. It calculates the number of members who have received screening, the number who have not, and provides percentage breakdowns of each. Additionally, we calculate the total number of members eligible for screening.

![image](https://github.com/user-attachments/assets/f4f58f3b-5826-4daf-95e9-f2377c4df830)

### Key Measures

The following key measures are calculated and used throughout the analysis:

1. **% of Members Didn't Receive Screening**  
   Calculates the percentage of members who did not receive screening, based on the count of members who didn’t receive screening divided by the total members eligible for screening.

2. **% of Members Received Screening**  
   Calculates the percentage of members who received screening, based on the count of members who received screening divided by the total members eligible for screening.

3. **Count of Members Didn't Receive Screening**  
   Counts the number of members who did not receive screening, where the EBM Numerator equals 0.

4. **Count of Members Received Screening**  
   Counts the number of members who received screening, where the EBM Numerator equals 1.

5. **Members Didn't Receive Screening**  
   Concatenates the count of members who did not receive screening with the percentage of members who didn’t receive screening.

6. **Members Eligible for Screening**  
   Counts the number of members eligible for screening, where the EBM Denominator equals 1.

7. **Members Received Screening**  
   Concatenates the count of members who received screening with the percentage of members who received screening.

8. **Select Metric**  
   Provides a dynamic selection of metrics for reporting or visualization.

## Data Description

The dataset includes the following columns:

- **Member ID Encrypted**: A unique identifier for each member, stored in an encrypted format.
- **EBM Numerator**: A value indicating whether a member received screening (1) or not (0).
- **EBM Denominator**: A value indicating if the member is eligible for screening.
- **ORIG_PREFERRED_LANGUAGE**: The member's preferred language.
- **SRC_LANGUAGE**: The language source, possibly for mapping purposes.
- **ORIG_RACE**: The original race/ethnicity of the member.
- **SRC_RACE**: The source race/ethnicity for comparison or mapping.
- **Original Member Ethnicity**: Detailed ethnicity information of the member.
- **SRC_ETHNICITY**: The source ethnicity for mapping or comparison.
- **Zip (5-digit)**: The 5-digit ZIP code of the member.

## Measures Created

The following DAX measures were created to perform analysis on the dataset:

- **% of Members Didn't Receive Screening**
- **% of Members Received Screening**
- **Count of Members Didn't Receive Screening**
- **Count of Members Received Screening**
- **Members Didn't Receive Screening**
- **Members Eligible for Screening**
- **Members Received Screening**
- **Select Metric** (for dynamically selecting metrics)

## Setup

### Prerequisites

1. Power BI (or any other compatible analytics platform).
2. A dataset containing member screening data.

### Steps to Use

1. **Import the Dataset**: Import the dataset into Power BI.
2. **Create Measures**: Implement the DAX measures provided above.
3. **Visualize**: Create visualizations based on the key metrics.
4. **Analyze**: Use the dynamic metric selection to analyze the data and get insights.

## Contributing

Feel free to fork this repository and submit pull requests if you have suggestions or improvements to the code or analysis.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
