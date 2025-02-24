# Antares Apps doo – Auto Close Vendor Entries - Functionality

## Functionality Overview
The "Auto Close Vendor Entries" feature streamlines the process of closing vendor ledger entries in Business Central. Its primary purpose is to identify entries that meet predefined conditions for automatic closure, reducing manual effort and improving process efficiency.

## Running the functionality
To access  the "Auto Close Vendor Entries" feature, open the global search (Alt + Q), type "Auto Close Vendor Entries" and select the corresponding option under "Go to Pages and Tasks." This will open the execution window for the functionality.
Before starting the process, configure the following parameters:
   - **Allow Partial Closing:**  
     When enabled, the system permits partial closing of vendor entries. If an entry cannot be fully closed - for example, due to discrepancies in amounts - the system will close only the portion that meets the conditions.
   - **Closing Entries Can Be Older:**  
     When enabled, the system allows the closing of entries even if the posting date of a positive entry (e.g., a payment) is earlier than that of a negative entry (e.g., an invoice).
   - **Filter - Vendor Ledger Entry:**  
     Specify a vendor number to restrict the process to entries related to a particular vendor.
Once the parameters are set, click "OK" to execute the process.

## Result
After processing, the system will display a message summarizing the outcome:
  - If entries have been successfully closed, the system will indicate the number of closed entries. 
  - If no entries meet the closing conditions, an appropriate message will be displayed.

## Reporting bugs
If you stumble upon any issues please report an issue on the following link:
[Issues](https://github.com/AntaresAppsDoo/Wiki/issues).

