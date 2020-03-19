# AzureTips For WebAppService and Docker

Debugging
During the research I used Kudu a lot for debugging. Kudu is not a security tool, but it is indeed very useful debugging tool.

For each Azure web app, which may contain a single function or more, there is a corresponding Kudu website to debug and manage the functions. Kudu was developed by Microsoft and it allows debugging of both Windows and Linux based functions. It is accessed by browsing https://*.scm.azurewebsites.net where the wildcard is your web app name.

With Kudu, you can download Docker logs, browse your home directory files (the shared directory), see your function Git endpoint and much more. Kudu functionality varies between Windows and Linux environment, as the deployment and features of Azure Functions also varies when changing operating system.

Most of Kudu’s functionality is exported using REST API.

# AzureTips 

And the source on GitHub here: 
https://github.com/Microsoft/AzureTipsAndTricks
https://www.michaelcrump.net/azure-tips-and-tricks-sorted-list/
You can find them as a browsable UI here: http://azuredev.tips

# AzureTips - How to know a new Service ?

A good point to start is the Azure Service Catalog: 
  https://azure.microsoft.com/en-us/services/

Samples: 
  https://azure.microsoft.com/en-us/resources/samples/

Videos: 
  https://azure.microsoft.com/en-us/resources/videos/index/
Let’s take the example of the “Azure Application Gateway”. I will show you a couple of artifacts that exist for most of the Azure services but usually are scattered around the internet. Knowing that they exist and what they are helps you look for the information you need. I will use the application gateway as an example, but you can of course use the same idea for any other service.


# AzureBookmark
All necessary links and tips &amp; tricks on Azure Services

**Microsoft Azure**

Version d’évaluation de Microsoft Azure
http://azure.microsoft.com/fr-fr/pricing/free-trial/

Azure Services Reference Map
https://nnmer.github.io/azure-services-map/dist/

Les services d’Azure présentés comme une table périodique des éléments
http://www.concurrency.com/landing/azure-periodic-table

Azure InfoHub avec les flux RSS liés à Azure, le lien pour suivre l’actualité Azure
http://aka.ms/azureinfohub

Voir les régions Azure disponibles et prévues
https://azure.microsoft.com/en-us/regions/

Voir la disponibilité des services Azure par région
https://azure.microsoft.com/fr-fr/regions/#services

Cloud Platform roadmap
https://www.microsoft.com/en-us/cloud-platform/roadmap-recently-available

Azure Preview features –> pour tester en beta les futurs services https://azure.microsoft.com/en-us/services/preview/

Azure product updates, roadmap, and announcements
https://azure.microsoft.com/en-us/updates/

Proposer des nouvelles fonctionnalités ou faire un feedback directement aux équipes produits d’Azure (Uservoice)
http://feedback.azure.com

Microsoft Azure Speed test : déterminez votre Datacenter Azure le plus proche
http://azurespeedtest.azurewebsites.net/

Encore mieux que l’outil précédent avec les latences sur pleins de services et plein d’autres outils
http://www.azurespeed.com/

Azure speed test tool for PowerShell
https://github.com/devblackops/AzSpeedTest

Où sont stockées mes données Azure? : http://azuredatacentermap.azurewebsites.net/ ou
http://o365datacentermap.azurewebsites.net/

Correspondance entre les services Microsoft Azure et Amazon Web Services
https://azure.microsoft.com/en-us/campaigns/azure-vs-aws/mapping/

**— Combien ça coûte Azure —**

Calculatrice des coûts Azure
http://azure.microsoft.com/en-us/pricing/calculator/

Azure Price Calculator (intéressant pour du calcul bulk de plusieurs VM)
https://azprice.info/ (merci à Florent Point pour le lien)

Microsoft Azure Total Cost of Ownership (TCO) Calculator
http://aka.ms/azure-tco-calculator

Azure Usage And Billing Portal
https://github.com/Microsoft/AzureUsageAndBillingPortal

**— Outils d’administrations Azure —**

Le portail d’administration classic de Microsoft Azure :
https://manage.windowsazure.com

le portail d’administration
https://portal.azure.com/

Portail Azure en mode preview
https://preview.portal.azure.com/

Microsoft Azure Enterprise Portal
https://ea.azure.com

Module Azure PowerShell :
https://github.com/Azure/azure-powershell/releases

How to install and configure Azure PowerShell
https://azure.microsoft.com/en-us/documentation/articles/powershell-install-configure/

Note : pour Récupérer la version du module Azure PowerShell, exécuter la commande suivante :
PS c:\> (Get-Module Az -ListAvailable).Version

Azure CLI (client ligne de commande pour Linux, Mac OS X et Windows)
https://azure.microsoft.com/en-gb/documentation/articles/xplat-cli-install/

Azure CLI 2.0
https://github.com/Azure/azure-cli

Equivalence entre syntaxe Azure CLI et Azure CLI 2.0 : 
https://github.com/Azure/azure-cli/blob/master/doc/azure2az_commands.rst

Install Azure CLI 2.0
https://docs.microsoft.com/en-us/cli/azure/install-azure-cli?view=azure-cli-latest

Azure Cloud Shell bash
https://shell.azure.com/bash

Azure Cloud Shell PowerShell
https://shell.azure.com/powershell

Les outils disponibles dans la console Azure Cloud Shell : 
https://docs.microsoft.com/en-us/azure/cloud-shell/features#tools

Configurer un stockage persistant pour la console Azure Cloud Shell : 
https://docs.microsoft.com/en-us/azure/cloud-shell/persisting-shell-storage

Windows Azure AD PowerShell module (version 64 bits)
http://go.microsoft.com/fwlink/p/?linkid=236297

Scripts pour Azure
http://azure.microsoft.com/en-us/documentation/scripts/

Azure app pour iOS
https://itunes.apple.com/us/app/microsoft-azure/id1219013620?ls=1&mt=8

Azure app pour Android
https://play.google.com/store/apps/details?id=com.microsoft.azure

**— Azure Resource Manager —**

Azure Resource Explorer (Preview)
https://resources.azure.com

Azure Quickstart Templates (Azure Ressource Manager)
http://azure.microsoft.com/en-us/documentation/templates/

https://github.com/Azure/azure-quickstart-templates

Azure Resource Manager Template Visualiser
http://armviz.io/#

Migration des ressources IaaS ASM (Classic) vers le mode ARM (Azure Resource Manager)
http://aka.ms/classicmigration

migAz : outils de migration de ressources Azure
https://github.com/Azure/migAz

Azure Migrate : outil et service de migration vers Azure
https://docs.microsoft.com/en-us/azure/migrate/

**— Terraform et Azure —**

Azure Provider
https://www.terraform.io/docs/providers/azurerm/

Github provider Terraform Azurerm
https://github.com/terraform-providers/terraform-provider-azurerm

**— Surveillance d’Azure & OMS —**

Etat des services Azure
http://status.azure.com

Azure Operational Insights (OMS)
https://opinsights.azure.com/

Operational Insights pour Windows Phone
http://www.windowsphone.com/en-us/store/app/operational-insights/4823b935-83ce-466c-82bb-bd0a3f58d865

Microsoft OMS pour Android
https://play.google.com/store/apps/details?id=com.microsoft.operations.AndroidPhone&hl=en

Microsoft OMS pour iOS
https://itunes.apple.com/us/app/microsoft-operations-management/id1042424859

OMS Agent for Linux
https://github.com/Microsoft/OMS-Agent-for-Linux

OMS Agent Linux for Docker
https://github.com/Microsoft/OMS-docker#supported-linux-operating-systems-and-docker

Calculatrice des coûts OMS
http://oms-calculator-webapp.azurewebsites.net/home

La bible du language de requêtes d’Azure Log Analytic (OMS) : Azure Log Analytics Query Language
https://docs.loganalytics.io/index

**— Connexion au stockage Azure —**

Microsoft Azure Storage Explorer
http://storageexplorer.com/

Azure Explorer – a free Microsoft Azure storage tool
http://www.red-gate.com/products/azure-development/azure-explorer/

CloudBerry Explorer for Microsoft Azure Storage: Freeware Client
http://www.cloudberrylab.com/free-microsoft-azure-explorer.aspx

Veeam FastSCP for Microsoft Azure
https://www.veeam.com/blog/fastscp-microsoft-azure-available.html

Outil AzCopy
Pour Windows : http://aka.ms/downloadazcopy
Pour Linux : https://aka.ms/downloadazcopyprlinux

Troubleshooting tool for Azure Files mounting errors on Windows
https://gallery.technet.microsoft.com/Troubleshooting-tool-for-a9fa1fe5

**— Identité et Azure Active Directory —**

Assistant de connexion Microsoft Online Services
http://www.microsoft.com/fr-fr/download/details.aspx?id=41950

Azure AD Graph Explorer
https://graphexplorer.cloudapp.net/

Microsoft Graph Explorer
https://developer.microsoft.com/en-us/graph/graphexplorer

Portail d’administration d’Azure Active Directory
https://aad.portal.azure.com

Portail des applications utilisateurs (AAD Premium)
https://myapps.microsoft.com/

My Apps for Android
https://play.google.com/store/apps/details?id=com.microsoft.myapps

My Apps for iOS
https://itunes.apple.com/us/app/my-apps-windows-azure-active/id824048653?mt=8

Cloud App Discovery (AAD Premium)
http://appdiscovery.azure.com/

Azure AD Connect (Remplaçant de DirSync)
http://aka.ms/aadconnect

Azure Active Directory Connect Health
https://msdn.microsoft.com/en-us/library/dn906722.aspx

ADFS Help – Resolve authentication issues faster!
https://adfshelp.microsoft.com/

Portail d’enregistrement des utilisateurs pour le Self Service Password Reset (AAD Basic et Premium)
https://account.activedirectory.windowsazure.com/PasswordReset/Register.aspx

Portail de réinitialisation des mots de passe des utilisateurs Azure Active Directory (AAD Basic et Premium)
http://passwordreset.microsoftonline.com

Microsoft AppSource : find the right SaaS application for your business
https://appsource.microsoft.com/en-us/

**— Capacity Planning —**

Azure Site Recovery Capacity Planner
http://aka.ms/asr-capacity-planner-excel

Azure Backup – Storage capacity planner for IaaS virtual machine backup
https://gallery.technet.microsoft.com/Azure-Backup-Storage-a46d7e33

Capacity planner for Azure Backup
https://gallery.technet.microsoft.com/Capacity-planner-for-Azure-de6f1457

Azure DocumentDB – Estimate Request Units and Data Storage
https://www.documentdb.com/capacityplanner

**— Azure Security —**

Azure Penetration Security Form : formulaire à remplir avant de faire des tests de pénétration sur des workloads exécutés sur Azure
https://security-forms.azure.com/penetration-testing/terms

Azure PCI DSS 3.1 Responsibility Matrix 2016
https://gallery.technet.microsoft.com/Azure-PCI-DSS-Responsibilit-02d4b4b2

Azure Interactive – Security & operation management
http://azureinteractives.azurewebsites.net/AzureSecurity/default.html

**— Azure et réseaux —**

Microsoft Azure Datacenter IP Ranges & Services Tags https://www.microsoft.com/en-us/download/confirmation.aspx?id=56519

Azure Range : outil Web pour déterminer les plages IP de telle ou telle région Azure
http://iprange.omartin2010.com

Site Recovery service endpoint IP addresses (XML file)
https://aka.ms/site-recovery-public-ips

  URL et Services associés<br/>
*.core.windows.net –> Stockage Azure<br/>
*.cloudapp.net –> Cloud Service, VM<br/>
*.msapproxy.net -> Azure AD Application Proxy<br/>
*.trafficmanager.net -> Azure Traffic Manager<br/>
*.onmicrosoft.com -> Identité, Azure AD<br/>
*.azurewebsites.net -> Sites Web<br/>
*.azure.com -> Azure Portal<br/>
*.windowsazure.com -> Azure Portal [Classic], Marketplace d’Azure<br/>
*.database.windows.net -> SQL Database<br/>
*.visualstudio.com -> Visual Studio Online<br/>
*.policykeyservice.dc.ad.msft.net Azure –> Azure Cloud App Discovery<br/>
*.hypervrecoverymanager.windowsazure.com –> Azure Site Recovery<br/>
*.backup.windowsazure.com –> Azure Backup<br/>
*.accesscontrol.windows.net<br/>
*.mms.microsoft.com –> Azure Logs Analytics (OMS)<br/>
*.vault.azure.net –> Azure Key Vault<br/>
*.azurecr.io –> Azure Registry<br/>
*.redis.cache.windows.net ==> Cache Redis Azure<br/>
*.search.windows.net ==> Azure Search<br/>
*.azureedge.net ==> Azure CDN Standard Verizon<br/>
*.azure-api.net ==> Azure API Management<br/>
dev.azure.com/* ==> Azure DevOps<br/>
login.microsoftonline.com ==> authorization & authentication<br/>
*.servicebus.windows.net ==> Service Bus<br/>
*.azurecr.io ==> Azure Container Registry<br/>
*.azmk8s.io ==> Azure Kubernetes Service<br/>
*.bastion.azure.com ==> Azure Bastion<br/>

**— Architectures de référence —**

Azure Interactive Cloud Pattern to solve design problems
http://azureinteractives.azurewebsites.net/CloudDesignPatterns/default.html

An great online app to create Azure architecture diagrams (if you don’t have Visio)
https://github.com/cloudskew/cloudskew/blob/master/readme.md

**— Intelligence Artificielle —**

Language Understanding Intelligence Service (LUIS)
https://www.luis.ai/home

Q&A Maker
https://www.qnamaker.ai/

**- Microsoft Intune -**

Version d’évaluation 30 jours de Microsoft Intune :
http://www.microsoft.com/fr-fr/server-cloud/products/windows-intune/try.aspx

Portail d’administration de Microsoft Intune :
https://manage.microsoft.com/ et https://account.manage.microsoft.com

Page d’accueil des utilisateurs Microsoft Intune :
https://portal.manage.microsoft.com/

Microsoft Intune Service health Status
http://status.manage.microsoft.com/StatusPage/ServiceDashboard

Portail Intune pour l’éducation (Merci à JP)
https://intuneeducation.portal.azure.com

**— Azure DevOps —**

Azure Devops portal
https://dev.azure.com

Azure DevOps Status page
https://status.dev.azure.com/

**- Office 365 -**

Version d’évaluation 30 jours d’Office 365 Entreprise E3 :
http://office.microsoft.com/fr-fr/business/microsoft-office-365-entreprise-e3-FX103030346.aspx

Portail d’administration Office 365
https://portal.microsoftonline.com/

Nouveau portail d’administration Office 365 [Preview]
https://portal.office.com/

Procédure pour accéder à la console d’administration Azure AD avec un compte AAD ayant les droits Admin Global (créé au préalable dans Office 365, AAD..)
https://account.windowsazure.com/signup?offer=MS-AZR-0110P [Source : Register your free Azure Active Directory subscription https://technet.microsoft.com/en-us/library/dn832618.aspx ]

Page d’accueil des utilisateurs Office 365
https://login.microsoftonline.com/

Outlook Web Access Office 365
https://outlook.office365.com/owa/

Microsoft PowerBI
http://app.powerbi.com

Portail Azure RMS (Rights Management Services)
https://portal.aadrm.com/

Microsoft Remote Connectivity Analyzer (Merci à Flavien)
https://testconnectivity.microsoft.com/

Office 365 service health status
http://status.office365.com/

Office 365 Status (Twitter Officiel, plus efficace que toutes la console ci dessus)
https://twitter.com/Office365Status

Centre de sécurité et conformité (merci à Flavien)
https://protection.office.com

Fix Outlook account problems in Office 365 – Automatically diagnose and fix Outlook issues (Merci à Flavien)
https://portal.office.com/support/help.aspx?sid=sara&ui=en-US&rs=en-US&ad=US#/330cfd4a-358a-47fc-a679-71c762039f09

Vérifications de l’intégrité, de la disponibilité et de la connectivité d’Office 365 (Merci à Flavien)
https://configure.office.com/Scenario.aspx?sid=11

Office 365 Best Practices Analyzer for Exchange Server 2013
https://community.office365.com/en-us/w/deploy/office-365-best-practices-analyzer-for-exchange-server-2013(merci à Flavien)

PowerShell for Office 365
http://powershell.office.com/

La roadmap (Merci à Patrick et Nicolas)
http://office.com/roadmap

Description du service (par plan) (Merci à Patrick et Nicolas)
http://O365SD.com

LE point d’entrée Yammer (Merci à Patrick)
http://www.yammer.com

Produits Office pour OS mobiles (Merci à Patrick)
https://products.office.com/en-GB/mobile

BlackBerry Business Cloud Services pour Microsoft Office 365 (Merci à Flavien)
Portail pour les administrateurs : https://businesscloud.blackberry.com/Office365/webconsole
Portail pour les utilisateurs sur Blackberry : https://businesscloud.blackberry.com/office365/webdesktop

URL et plages d’adresses IP Office 365
https://support.office.com/fr-fr/article/URL-et-plages-d-adresses-IP-Office-365-8548a211-3fe7-47cb-abb1-355ea5aa88a2

IFTTT Microsoft’s Recipes
https://ifttt.com/p/microsoft/shared

Office 365 Planner
https://tasks.office.com/

Office 365 Advanced Security Management
*.adallom.com

Assistant Configuration Exchange hybride
https://configure.office.com/Scenario.aspx?sid=13

Microsoft Stream
https://stream.microsoft.com

Microsoft Azure Information Protection
http://aka.ms/getaip

Centre d’administration OneDrive
https://admin.onedrive.com

Microsoft School Data Sync
https://sds.microsoft.com/

Microsoft Teams
https://teams.microsoft.com

Microsoft Forms
https://forms.office.com/

**- PowerBI -**

Portail PowerBI
https://powerbi.microsoft.com/

Support PowerBI – statut des services
https://powerbi.microsoft.com/fr-fr/support/

**- Windows 10 -**

Windows Store for Business
https://businessstore.microsoft.com

Pour connaître les builds Windows (10, Server, IoT..) de chaque programme (Insider, Preview…)
http://changewindows.org/

Portail Windows Defender Advanced Threat Protection
http://securitycenter.windows.com

