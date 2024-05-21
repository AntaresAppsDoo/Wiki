# Antares Apps doo – Serbian Functionalities Help - Setup

## Creating a Cash Desk
To create a cash desk, navigate to Cash Desks and click on +New. This action will open the Cash Desk card, where you'll need to input the required information into the corresponding fields.<br/>
Ensure to complete the mandatory fields, including Cash Desk Posting Group, Debit Rounding Account, Credit Rounding Account, Rounding Method Code, Cash Receipt Limit, and Cash Withdrawal Limit.<br/>
Under the Numbering section, select CASH-DESK-RECEIPT for the Cash Document Receipt Nos. field, and CASH-DESK-WITHDRAWAL for the Cash Document Withdrawal Nos. field. This finalizes the process of creating the cash desk.

## Creating Cash Desk Templates
To create Cash Desk Templates, navigate to Settings, then My Settings, and choose the Accountant role. Within the Cash Management section, access Cash Desk Templates.<br/> 
Once the Cash Desk Templates card appears, select +New to initiate the creation of the cash desk template by filling in the required fields, ensuring that the Cash Desk No. and Cash Document Type fields are completed.<br/> 
To check if templates have been created for each cash desk, click on Related, select Setup, and then choose Cash Desk Templates. If you want to use a Cash Desk Template while creating a new cash document, go to the Lines section, click on Cash Desk Template, and select the desired template.

## Creating a Cash Document
To create a Cash Document, you must first select the appropriate Cash Desk. When the Cash Desk card appears, select the +New option.<br/>
Within the General section, ensure to fill in the mandatory fields: Document Type and Payment Purpose.<br/>
Moving to the Lines section, select the appropriate option for the Account Type field based on the Document Type and Payment Purpose. Then, input the Account No. and Amount. This completes the creation of the cash document, which is automatically assigned the Open status.

## Releasing a Cash Document
To change the document status to Released, navigate to the Release card and select the Release option.<br/>
If the document already has the Released status, selecting the Reopen option will revert it to the Open status.

## Posting a Cash Document
To post a Cash Document, navigate to the Post card and confirm your intention to post the relevant document.<br/>
Upon confirmation, the document's status will change to Posted and it will be automatically included in the Posted Cash Documents.<br/>
For each posted document, you can access the Related Entries card to view all items and documents associated with that document and its posting date.

## Printing a Cash Document
To print a cash document, choose the relevant cash desk, then click on the Related card. Next, select the Documents option and choose from the three available document groups (Open Cash Documents, Released Cash Documents, Posted Cash Documents).<br/>
This will display a list of cash documents. Click on the desired document to open it.<br/>
Once you've opened the specific cash document, navigate to the Print card and select the Print option.

## Setting up Payment Methods
To configure payment methods navigate to Settings, then My Settings, and select the Accountant role. In the search bar, type "Payment Methods" to access the Payment methods page.<br/>
From the list provided, choose "CASH DESK". In the Cash Desk Code column, select the cash desk associated with the payment. In the Cash Document Action column, choose from the available options.<br/>
Selecting Create generates a cash document with an Open status. Opting for Release assigns the cash document an Released status. Choosing Post automatically posts the document, giving it a Posted status. Additionally, options like Release and Print and Post and Print enable automatic printing.

## Posting a Sales or Purchase Document
If you create a Purchase Order for a supplier and select CASH DESK in the Payment Method Code field, depending on the selected action in the Payment Method, the document will be created, released, or posted with the possibility of automatic printing.<br/>
If you create a Sales Order for a customer and select CASH DESK in the Payment Method Code field, depending on the selected action in the Payment Method, the document will be created, released, or posted with the possibility of automatic printing.<br/>

## Reporting bugs
If you stumble upon any issues please report an issue on the following link:
[Issues](https://github.com/AntaresAppsDoo/Wiki/issues).
