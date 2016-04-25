# data flow digram 
![Bilby Stampede](https://cloud.githubusercontent.com/assets/17163853/14790530/452939d4-0ad7-11e6-9d60-7e038c364ec5.png)

# Entities relationship digram 
![Bilby Stampede](https://cloud.githubusercontent.com/assets/17163853/14790478/18b40186-0ad7-11e6-9722-96490e2f0a6c.png)


# DFD dictionary 
### Entities
* Developer: Code developer in the company.
* Corporate Manager: Managers who makes decisions and evaluates policy infomation. 
* National Vulnerability Database: A US government Vulnerability data instution, manages the National Vulnerability Database.

### Database
* NIST:It carries the standards names for packages or files of software.  
* Policy database:It holds the all policy information of the copmany's info. 
* Risk database:It holds the information that could risk the software and could affect it 

### Processes
* Manager Code Stream: A central process that connects developer and manager, as well as others.
* Manage Project Information: A process that manage code and information for corporate manager.
* Manager Policy Information: A process that handles policy information comes and goes between policy database and corporate manager.
* License Control: This process checks the license and copyright of the code.
* Manager CPE Information: This process manages the CPE information between National Vulnerability Database and NIST.
* Update Risk Database: Process the update information to the Risk database.
* Manifest: Create the manifest information for a project.

### Data flows
* Files: A file or package.
* CPE Info Response: CPE information from National Vulnerability Database.
* License and copyright Info Request: Ask License control for a license or copyright inspection.
* License and copyright Info Response: Information about license or copyright from license control.
* CPE response: A CPE information response from National Vulnerability Database.
* CPE request: A CPE information request to National Vulnerability Database.
* CPE File Info:  CPE information from National Vulnerability Database.
* CPE Info and File: Update the CPE information to the Risk database.
* CPE Info and File: Update the CPE information to the Risk database.
* Package Info Request: A package information request sent from corporate manager.
* Package Info Response: A package information response sent from Risk database.
* Project Info Ruquest: The request of project information from Risk database.
* Project Info Response: The reponse of project information from Risk database.
* Project Info: Sents the project information to the manifest.
* Project Manifest Result: The result of project manifest from manifest.
* Package Info: Sent the project information to the policy database.
* Project Info Request: Sent the request project information to the policy database.
* Policy Info Response: Response the policy information of project to corporate manager.

#Policy 
###Context:
     Setup to maintain vulnerability of project file minimal and unharmful for the corporate system.
    
###Thresthold:
    Thresthold will be set in accord with given context.

###Response:
    If file failed CVE score, reject the file until requirement is met.

###Policy ID

###Policy Name

###Policy Update date

###Policy Issuer

###Policy License

###Policy Comment
    
#Manaifest 
###Document
* Date: 
* Author: 
* Document License: 
* Comments: 

###Project
* Project Name:
* Submitter:
* Project code:

###Package
* Update Date: 
* Name:
* CVE:
* License: 
* CPE Information: 
* Size: 
* Location: 

#usecase #1

**Title:** Developer commits code to be examined for vulnerabilities

**Primary Actor:** Developer

**Goal in Context:** Gather vulnerabilities information for all external source code that is used by developers

**Stakeholders:** Developer / Manager

**Preconditions:** Developer is able to check in internal source code to vulnerability system. NIST vulnerability database is up to date.

**Main success Scenario:** Developer check in code and vunerability information is recorded to the Risk DB.

**Failed End Conditions:** Developer is unable to check in code. Checked in code is not checked for vulnerabilities, failing to update Risk DB.

**Trigger:** Code check in

#usecase #2

**Title:** Corporate managers set policy to control project vulnerabilities 

**Primary Actor:** Corporate Managers

**Goal in Context:** Set up a policy database and control project vulnerabilities. 

**Stakeholders:** Project manager and corporate managers.

**Preconditions:** Check project information for vulnerability and make sure it follows policy regulation.

**Main Success Scenario:** Project vulnerability information passed policy requirement 

**Failed End Conditions:** Project information failed policy requirement, represent a risk. 

**Trigger:** violated policy.

#usecase #3
**Title:** The manager checks the volurnibility of database in the system

**Primary Actor:** Corporate Managers

**Goal in Context:** avoid any issues might happen in the system 

**Stakeholders:** project manager and corporate manager

**Preconditions:** File/package information is in the License DB, Proper project information has been recovered

**Main Success Scenario:** Corporate manager reciecves formed license and vulnerability inforamtion for the requested project info

**Failed End Conditions:** Corporate manager recieved pooryly formed license and vulnerability inforamtion for the requested project information

**Trigger:** Corporate manager uploades project information to which license and vulnerability inforamtion is recovered from the License DB
