# Data Flow Diagram Dictionary

## Entities
* Developer: Code developer in the company.
* Corporate Manager: Managers who makes decisions and evaluates policy infomation. 
* National Vulnerability Database: A US government Vulnerability data instution, manages the National Vulnerability Database.

## Database
* NIST:It carries the standards names for packages or files of software.  
* Policy database:It holds the all policy information of the copmany's info. 
* Risk database:It holds the information that could risk the software and could affect it 

## Processes
* Manager Code Stream: A central process that connects developer and manager, as well as others.
* Manage Project Information: A process that manage code and information for corporate manager.
* Manager Policy Information: A process that handles policy information comes and goes between policy database and corporate manager.
* License Control: This process checks the license and copyright of the code.
* Manager CPE Information: This process manages the CPE information between National Vulnerability Database and NIST.
* Update Risk Database: Process the update information to the Risk database.
* Manifest: Create the manifest information for a project.

## Data flows
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
* License Information & files: Update License and copyright informtion to the Risk database.

