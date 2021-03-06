-----
##Use Case #1

**Title:** Developer commits code to be examined for vulnerabilities

**Primary Actor:** Developer

**Goal in Context:** Gather vulnerabilities information for all external source code that is used by developers

**Stakeholders:** Developer / Manager

**Preconditions:** Developer is able to check in internal source code to vulnerability system. NIST vulnerability database is up to date.

**Main success Scenario:** Developer check in code and vunerability information is recorded to the Risk DB.

**Failed End Conditions:** Developer is unable to check in code. Checked in code is not checked for vulnerabilities, failing to update Risk DB.

**Trigger:** Code check in

-----
##Use Case #2

**Title:** Corporate managers set policy to control project vulnerabilities 

**Primary Actor:** Corporate Managers

**Goal in Context:** Set up a policy database and control project vulnerabilities. 

**Stakeholders:** Project manager and corporate managers.

**Preconditions:** Check project information for vulnerability and make sure it follows policy regulation.

**Main Success Scenario:** Project vulnerability information passed policy requirement 

**Failed End Conditions:** Project information failed policy requirement, represent a risk. 

**Trigger:** violated policy.

-----
##Use Case #3

**Title:** The manager checks the vulnerability of database in the system

**Primary Actor:** Corporate Managers

**Goal in Context:** avoid any issues might happen in the system 

**Stakeholders:** project manager and corporate manager

**Preconditions:** File/package information is in the License DB, Proper project information has been recovered

**Main Success Scenario:** Corporate manager reciecves formed license and vulnerability inforamtion for the requested project info

**Failed End Conditions:** Corporate manager recieved pooryly formed license and vulnerability inforamtion for the requested project information

**Trigger:** Corporate manager uploades project information to which license and vulnerability inforamtion is recovered from the License DB
