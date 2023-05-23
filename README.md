# Delivery Cost Analysis and Billing Discrepancy Detection System for E-commerce Companies

## Abstract
The Delivery Cost Analysis and Billing Discrepancy Detection System aims to optimize shipping operations for e-commerce companies. The system analyzes the delivery costs and detects any discrepancies in the billing by comparing the expected charges with the billed charges from courier companies. By identifying patterns and factors contributing to these discrepancies, the system helps reduce the difference between expected and billed charges, ultimately minimizing operational costs and enhancing customer satisfaction.

## Problem Statement
E-commerce companies face the challenge of optimizing shipping operations and ensuring accurate billing from courier companies. The goal of this project is to develop a system that analyzes the discrepancies between the expected shipping charges and the charges billed by the courier company. By understanding the factors that contribute to these discrepancies, the system aims to reduce the difference between the expected and billed charges, while maintaining high customer satisfaction and minimizing operational costs.

## Conclusion
The analysis performed in this project reveals a significant difference between the expected charges based on weight slots and the actual charges billed by the courier company. This discrepancy may arise from factors such as incorrect weight measurement and misclassification of delivery zones. By identifying these issues, e-commerce companies can negotiate better rates with courier companies, optimize their shipping costs, and ensure accurate billing.

## Overview
This project focuses on analyzing delivery costs and detecting billing discrepancies in the context of an e-commerce company. The project involves merging and analyzing five different datasets, including website order reports, warehouse pincode mapping, SKU master data, courier company invoices, and courier charges rate cards. By comparing the expected charges as per the company's weight slots with the charges billed by the courier company, the system provides insights into the weight slabs, delivery zones, expected charges, billed charges, and the difference between expected and billed charges.

## Input Data
The project requires the following datasets:
- Website order report: Lists Order IDs and products (SKUs) for each order.
- Warehouse pincode to All India pincode mapping: Used to determine delivery zones and compare them with the courier company's invoice.
- SKU master with gross weight: Helps calculate the total weight of each order and compare it with the courier company's invoice.
- Courier company invoice in CSV format: Contains information such as AWB Number, Order ID, weight of shipment, warehouse pickup pincode, customer delivery pincode, delivery zone, charges per shipment, and shipment type.
- Courier charges rate card: Provides the charges at weight slab and pincode levels.

## Output Data
The system generates a resultant CSV/Excel file with the following columns:
- Order ID
- AWB Number
- Total weight as per the company's records
- Weight slab as per the company's records
- Total weight as per the courier company's invoice
- Weight slab charged by the courier company
- Delivery zone as per the company's records
- Delivery zone charged by the courier company
- Expected charge as per the company's records
- Charges billed by the courier company
- Difference between expected and billed charges

## Exploratory Data Analysis (EDA)

During the course of this project, various exploratory data analysis techniques were applied to gain insights into the dataset. The following EDA findings provide a deeper understanding of the data and are relevant to the project:

### Histogram of Total Weight
![Histogram of Total Weight](https://github.com/Aravinth-Megnath/Data-analysis-project--Delivery-cost/assets/120720408/b41fdeec-e2e2-4c7f-b59e-70a1490fa24d)

The histogram shows the distribution of the total weight of packages as per Company X. It reveals that the majority of the packages in the dataset have a weight between 0.5 and 1.5 kilograms.

### Barplot - Courier Company Charges by Delivery Zone
![Barplot - Courier Company Charges by Delivery Zone](https://github.com/Aravinth-Megnath/Data-analysis-project--Delivery-cost/assets/120720408/e672859d-0403-4ae9-adc9-31b59e287770)

The bar plot displays the charges billed by the courier company for each delivery zone. It indicates that delivery zones b, d, and e have the highest charges. The length of the line bisecting the bars represents the standard deviation of the charges. Zone e exhibits higher variability in charges compared to other zones.

### Scatterplot - Expected vs. Billed Charges by Courier Company
![Scatterplot - Expected vs. Billed Charges by Courier Company](https://github.com/Aravinth-Megnath/Data-analysis-project--Delivery-cost/assets/120720408/acda5208-fc11-4693-b68f-37c99f7fae70)

The scatterplot illustrates the relationship between the expected charges and the billed charges by the courier company for different delivery zones. It shows that there is variability in the billed charges for different expected charges and delivery zones.

### Boxplot - Comparison of Delivery Zone Charges
![Boxplot - Comparison of Delivery Zone Charges](https://github.com/Aravinth-Megnath/Data-analysis-project--Delivery-cost/assets/120720408/ce8e94f3-9ce5-493d-b0b9-1adc0011e5d6)


The box plot compares the charges billed by the courier company for different delivery zones. It reveals that delivery zones b and d have a wider range of charges, including some outliers, indicating variability in charges. Zone e has a wider range of charges, without any outliers.



## Getting Started
To use the Delivery Cost Analysis and Billing Discrepancy Detection System, you can follow these steps:
1. Prepare the required input datasets.
2. Run the system to perform the analysis and generate the resultant CSV/Excel file.
3. Review the analysis results to identify billing discrepancies and gain insights into weight slabs, delivery zones, and charges.


## Contributing
Contributions to the Delivery Cost Analysis and Billing Discrepancy Detection System are welcome! If you have any suggestions, improvements, or bug fixes, please feel free to submit a pull request.

## License
This project is licensed under the [MIT License](LICENSE).


## Feedback

Your feedback is important to me! If you have any suggestions, questions, or feedback regarding this project, please feel free to reach out to me at:

- Email: [aravinthmegnath@gmail.com]
- [![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue.svg)](https://www.linkedin.com/in/aravinth-meganathan-200667a1/)

I appreciate your valuable input and look forward to hearing from you!
