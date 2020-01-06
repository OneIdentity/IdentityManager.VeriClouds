VeriClouds is a credential verification service that helps organizations detect compromised credentials before hackers do.
VeriClouds Solution Accelerator demonstrates the VeriClouds credVerify API integration into the password validation rule of One Identity Manager.

In your environment, you will need to import the VeriClouds Solution Accelerator transport package and configure the 2 customs configuration parameters with the following values:

Custom\credVerify\APIKey = "Api Key name"  (obtained from the Vendor specific to your organization)

Custom\credVerify\APISecret = "Api Secret" (obtained from the vendor specific to your organization)

Then add the script SDK_CredVerify_ValidatePassword to a password policy of choice. For example; to the One Identity Manager password policy (used for System User passwords and the Employee based authenticators) or the Password policy for central password of employees.

Once the script is added to the password policy of choice.  If the user try to set a password that has been detected as compromised via the Password Reset portal (or any other OneIM tool), the system will inform you about the password being compromised and forces you to try a different password. 


