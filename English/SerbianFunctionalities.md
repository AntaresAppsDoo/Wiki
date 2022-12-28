# Antares Apps doo – Serbian Functionalities Help - Setup

## Installation
[Click here to search for Serbian Functionalities on AppSource](https://appsource.microsoft.com/en-us/product/dynamics-365-business-central/PUBID.antaresapps1634735406093%7CAID.serbianfunctionalities%7CPAPPID.92da857b-0491-42d8-9333-e69b77e879af).

## Setup The Company Currency to RSD
Set RSD for LCY Code in General Ledger Setup. This field is across the system to determine if serbian functionalities are active in the company.<br/>
General Ledger Setup -> LCY Code

## Setup Currency Exchange Rates Update
Currencies -> Exchange Rate Service -> Exchange Rate Services<br/>
After calling the Action "Exchange Rate Services" the connection with National Bank of Serbia will be initialized.<br/>
Open the Exchange Rate Service Card and enter the username, password and licence id.<br/>
Enable the Exchange Rate Service and select the parameter for running the Job Queue.<br/>
Suggested Settings: Run once daily at 08:30

## Setup Bank Account Update based on VAT Registration No.
Purchases & Payables Setup -> Set Up Bank Account Sync.<br/>
After running the action "Set Up Bank Account Sync." enter the username, password and licence id.

## Setup Bank Statement Export/Import
Bank Export/Import Setup -> Set Up Office Banking<br/>
Bank Export/Import Setup -> Set Up Halcom Banking<br/>
Create new Bank Account and enter values in field "Bank Statement Import Format" and "Payment Export Format"<br/>
General Journal Templates -> create new General Journal Template for example PAYMENT. Type = Payments<br/>
General Journal Templates -> Related -> Template -> Batches -> Create new batch for example EXPORT. "Bal Account Type" = Bank Account, enter Bank Account in field "Bal. Account No."<br/>
General Journal Templates -> Related -> Template -> Batches -> Create new batch for example IMPORT. "Bal Account Type" = Bank Account, enter Bank Account in field "Bal. Account No."

## Prepayments
**1. Customer Posting Groups setup:**
![image](https://user-images.githubusercontent.com/42636293/209877202-4e0ee4e7-f2c5-4bc6-b558-ab9c7b6dabd7.png)

**2. Vendor Posting Groups setup:**
![image](https://user-images.githubusercontent.com/42636293/209877259-44a64a91-fa1c-4e67-98b2-04efcb5e8679.png)

**3. VAT Posting Setup:**
![image](https://user-images.githubusercontent.com/42636293/209877322-029972b9-2e82-4762-bd5f-6dec9229fcef.png)

**4. G/L Accounts Setup:**
![image](https://user-images.githubusercontent.com/42636293/209877342-dc1ea625-d363-4525-8092-55b7be24736f.png)
![image](https://user-images.githubusercontent.com/42636293/209877368-e582fe6a-ef8a-498d-ba5c-b2da1123dec7.png)
![image](https://user-images.githubusercontent.com/42636293/209877399-0d4b34b2-3988-473e-924b-36a626820354.png)
![image](https://user-images.githubusercontent.com/42636293/209877412-373a63d3-ca1d-4bdc-9ef2-b29dddc1be81.png)

## Reporting bugs
If you stumble upon any issues please report an issue on the following link:
[Issues](https://github.com/AntaresAppsDoo/Wiki/issues).
