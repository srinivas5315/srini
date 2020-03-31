# Deploy an HPC Pack cluster in Azure with Microsoft HPC Pack 2019 Preview

## **Note:**

See [Pre-Requisites](#prerequisites) section on this page before starting your deployment.

---

## Following templates are Active Directory Domain integrated

### Template 1: High-availability cluster for Windows workloads with new Active Directory Domain

This template deploys an HPC Pack cluster with high availability for Windows HPC workloads in Active Directory Domain forest. The cluster includes one domain controller, **two** head nodes, one Database Server with SQL Server 2016 Standard version, and a configurable number of **Windows** compute nodes.

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FAzure%2Fhpcpack-template%2Fmaster%2FHPCPack2019%2Fnewcluster-templates%2Ftwo-hns-wincn-ad.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>

### Template 2: High-availability cluster for Windows workloads with existing Active Directory Domain

This template deploys an HPC Pack cluster with high availability for Windows HPC workloads in an existing Active Directory Domain forest. The cluster includes **two** head nodes, one Database Server with SQL Server 2016 Standard version, and a configurable number of **Windows** compute nodes. You can choose not to create public IP address for the head node if you have a virtual network with Express Route configured and you want to join the cluster to your on-premises Active Directory Domain.

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FAzure%2Fhpcpack-template%2Fmaster%2FHPCPack2019%2Fnewcluster-templates%2Ftwo-hns-wincn-existing-ad.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>

### Template 3: High-availability cluster with Azure SQL databases for Windows workloads with existing Active Directory Domain

This template deploys an HPC Pack cluster with high availability for Windows HPC workloads in an existing Active Directory Domain forest. The cluster includes **two** head nodes, SQL Azure databases, and a configurable number of **Windows** compute nodes. You can choose not to create public IP address for the head node if you have a virtual network with Express Route configured and you want to join the cluster to your on-premises Active Directory Domain.

***Note***: Make sure you have enabled **service endpoint for Azure SQL Database(Microsoft.Sql)** on the subnet in which you want to create the cluster.

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FAzure%2Fhpcpack-template%2Fmaster%2FHPCPack2019%2Fnewcluster-templates%2Ftwo-hns-wincn-existing-ad-sqlazure.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>

### Template 4: Single head node cluster for Windows workloads with new Active Directory Domain

This template deploys an HPC Pack cluster with one **single** head node for Windows HPC workloads in Active Directory Domain forest. The cluster includes one domain controller, one **single** head node with local databases (SQL server 2019 Express version), and a configurable number of **Windows** compute nodes.

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FAzure%2Fhpcpack-template%2Fmaster%2FHPCPack2019%2Fnewcluster-templates%2Fsingle-hn-wincn-ad.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>

### Template 5: Single head node cluster for Windows workloads with existing Active Directory Domain

This template deploys an HPC Pack cluster with one **single** head node for Windows HPC workloads in an existing Active Directory Domain forest. The cluster includes one **single** head node with local databases (SQL server 2019 Express version), and a configurable number of **Windows** compute nodes. You can choose not to create public IP address for the head node if you have a virtual network with Express Route configured and you want to join the cluster to your on-premises Active Directory Domain.

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FAzure%2Fhpcpack-template%2Fmaster%2FHPCPack2019%2Fnewcluster-templates%2Fsingle-hn-wincn-existing-ad.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>

### Template 6: Single head node cluster for Linux workloads with existing Active Directory Domain

This template deploys an HPC Pack cluster with one **single** head node for Windows HPC workloads in an existing Active Directory Domain forest. The cluster includes one **single** head node with local databases (SQL server 2019 Express version), and a configurable number of **Linux** compute nodes. You can choose not to create public IP address for the head node if you have a virtual network with Express Route configured and you want to join the cluster to your on-premises Active Directory Domain.

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FAzure%2Fhpcpack-template%2Fmaster%2FHPCPack2019%2Fnewcluster-templates%2Fsingle-hn-lnxcn-existing-ad.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>

---
## Following templates are NOT Active Directory Domain integrated

### Template 1: High-availability cluster for Windows workloads

This template deploys an HPC Pack cluster with high availability for Windows HPC workloads. The cluster includes **two** head nodes, one Database Server with SQL Server 2016 Standard version, and a configurable number of **Windows** compute nodes.

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FAzure%2Fhpcpack-template%2Fmaster%2FHPCPack2019%2Fnewcluster-templates%2Ftwo-hns-wincn-noad.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>

### Template 2: High-availability cluster for Linux workloads

This template deploys an HPC Pack cluster with high availability for Windows HPC workloads. The cluster includes **two** head nodes, one Database Server with SQL Server 2016 Standard version, and a configurable number of **Linux** compute nodes.

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FAzure%2Fhpcpack-template%2Fmaster%2FHPCPack2019%2Fnewcluster-templates%2Ftwo-hns-lnxcn.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>

### Template 3: Single head node cluster for Windows workloads

This template deploys an HPC Pack cluster with one **single** head node and a configurable number of **Windows** compute nodes. The head node is with local databases (SQL server 2019 Express version).

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FAzure%2Fhpcpack-template%2Fmaster%2FHPCPack2019%2Fnewcluster-templates%2Fsingle-hn-wincn-noad.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>

### Template 4: Single head node cluster for Linux workloads

This template deploys an HPC Pack cluster with one **single** head node and a configurable number of **Linux** compute nodes. The head node is with local databases (SQL server 2019 Express version).

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FAzure%2Fhpcpack-template%2Fmaster%2FHPCPack2019%2Fnewcluster-templates%2Fsingle-hn-lnxcn.json" target="_blank">
    <img src="http://azuredeploy.net/deploybutton.png"/>
</a>

---
## <a name="prerequisites"></a>Pre-Requisites:

### 1. Prepare a PFX certificate

Microsoft HPC Pack 2019 cluster requires a Personal Information Exchange (PFX) certificate to secure the communication between the HPC nodes. The certificate must meet the following requirements: 1.Have a private key capable of **key exchange**; 2.Key usage includes **Digital Signature** and **Key Encipherment**; 3.Enhanced key usage includes **Client Authentication** and **Server Authentication**.You can generate a self-signed certificate which meets the requirements with the following commands and export it as a PFX certificate.

For operating system **Windows 10, Windows Server 2016, or Windows Server 2019**, just run the built-in ***New-SelfSignedCertificate*** command as following:

```PowerShell
New-SelfSignedCertificate -Subject "CN=HPC Pack Node Communication" -KeySpec KeyExchange -TextExtension @("2.5.29.37={text}1.3.6.1.5.5.7.3.1,1.3.6.1.5.5.7.3.2") -CertStoreLocation cert:\CurrentUser\My -KeyExportPolicy Exportable -HashAlgorithm SHA256 -NotAfter (Get-Date).AddYears(5) -NotBefore (Get-Date).AddDays(-1)
```

For operating system **earlier than Windows 10 or Windows Server 2016**, you can download the [Self-signed certificate generator](https://gallery.technet.microsoft.com/scriptcenter/Self-signed-certificate-5920a7c6/) from Microsoft Script Center. Extract its contents and run the following command.

```PowerShell
Import-Module -Name c:\ExtractedModule\New-SelfSignedCertificateEx.ps1
New-SelfSignedCertificateEx -Subject "CN=HPC Pack Node Communication" -KeySpec Exchange -KeyUsage "DigitalSignature,KeyEncipherment" -EnhancedKeyUsage "Server Authentication","Client Authentication" -StoreLocation CurrentUser -SignatureAlgorithm SHA256 -Exportable -NotAfter (Get-Date).AddYears(5) -NotBefore (Get-Date).AddDays(-1)
```

### 2. Upload the certificate to Azure Key Vault 

Before deploying the HPC cluster, you shall import the PFX certificate as an **Azure Key Vault certificate**. The Azure Key Vault must be in the same location where you plan to deploy your HPC cluster.

You can create an Azure Key Vault and import the PFX certificate manually on [Azure Portal](https://portal.azure.com), make sure to check the two options ***Enable access to Azure Virtual Machines for deployment*** and ***Enable access to Azure Resource Manager for template deployment*** in ***advanced access policies*** when you create the Azure Key Vault.

Or you can [install Azure PowerShell module](https://docs.microsoft.com/en-us/powershell/azure/install-az-ps) in your computer and refer to the PowerShell script as below to create the Azure key vault and import the certificate. 

Remember the following information which will be used in deployment: key vault name, resource group name, secret Id, and certificate thumbprint. 

```PowerShell
#Give the following values
$VaultName = "mytestvault"
$CertName = "hpcpfxcert"
$VaultRG = "myresourcegroup"
$location = "westus"
$PfxFile = "c:\Temp\mytest.pfx"
$Password = "yourpfxkeyprotectionpassword"
#Validate the pfx file
try {
    $pfxCert = New-Object System.Security.Cryptography.X509Certificates.X509Certificate2 -ArgumentList $PfxFile, $Password
}
catch [System.Management.Automation.MethodInvocationException]
{
    throw $_.Exception.InnerException
}
$pfxCert.Dispose()
$rg = Get-AzResourceGroup -Name $VaultRG -Location $location -ErrorAction SilentlyContinue
if($null -eq $rg)
{
    $rg = New-AzResourceGroup -Name $VaultRG -Location $location
}
$hpcKeyVault = New-AzKeyVault -Name $VaultName -ResourceGroupName $VaultRG -Location $location -EnabledForDeployment -EnabledForTemplateDeployment
$secpass = ConvertTo-SecureString -String $Password -AsPlainText -Force
$keyVaultCert = Import-AzKeyVaultCertificate -VaultName $VaultName -Name $CertName -FilePath $PfxFile -Password $secpass
"The following Information will be used in the deployment template"
"Vault Name             :   $VaultName"
"Vault Resource Group   :   $VaultRG"
"Certificate URL        :   $($keyVaultCert.SecretId)"
"Certificate Thumbprint :   $($keyVaultCert.Thumbprint)"
```