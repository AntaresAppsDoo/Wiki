# Antares Apps doo – Serbian Functionalities Help - Setup

## Installation
[Click here to search for Serbian Functionalities on AppSource](https://appsource.microsoft.com/en-us/product/dynamics-365-business-central/PUBID.antaresapps1634735406093%7CAID.serbianfunctionalities%7CPAPPID.92da857b-0491-42d8-9333-e69b77e879af).

## Setup The Company Currency to RSD
Set RSD for LCY Code in General Ledger Setup. This field is across the system to determine if serbian functionalities are active in the company.
General Ledger Setup -> LCY Code

## Setup Currency Exchange Rates Update
Currencies -> Exchange Rate Service -> Exchange Rate Services
After calling the Action "Exchange Rate Services" the connection with National Bank of Serbia will be initialized.
Open the Exchange Rate Service Card and enter the username, password and licence id.
Enable the Exchange Rate Service and select the parameter for running the Job Queue.
Suggested Settings: Run once daily at 08:30

## Setup Bank Account Update based on VAT Registration No.
Purchases & Payables Setup -> Set Up Bank Account Sync.
After running the action "Set Up Bank Account Sync." enter the username, password and licence id.

## Setup Bank Statement Export/Import
Bank Export/Import Setup -> Set Up Office Banking
Bank Export/Import Setup -> Set Up Halcom Banking
Create new Bank Account and enter values in field "Bank Statement Import Format" and "Payment Export Format"
General Journal Templates -> create new General Journal Template for example PAYMENT. Type = Payments
General Journal Templates -> Related -> Template -> Batches -> Create new batch for example EXPORT. "Bal Account Type" = Bank Account, enter Bank Account in field "Bal. Account No."
General Journal Templates -> Related -> Template -> Batches -> Create new batch for example IMPORT. "Bal Account Type" = Bank Account, enter Bank Account in field "Bal. Account No."

## Reporting bugs
If you stumble upon any issues please report an issue on the following link:
[Issues](https://github.com/AntaresAppsDoo/Wiki/issues).
