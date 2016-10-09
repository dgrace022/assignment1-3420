##Entities
**Developer:** A person that submits an open source software package to be checked for licenses and vulnerabilities. The developer can also make a request for software project license and vulnerability information, as well as policy information.

**Manager:** A person that like the developer, can make a request for software project license and vulnerability information and policy information. Unlike the developer, the manager is capable of adding new policies and modifying old policies. 
##Datastores
**OSS Results Database:** A database that stores all submitted open source software packages, along with license and vulnerability information.

**NIST Vulnerability Database:** A database that has information about all known vulnerabilities in submitted software. 

**Policy Database:** A database that holds information about the policies on the use of open source software for the business that implements this system.
##Processes
**Manage OSS Package for Vulnerability Checking:** This process accepts an oss package from Manage OSS Package for Licenses Scanning, Vulnerability Checking process, extracts the name of the oss package, sends the name to the NIST Vulnerability Database, and takes the vulnerability results and sends it back to Manage OSS Package for Licenses Scanning, Vulnerability Checking process.

**Manage OSS Package for Licenses Scanning, Vulnerability Checking:** This process accepts an oss package from a developer, and sends it to Manage OSS Package for Vulnerability Checking process and Scan for OSS Licenses process and accepts the results from both processes. It the sends these results to the OSS Results Database and back to the developer.

**Scan for OSS Licenses:** This process accepts an oss package from the Manage OSS Package for Licenses Scanning, Vulnerability Checking process and scans the package to find all the licensing in it. It then sends the oss package license results back to the Manage OSS Package for Licenses Scanning, Vulnerability Checking process.

**Query OSS Package License, Vuln. Information:** This process accepts a Software Project License and Vulnerability Information Request from either the developer or the manager, and sends it to the OSS Results Database, which it then recieves a Software Project License and Vulnerability Information Response and sends it back to the entity that made the request.

**Query Policy Database:** This process accepts a Policy Information Request from either the developer or the manager, and sends it to the Policy Database, which it then recieves a Policy Information Response and sends it back to the entity that made the request.

**Add or Modify Policy Database:** This process accepts either a new policy or modified policy from the Manager, to which it then sends it to the Policy Database.

##Data Flows
**OSS Package:** This is the open source software package the developer sends to the Manage OSS Package for Licenses Scanning, Vulnerability Checking process, so that it can be scanned for licenses and vulnerabilities.

**OSS Package License Result:** This is the data that comes back from the Scan for OSS Licenses process which contains information about all the licenses an oss package has.

**OSS Package Name:**

**Vulnerability Result:**

**OSS Package, License, & Vuln. Result:**

**Software Project License and Vulnerability Information Request:**

**Software Project License and Vulnerability Information Response:**

**Policy Information Request:**

**Policy Information Response:**

**New Policy:**

**Modified Policy:**
