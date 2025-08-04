# CREATION OF DATABASE AND BACKUPS<!DOCTYPE html>

<li><strong>Overview:</strong> A Database ia an organized collection of data that can be easily accessed, managed and updated(e.g., SQL Server, MySQL, PostgreSQL) and its purpose in my project is to i)Create Azure SQL Database 
                 ii)Enable Transparent Data Encryption(TDE)
                 iii)Use Azure backups (5GB) and manual snapshots for site recovery.</li>
                <li><strong>Requirements:</strong> Requirements are database server access, credentials, and necessary tools (e.g., Azure CLI, SQL Management Studio).</li>
                <li><strong>Database Creation Steps:</strong> Provide step-by-step instructions to create the database. For example:
                    <pre>
# Example for SQL Server
CREATE DATABASE MyDatabase;
                    </pre>
                </li>
                <li><strong>Backup Steps:</strong> Explain how to back up the database. For example:
                    <pre>
# Example for SQL Server
BACKUP DATABASE MyDatabase TO DISK = 'D:\Backups\MyDatabase.bak';
                    </pre>
                </li>
                <li><strong>Restore Steps:</strong> (Optional) Add instructions to restore from a backup.
                    <pre>
# Example for SQL Server
RESTORE DATABASE MyDatabase FROM DISK = 'D:\Backups\MyDatabase.bak';
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
