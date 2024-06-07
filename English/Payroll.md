# Antares Apps doo – Antares Payroll Help - Setup

## Installation
[Click here to search for Antares Payroll on AppSource](https://appsource.microsoft.com/en-us/product/dynamics-365-business-central/PUBID.antaresapps1634735406093%7CAID.payroll%7CPAPPID.82ed9411-e456-4ed9-848d-035fead71575).

## Permissions for payroll
After installation make sure that at least one user has been marked as payroll administrator:<br/>
Global Search -> User Setup -> Payroll User -> Admin<br/>
If the user has been set up as Payroll Offices he may need to talk to admin when there is a need to reopen already closed calculations.

## Role Center for Payroll
After installation switch to Payroll Role Center by clicking on:<br/>
My Settings -> Role -> Payroll

## Demo Data
In order to install basic demo data init the process by calling the action:<br/>
Payroll Setup -> Init Setup Data

## Running Payroll Calculation
1. Create new Employee in the Employee List
1. Enter Name, Last Name, National ID, Address and the Bank Account No.
1. Open the Employee Contracts using action Employee -> Contracts
1. Enter From Date, Employment Contract Code, Job Title, Work-Hour Template, Amount Type and Amount
1. Create new Calculation from the Calculation list.
1. Enter Employment Contract Code on the Calculation Card
1. Call Action "Create Calculation Employees"
1. In case it is a type of contract for research and development, it is necessary to call up the employee's card from the calculation card and enter the hours that the employee spent on research and development.
1. Export Calculation to XML in order to be able to send Tax report using the action "Export Calculation to XML"
1. Export Calculation to Gen. Journal Line using the action "Export Calculation to Gen. Journal Line"
1. Close the Calculation in order to prevent further modifications
1. Payments are processed in Payment Journal by using the action "Suggest Payroll Payments"

## Necessary data for exporting Calculation to XML
1. Company information -> Name
1. Company information -> Address
1. Company information -> VAT Registration No.
1. Company information -> Registration No.
1. Company information -> Post code -> Place of residence matches the field "Municipality Payment Code" on the postal code
1. User Setup -> E-mail
1. User Setup -> Phone No.
1. Employee -> Postal code -> Place of residence matches the field "Municipality Payment Code" on the postal code
1. The number of employees is generated on the basis of all active regular employees observed on the first day of calculation

## Reporting bugs
If you stumble upon any issues please report an issue on the following link:
[Issues](https://github.com/AntaresAppsDoo/Wiki/issues).
