# **End User cant use windows search and printer isn't connecting to `client-1.mydomain.com` **

# **Prerequisites**
----

- You need administrative privileges in the Active Directory in DC-1.
- Client-1 end user will be `jbade.core`, device name `client-1.mydomain.com` 
- You need to be able to access the target computers via Computer Management.
- The remote management tools must be enabled on the target machines (Remote WMI, RPC, etc.).
- You should know the target machine's hostname or IP address.

## **Step 1: Open Computer Management on your Admin PC**

- logging in as `jane_admin` in DC-1 to 
- Press Windows + R to open the Run dialog.
- Type compmgmt.msc and press Enter. This will launch Computer Management.
  ![image](https://github.com/user-attachments/assets/0278eda7-18a6-48ad-a160-1d9ef92534df)

- Computer Management
  ![image](https://github.com/user-attachments/assets/387fdb77-38b7-44ae-a283-2a5df7ccf554)

## **Step 2: Connect to a Remote Computer**
- In the Computer Management window, expand the System Tools section on the left panel.
- Right-click on Computer Management (Local) and select Connect to another computer.
  ![image](https://github.com/user-attachments/assets/ee517923-25f4-49dc-a235-e5fe2b3d0e31)

- In the dialog box, enter the hostname or IP address of the remote computer where you want to restart Windows Search and Printer services. Stop and         Restart.
  ![image](https://github.com/user-attachments/assets/fee20e1c-dc29-4040-a7be-942d1dbe35f0)

  ![image](https://github.com/user-attachments/assets/dacdb3d3-7186-4c51-b281-e437b3fb0e54)


- If the machine is part of the same domain and you have the appropriate permissions, it should connect successfully.
- If prompted, enter the credentials for an account that has administrative access to the target machine.
 

