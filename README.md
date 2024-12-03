# **End User cant use windows search and printer isn't connecting to `client-1.mydomain.com`**

# **Prerequisites**
----

- You need administrative privileges in the Active Directory in DC-1.
- Client-1 end user will be `bade.core`, device name `client-1.mydomain.com` 
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



## **End User `bade.core` was temporary administrator privileges to install software or update existing applications**

- End users generally do not need admin privileges for routine tasks on a computer. However, there are certain scenarios where an end user might request or need admin rights. These cases typically involve the ability to perform tasks that require elevated privileges—such as installing software, modifying system settings, or managing services—that are restricted for security and stability reasons, and just for fun.  

 ![image](https://github.com/user-attachments/assets/3e098a27-8236-47f3-84ad-6baf2a87366a)
![image](https://github.com/user-attachments/assets/23636623-062f-49db-9663-5da23a49148e)

-End-User `bade.core` wants to run `Windows Command Processor` as ADMIN
![image](https://github.com/user-attachments/assets/dc4aa269-9db6-40bd-b2f3-36e7b9fe01b2)
![image](https://github.com/user-attachments/assets/45ff4691-c81c-4211-bb09-cbe54bc8d9cb)

## **checking security logs**

![image](https://github.com/user-attachments/assets/a4ec0853-d1ff-4564-b730-9baa3543022f)



## **As Admin Remote Desktop to End-Users computer**

- Open Remote Desktop Connection 
![image](https://github.com/user-attachments/assets/3bbcdd26-bab0-4db5-92f5-38beeda2447d)
![image](https://github.com/user-attachments/assets/e3b13d29-1754-47dd-9ee4-7e919613bd1c)
![image](https://github.com/user-attachments/assets/8970d76a-be02-4be8-b35a-4a61c9fcd23f)
![image](https://github.com/user-attachments/assets/9cd7bd3c-4ad8-4afc-a8f7-4f1000fc6d29)




## **Using Registry Editor **

![image](https://github.com/user-attachments/assets/d5262f8b-6870-40d9-842e-f6b0e03e658a)

- Could not Connect to Client-1
  ![image](https://github.com/user-attachments/assets/ecef0909-e021-436d-9b30-858b24eddedc)

- Went back into Client-1 to Enable Remote Registry Properties
  ![image](https://github.com/user-attachments/assets/d4aec954-4cdc-4eec-a16d-c1149d276e2a)
  ![image](https://github.com/user-attachments/assets/20ce926d-40d4-4fd7-bc3d-88b6e297c090)

- In DC-1 I was able to connect to `client-1.mydomain.com` 
![image](https://github.com/user-attachments/assets/949a1d2a-8db1-4245-9f4c-df94677be44e)














