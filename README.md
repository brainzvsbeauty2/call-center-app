# call-center-helper

##  Business Requirements

#### Client Request Story:

The client wants an application that allows for recording call related information (contact information, complaint, and/or solution provided). Primary user is call center personnel that are to use this application as they are answering customer’s calls. Calls can be related to the client’s web-site, web-site administration, or transactions. 

1. Minimal functionality version of the application is requested to generate text in the clipboard related to the data entered in the form; this text will be kept elsewhere for records keeping.

2. Extended functionality for future implementation requires hosting data in a database and persisting all the information in-house, for this additional requirements will be given regarding how this data will be viewed and reports that are to be generated for administrative purposes.

3. The perfect application not only will allow for persisting information on a database but customizing the fields and dynamically generating the forms from those customizations. Customizations would be enabled through an administrative interface where any admin user would be able to add, remove and change the fields on the application.

#### Screen Proto-types 

![Call Center Helper Home Screen](https://user-images.githubusercontent.com/58577471/122642818-54422100-d0da-11eb-8941-3a28e0122240.png)


 ## Technical Requirements

1. Display information for the employee to type in certain information while assisting callers.
  * Contact Information about the Caller:
  * Name (required)
  * Call back number (required)
  * Email address (optional)
  
2. The call center employee should select the reason for the call from a list of options
  * Options for the List of Reasons
     * Web-site
     * Administration
     * Transactions


### Based on the Reason selected by the call center employee a list of fields should appear allowing the call center employee to write information about the call but also prompting and reminding them to ask the caller for certain information.

    List of data elements that will always be available:
      * Name
      * Email: 
      * Call back Number: 
      * Appears if Additional Steps Needed is Checked: Steps Text Area
      * Checkbox for resloved issues 
      * Main Customer Complaint/ Extended Reason for Calling
    
### For Web-Site Related calls the fields that the call center employee needs to fill out are:

    * Verification ( Last 4 of SSN and Date of Birth or Security question)  (required)
    * Web Page (required): the actual page the user is calling about
    * Portion of the page (optional): navigation, footer, menu, dropdown etc
    * Browser Type: Chrome, Firefox, Safari, Explorer, Other?
    * Browser Version (optional): can be handy for the development team
    * Date of the Issue (required):
    * Time the issue happened (required):
    * Steps the user followed to cause the issue (optional)
    
![callcentercasecreationweb](https://user-images.githubusercontent.com/58577471/122828288-7642cb80-d2b3-11eb-9bef-270092253996.png)



### For Administration Related calls the fields that the call center employee needs to fill out are:

    * Username (required)
    * Account number: (optional)
    * Verification ( Last 4 of SSN and Date of Birth or Security question)  (required)
    * What was the user’s issue? (why can’t they log in or trying to register or account lock) (required)

![callcentercasecadmin](https://user-images.githubusercontent.com/58577471/122828849-2fa1a100-d2b4-11eb-89c6-a471d8e01b0b.png)


### For Transaction Related calls the fields that the call center employee needs to fill out are:

    * Username (required)
    * Verification ( Last 4 of SSN and Date of Birth or Security question)  (required)
    * Transaction ID (required)
    * Date of transaction: (required)
    * Place of service: Place the transaction was taken place (store, restaurant , or place of business) (required)
    * Amount: The amount for the transaction (required)
    * Transaction type: Was the transaction a mistake or fraud or return ? (required)

![callcentercase transaction (1)](https://user-images.githubusercontent.com/58577471/122643810-eac51100-d0df-11eb-898e-40d2ad4f3004.png)



