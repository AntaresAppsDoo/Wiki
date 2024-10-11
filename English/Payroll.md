# Antares Apps doo – Antares Payroll Help - Setup

## Installation
[Click here to search for Antares Payroll on AppSource](https://appsource.microsoft.com/en-us/product/dynamics-365-business-central/PUBID.antaresapps1634735406093%7CAID.payroll%7CPAPPID.82ed9411-e456-4ed9-848d-035fead71575).

## Permissions for payroll
Three levels of access are provided in the payroll module:
* Payroll Administrator
  * Administrator has unlimited permissions in the Payroll module 
  * recommended permission sets for Cloud environment: SUPER or some other permission set with admin access in combination with "ANTPAYROLLADMIN" permission set.
  * Global Search -> User Setup -> Payroll User -> Admin<br/>
* Payroll Officer
  * Compared to the rights of the administrator, Officer has no right to change the general settings in the module.
  * recommended permission sets for Cloud environment: "D365 READ", "D365 HR, EDIT" and "ANTPAYROLLOFFICER" 
  * Global Search -> User Setup -> Payroll User -> Payroll Officer<br/>
* Payroll Contract Manager
  * Manager can change the Contracts of employees as well as their deductions and bonuses.
  * recommended permission sets for Cloud environment: "D365 READ", "D365 HR, EDIT" and "ANTPAYROLLCONTRMAN" 
  * Global Search -> User Setup -> Payroll User -> Contract Manager<br/>
  
After installation, at least one user needs to be set up as an payroll administrator in user setup. If this is not the case, the data init for the module is not possible.<br/>
In the case of the need to use security filters in order to e.g. the contract manager has limited access to only certain contracts, the following procedure must be performed:<br/>
Permissoin Sets -> position on permission set "ANTPAYROLLCONTRMAN" -> Copy permission set -> Copy by reference -> Opening the newly created permission set and adding only the desired tables with security filters.

## Role Center for Payroll
After installation switch to Payroll Role Center by clicking on:<br/>
My Settings -> Role -> Payroll

## Demo Data
In order to install basic demo data init the process by calling the action:<br/>
Setup -> Payroll Setup -> Init Setup Data
1. Selecting the option "Countries and post codes" will create a record for Serbia in Business Central in the "Countries/regions" table, as well as all municipalities from Serbia in the "Post Codes" table. Existing records in these two tables may be updated. The country and post code can then be assigned on the employee's card.
2. By selecting the option "Calendar and Work Hours Template" a record for Serbia will be created in Business Central in the table "Base Calendars" with all holidays in the current year and the year after the current one. A 40-hour work hours tempplate will also be created. The calendar and work hours template can be assigned when creating an employee contract.
3. By selecting the "Calculation settings" option, all currently supported types of calculations are created in the salary module with all associated settings related to taxes and contributions.
![image](https://github.com/AntaresAppsDoo/Wiki/assets/42636293/589772dd-390f-4005-bcce-97d7d5661a15)

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
1. The printout of the Calculation Recapitulation and Pay List can be called from the calculation card or from the list of calculations
1. Pay slips can be printed and sent to each employee individually or automatically for the entire calculation using e-mail. More information: [Pay Slips](https://github.com/AntaresAppsDoo/Wiki/blob/main/English/PaySlips.md).

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

## Report Selection
The following reports are delivered with the payroll module:
* Pay Slip
* Calculation Recapitulation
* Certificate of paid taxes and withholding tax
* Pay List for a Calculation
* Pay List for a Calculation with Project Shares

These reports can be replaced with user-defined reports using the Report Selection page for the Payroll module:
![image](https://github.com/user-attachments/assets/99096e19-efe9-4fa6-bd8c-e05082482003)


On the example of the Pay List, it is possible to choose one of two reports. The regular pay list is a simplified payroll list of employees, while the other one contains more details grouped by work category and enables an overview of project shares in Excel format.
![image](https://github.com/user-attachments/assets/96ef2359-e288-470d-a73f-27c19c89329b)  
![image](https://github.com/user-attachments/assets/b9d88047-a564-498b-b96e-4861af0e57bc)  

![image](https://github.com/user-attachments/assets/fbad0796-37ac-4eaa-90b4-892f78f7f9df)  
   
![image](https://github.com/user-attachments/assets/9d04e81d-f5c9-467f-8ccc-8b973208ec3f)  

## Reporting bugs
If you stumble upon any issues please report an issue on the following link:
[Issues](https://github.com/AntaresAppsDoo/Wiki/issues).
