# UPI_Transactions_CDC_Feed_Project

## What is this?
This project is a **Change Data Capture (CDC) Pipeline** built using **Databricks and GCP** to process real-time transaction data efficiently.

## What do we do in it?
- Process UPI merchant payment transactions.
- Aggregate real-time merchant transaction data.
- Load data into a **staging Delta table**.
- Merge new records into a **target Delta table**, ensuring deduplication.

## How to Run
1. Upload transaction data to the designated source location in **DBFS**.
2. Run `upi_merchant_pay_trx_mock_data.ipynb` to generate and stage transaction data.
3. Run `realtime_merchant_aggregation.ipynb` to aggregate and merge the transactions into the final table.

