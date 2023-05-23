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

## Getting Started
To use the Delivery Cost Analysis and Billing Discrepancy Detection System, you can follow these steps:
1. Prepare the required input datasets.
2. Run the system to perform the analysis and generate the resultant CSV/Excel file.
3. Review the analysis results to identify billing discrepancies and gain insights into weight slabs, delivery zones, and charges.

Please refer to the project documentation and code for detailed instructions on setting up and running the system.

## Contributing
Contributions to the Delivery Cost Analysis and Billing Discrepancy Detection System are welcome! If you have any suggestions, improvements, or bug fixes, please feel free to submit a pull request.

## License
This project is licensed under the [MIT License](LICENSE).
