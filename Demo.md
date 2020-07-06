## Azure SQL Database Deployment using CI/CD and Key-Vault Secrets

- Azure SQL Database type project can be created from Visual Studio and with the help of Azure DevOps CI/CD pipeline deployment will be made.
- CI pipeline gets automatically triggered for any changes made in the devops repository.
- It publishes the drop Artifacts and these Artifacts are deployed to Microsoft Azure using Release pipeline.
- Release Pipeline has two jobs 
      - Azure Key Vault
      - Azure SQL Dacpac
Azure Key Vault uses vault account from our azure portal.
Azure SQL Dacpac job takes values from variable and password from sql key secret via vault.

![image](https://user-images.githubusercontent.com/24872414/86594053-fd6c3600-bfb3-11ea-986d-234f6ac14dfc.png)

<div align='center'>
<u>
Fig 1.1 Azure Key-Vault Job
</u>
</div>

![image](https://user-images.githubusercontent.com/24872414/86594239-47edb280-bfb4-11ea-8a59-82ec684d44b0.png)

<div align='center'>
<u>
Fig 1.2 Azure SQL DacpacTask
</u>
</div>
