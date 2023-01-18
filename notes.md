---------------------------------------------------------------------------------------------------------
WINDOWS SERVICES: 
---------------------------------------------------------------------------------------------------------
https://stackify.com/what-are-windows-services/

    It is core component of microsoft operating system and enable the creation and management of long running process. 
    Unlike regular software, windows services can start without user intervention. 

    It consists of, 
        Local Services 
        Network Services 
        System 
    
    Examples of Windows services: 
        Active Directory Services 
        Background Intelligent Transfer Service 
        DNS Client Service - Resolves domain name to IP address. 
        Internet Connection Sharing (ICS) service 
        Routing and Remote Access Service 

    Application can be install it as a service by running utility InstallUtil.exe then passing path to service executable file then use services control manager to configure service. 

---------------------------------------------------------------------------------------------------------
WINDOWS SCHEDULED TASK SERVICES: 
---------------------------------------------------------------------------------------------------------
https://www.coretechnologies.com/blog/windows-services/schedule/

    Task scheduler service is used which is responsible for automatically launching executables, batch files and scripts without human intervention on, 
        Fixed date and time.
        When someone logs on to computer. 
        When system is booted. 
        When machine becomes idle. 
        When specific system event occurs. 

---------------------------------------------------------------------------------------------------------
IIS (Internet Information Services) SERVICES: 
---------------------------------------------------------------------------------------------------------
https://stackify.com/iis-web-server/

    An IIS webserver runs on Microsoft .Net platform on Windows OS. 
    IIS is used to host ASP.NET web application and static websites over the internet. 

    This is like apache used in Linux. 


---------------------------------------------------------------------------------------------------------
UNIX ACCOUNTS: 
---------------------------------------------------------------------------------------------------------
https://www.compuhoy.com/what-is-a-unix-account/#:~:text=A%20shell%20account%20is%20a,such%20as%20telnet%20or%20SSH.

    It provides interactive access to system. 
    Groups are used to logically group the user or accounts. 

    useradd         -> To add new account. 
    id -u user-name -> To check user.  
    echo $UID       -> To check user. 


---------------------------------------------------------------------------------------------------------
SSH KEYS: 
---------------------------------------------------------------------------------------------------------
https://www.cyberciti.biz/faq/how-to-set-up-ssh-keys-on-linux-unix/

    It provides secure way of logging. 
    ssh-keygen      -> To generate key 
    ssh-copy-id     -> To copy the public to server. 

---------------------------------------------------------------------------------------------------------
SERVICE ACCOUNTS: 
---------------------------------------------------------------------------------------------------------
https://www.beyondtrust.com/blog/entry/how-to-manage-and-secure-service-accounts-best-practices

    Service accounts are special type of non human privileged account used to execute applications and run automated services, virtual machine instances and other processes. 


---------------------------------------------------------------------------------------------------------
DEVOPS INTEGRATION: 
---------------------------------------------------------------------------------------------------------

Jenkins 

JFrog-Artifactory 

Udeploy 

Ansible 

Terraform 

GitHub

---------------------------------------------------------------------------------------------------------

IAC Code Steps: (GitHub -> Terraform )

    1. Write the IAC code in local VS Code. 
    2. Commit the code to GitHub.
    3. In Terraform Enterprise, create workspace.
    4. Under Settings, Version Control -> Select GitHub repository. 
    5. Whenever code is commit, it trigger the terraform workspace. 

Ansible Code Steps: (Ansible in Github -> Udeploy)

    1. Write the Ansible code in local VS code. 
    2. Commit the code to GitHub.
    3. In Udeploy bootstrapping component process, 
            a. Download the git using copy module.
            b. Execute the ansible script using ${p:bootstrap_ansible_execution}
    
Udeploy -> Terraform: 

    1. Write the terraform code and move to github. 
    2. Write the ansible code to trigger terraform. 
    3. Use the ansible code in Udeploy for deployment. 

---------------------------------------------------------------------------------------------------------

