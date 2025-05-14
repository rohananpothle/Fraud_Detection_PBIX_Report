# Dataset Overview:
The dataset contains information on various financial transactions, including payments, transfers,
and cash-outs. Each transaction includes details such as the type of transaction, the origin and
destination accounts, and whether the transaction was fraud or not.

# Data Dictionary:
  • step - maps a unit of time in the real world. In this case 1 step is 1 hour of time. Total steps 744
  (30 days simulation).
  
  • type - CASH-IN, CASH-OUT, DEBIT, PAYMENT and TRANSFER.
  
  • amount - amount of the transaction in local currency.
  
  • nameOrig - customer who started the transaction
  
  • oldbalanceOrg - initial balance before the transaction
  
  • newbalanceOrig - new balance after the transaction
  
  • nameDest - customer who is the recipient of the transaction
  
  • oldbalanceDest - initial balance recipient before the transaction.
  
  • newbalanceDest - new balance recipient after the transaction.
  
  • isFraud - 
  
  This is the transactions made by the fraudulent agents inside the simulation. In this
  specific dataset the fraudulent behavior of the agents aims to profit by taking control or
  customers’ accounts and try to empty the funds by transferring to another account and then
  cashing out of the system.
  
  • isFlaggedFraud - 

  The business model aims to control massive transfers from one account to
  another and flags illegal attempts. An illegal attempt in this dataset is an attempt to transfer more
  than 200.000 in a single transaction.

# **Fraudulent Transactions**

  1. All 7,591 transactions shown are fraudulent, representing 100% fraud in the filtered dataset.
  
  2. Total fraudulent transaction amount is ₹11.13 billion.
  
  3. Most common fraud transaction types:
  
  4. TRANSFER: ₹5.6B across 3.77K transactions.
  
  5. CASH_OUT: ₹5.5B across 3.82K transactions.
  
  6. Consistent fraudulent activity across days, with a peak amount of ₹0.56B on a single day and highest transaction count of 286.
  
  7. Fraudulent activity is evenly distributed between TRANSFER and CASH_OUT, both in volume and value—indicating these are key risk areas.

# **Flagged Fraudulent Transactions**

  1. All 16 transactions are both fraudulent and flagged, indicating 100% detection accuracy in this filtered set.
  
  2. Total flagged fraudulent transaction amount is ₹77.79 million.
  
  3. All flagged transactions are of TRANSFER type.
  
  4. The fraudulent activity peaked on Day 32 with ₹23M and 3 transactions.
  
  5. The trend shows low volume but high-value transfers, suggesting targeted fraud attempts rather than widespread activity.


  # Reccomandations
  
  Focus Fraud Detection on TRANSFER and CASH_OUT transactions, given their high value and volume.
  
  Investigate Day 13 transaction surge to rule out any coordinated fraudulent activity.
  
  Use anomaly detection techniques to flag unusual spikes in transaction amount or volume.
