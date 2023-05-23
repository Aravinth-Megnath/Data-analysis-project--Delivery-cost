# Delivery Cost Analysis and Billing Discrepancy Detection System for E-commerce Companies

## Abstract:
The project aims to develop a system that analyzes the delivery cost and detects billing discrepancies for e-commerce companies. The system utilizes data from the warehouse, courier company, and order details to calculate the expected delivery charges and compares it with the billing amount charged by the courier company. The system also provides a detailed report of the weight slab and delivery zones charged by the courier company, along with the expected and billed charges. The system helps e-commerce companies to identify any discrepancies in the billing and ensure transparency in their billing process, ultimately reducing their costs and increasing customer satisfaction.

## Problem statement:
"An e-commerce company wants to optimize its shipping operations by analyzing the discrepancies between the expected shipping charges and the billed charges by the courier company. The goal is to identify patterns and factors that contribute to these discrepancies and to develop strategies to reduce the difference between the expected and billed charges, while maintaining a high level of customer satisfaction and minimizing operational costs."

## Conclusion:
Based on the analysis performed in this project, we can conclude that there is a significant difference between the expected charges as per the company's weight slots and the actual charges billed by the courier company. This difference could be due to various factors, such as incorrect weight measurement, misclassification of delivery zones, and other factors.

We have also observed that the courier company is charging extra for certain weight slabs, and the charges are not proportional to the weight of the package. This finding can help us negotiate better rates with the courier company and optimize our shipping costs.

In conclusion, this project highlights the importance of analyzing shipping charges to identify cost-saving opportunities and improve overall efficiency in logistics operations.

## Overview:
Please understand the below mentioned real-life scenario and try to solve the assignment.
The sample data is attached in the link provided below for your reference.

### Business Scenario:
You are a data analyst and your client has a large ecommerce company in India (let’s call it X).
X gets a thousand orders via their website on a daily basis and they have to deliver them as fast
as they can. For delivering the goods ordered by the customers, X has tied up with multiple
courier companies in India as delivery partners who charge them some amount per delivery.

### Input Data:
Left Hand Side (LHS) Data (X’s internal data spread across three reports):
- Website order report- which will list Order IDs and various products (SKUs) part of each order. Order ID is common identifier between X’s order report and courier company invoice
- Warehouse pincode to All India pincode mapping -(this should be used to figure out delivery zone (a/b/c/d/e) and during analysis compare against one reported by courier company in their CSV invoice per Order ID
- SKU master with gross weight of each product. This should be used to calculate total weight of each order and during analysis compare against one reported by courier company in their CSV invoice per Order ID. The courier company calculates weight in slabs that is applicable for that delivery zone, so first you have to figure out the total weight of the shipment and then figure out applicable weight (based on zone’s weight slab)

### RHS Data (courier company invoice in CSV file):
- Invoice in CSV file mentioning AWB Number (courier company’s own internal ID), Order ID (company X’s order ID), weight of shipment, warehouse pickup pincode, customer delivery pincode, zone of delivery, charges per shipment, type of shipment
- Courier charges rate card at weight slab and pincode level. If the invoice mentions “Forward charges” then only forward charges (“fwd”) should be applicable as per zone and fixed & additional weights based on weight slabs. If the invoice mentions “Forward and rto charges” then forward charges (“fwd”) and RTO charges (“rto”) should be applicable as per zone and fixed & additional weights based on weight slabs.
- For the first slab of that zone, “fixed” rate as per the slab is applicable. For each additional slab, “additional” weight in the same proportion is applicable. Total charges will be “fixed” + “total additional” if any. For example: weight 2.2KG, Zone C. So for Zone C the slab length = 0.75KG. So the total applicable weight = 2.25KG. For the first 0.75 KG the charge is “fwd”, and for each 0.75 after the first, charges will be additional charges.

### Output Data:
Create a resultant CSV/Excel file with the following columns:
- Order ID
- AWB Number
- Total weight as per X (KG)
- Weight slab as per X (KG)
- Total weight as per Courier Company (KG)
- Weight slab charged by Courier Company (KG)
- Delivery Zone as per X
- Delivery Zone charged by Courier Company
- Expected Charge as per X (Rs.)
- Charges Billed by Courier Company (Rs.)
- Difference Between Expected Charges and Billed Charges (Rs.)

