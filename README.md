# CREATION OF DATABASE AND BACKUPS<!DOCTYPE html>

<li><strong>Overview:</strong> A Database ia an organized collection of data that can be easily accessed, managed and updated(e.g., SQL Server, MySQL, PostgreSQL) and its    
                PURPOSE IN MY PROJECT IS
                 i)Create Azure SQL Database 
                 ii)Enable Transparent Data Encryption(TDE)
                 iii)Use Azure backups (5GB) and manual snapshots for site recovery.</li>
                <li><strong>Requirements:</strong> Requirements are database server access, credentials, and other necessary tools (e.g., Azure CLI, SQL Management Studio).</li>
                <li><strong>Database Creation Steps:</strong> 
                    <pre>    Create an Azure SQL account, then give the database a name
                      <img width="839" height="326" alt="db2" src="https://github.com/user-attachments/assets/a990f3a1-b8c3-4167-8ced-ee5f1b217075" />
                      Select Microsoft entra only
                      <img width="700" height="377" alt="db3" src="https://github.com/user-attachments/assets/c7249853-d3b5-415a-a7bf-fd43b01d3df0" />
                      Go to the next step thats Networking, then select private endpoint in connectivity method
                      <img width="622" height="389" alt="db5" src="https://github.com/user-attachments/assets/a61309b2-a0fd-4975-aca0-dc7889fae42e" />
                      Next step is to create a private endpoint and also a virtual network next
                      <img width="943" height="394" alt="db10" src="https://github.com/user-attachments/assets/3a840be5-9178-49f6-9774-968d9802dd
                      <img width="584" height="254" alt="db6" src="https://github.com/user-attachments/assets/43655a87-aa0c-40bc-8843-526235715ead" />
                      TO use free service so you dont incure cost create your virtual network from cost management+Biling and this are few steps on how to go about it
                      Go to Biling (benefits and then preview)
                      Go to Virtual Network (50) and create
                      Next step is SECURITY
                      Enable DDOS protection to prevent attack
                      <img width="680" height="368" alt="db7" src="https://github.com/user-attachments/assets/3e2b13fa-69f4-4749-87ad-973a23d9530f" />
                      Then enable Virtual Encryption
                      Next is IP Address
                      Go to Add Subnets, Defualt and edit in the right corner
                      <img width="935" height="380" alt="db8" src="https://github.com/user-attachments/assets/07a76e2b-1e1d-47fa-9dd2-bef0c16f76f8" />
                      Then review and create
                      NB: Creating a Virtual Network prevents access from public endpoint. it can only be accessed within the organization (private endpoint)
                      Go back to SQL Database
                      Input the VN in Private Endpoint, then create
                      <img width="943" height="394" alt="db10" src="https://github.com/user-attachments/assets/0efdc323-6fc2-4235-8e6a-5d8b91c715c8" />
                      Go to the Database created, Go to security, then Data Encryption, confirm if its on and encrypted
                      <img width="691" height="389" alt="db last" src="https://github.com/user-attachments/assets/660ed0f9-123a-49be-8038-3bd73a0b8178" />
                      




  </pre> Azure Backup is a cloud-based service that helps you back up or protect and also restore your data in Microsoft's cloud. It is part of Azure recovery suite.  We can use it to back up
                    On-premises servers and files,
                    Azure Virtual Machine,
                    SQL database (on Azure VMs or managed instances),
                    Azure file share, 
                    Application and workloads.
                </li> General requirements include Azure Subscription, Recovery Service Vault, Storage type, Network Access, Encryption Key etc
                <li><strong>Backup Steps:</strong>
                    <pre> Go to Backup Vault and then CREATE
                    Input your Resource group
                    Backup Vault name 
                    Select Locally reductant storage for your Backup Storage
                    <img width="572" height="328" alt="backup1" src="https://github.com/user-attachments/assets/48f498c4-50d1-4a61-99b5-5495570ea9a7" />
                    Review and create
                    <img width="545" height="371" alt="backup2" src="https://github.com/user-attachments/assets/6e3daf47-d27e-4f71-96b7-05b43c038550" />
                    Then go to your resourse 
                    Add backup
                    Configure the Backup
                    Database type- Azure Blobs 
                    Vault-input a name
                    <img width="604" height="393" alt="backup4" src="https://github.com/user-attachments/assets/b1f997db-a00e-4eb3-b239-fd473a3941eb" />
                    Backup policy- Create new
                    <img width="604" height="379" alt="backup5" src="https://github.com/user-attachments/assets/f5600647-b875-4583-abd8-5412f8896288" />
                    Edit Retention
                    Specify the duration you want and also specify operational backup
                    <img width="933" height="400" alt="backup6" src="https://github.com/user-attachments/assets/bca2cf03-712c-4185-8031-a3dc1c7f5bc5" />
                    Select next and select the backup frequency you desire either daily or weekly
                    Edit your Time and Time zone 
                    Set retention settings (vaulted backup)
                    Edit it to 7days or optional days (set retention date as long as company will need it)
                    Then create
                    <img width="922" height="383" alt="backup7" src="https://github.com/user-attachments/assets/32b340eb-ad4e-466b-8bfc-7e7cc5143592" />
                    Next Data source (edit) choose the storage account you want to backup
                    <img width="879" height="410" alt="backup8" src="https://github.com/user-attachments/assets/f4619da3-ea81-465d-876a-09f43b2ed4ee" />
                    </pre>
                </li>
                <li><strong>Troubleshooting:</strong> Add common issues and solutions.</li>
                <li><strong>References:</strong> Link to official documentation for your database technology.</li>
            </ul>
        </li>
        <li>
            <strong>Commit and Push:</strong>
            <ul>
                <li>Commit your documentation file and push it to your GitHub repository.</li>
            </ul>
        </li>
        <li>
            <strong>Keep Documentation Updated:</strong>
            <ul>
                <li>Update the documentation as your database setup or backup process changes.</li>
            </ul>
        </li>
    </ol>
    <p>
        For more details, see the official documentation for your database technology (e.g., 
        <a href="https://learn.microsoft.com/en-us/sql/" target="_blank">SQL Server Docs</a>, 
        <a href="https://dev.mysql.com/doc/" target="_blank">MySQL Docs</a>, 
        <a href="https://www.postgresql.org/docs/" target="_blank">PostgreSQL Docs</a>).
    </p>
</body>
</html>
