# Antares Apps doo – Transit Account

# Description of functionality
A transit account can be used in purchasing to temporarily post document lines to the general ledger to the selected transit account instead of the purchasing account. A transit account can be entered on purchase order lines, purchase invoice lines, and purchase credit memo lines.

## Entry of the transitional account on the purchase document
In order for the entry of the transitional account on the purchase document to be possible, it is necessary to display the field "Transit G/L Account No." in the purchase document. If the value of the field was entered during posting, the purchase account will be replaced by the entered account. If the value of the field is ignored, the posting takes place on the purchase account.  
<img width="967" alt="image" src="https://github.com/user-attachments/assets/db6038ad-06ac-4b55-ac85-1505c1987c70">

## Verification of general ledger items
After posting, it is possible to identify the general ledger entries which postings took place to the entered transitional account. For this purpose, it is necessary to display the field "Source G/L Account No." on the general ledger entries.  
<img width="1028" alt="image" src="https://github.com/user-attachments/assets/cb582ce9-c0c6-4313-80bc-bcbee3652315">

## Transfer from the transit account to the purchase account
In order for amounts to be transferred from the temporary account to purchase account, it is necessary to call the action "Move from transit accounts" in the General Journal:  
![image](https://github.com/user-attachments/assets/c18363fa-e241-49f1-b24c-6ed76f76788a)
