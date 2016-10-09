# Use Case 1
**Title:** Determine Software Project License and Vulnerability Information

**Primary Actor:** Manager

**Goal in Context:** Manage is to retrieve software project license and vulnerability information.

**Stakeholders:** Manager, Developer

**Preconditions:** OSS Results Database is populated. NIST Vulnerability Database is up-to-date with current known vulnerabilities.

**Main Success Scenario:** Manager receives accurate software project license and vulnerability information.

**Failed End Conditions:** Manager recieves inaccurate software project license and vulnerability information. Manager does not recieve any information.

**Trigger:** Manager makes a request for software project license and vulnerability information.

# Use Case 2
**Title:** Add a New Policy

**Primary Actor:** Manager

**Stakeholders:** Manager, Developer

**Preconditions:** Policy Database is able to be accessed.

**Main Success Scenario:** A new policy is added to Policy Database.

**Failed End Conditions:** The Policy Database does not receive a new policy, and thus is not added.

**Trigger:** Manager submits a new policy.

# Use Case 3
**Title:** Determine Policy Information

**Primary Actor:** Developer

**Stakeholders:** Developer, Manager

**Preconditions:** The Policy Database is populated.

**Main Success Scenario:** The developer receives accurate policy information.

**Failed End Conditions:** The developer receives inaccurate policy information. The developer does not receive policy information at all.

**Trigger:** Developer makes a request for policy information.
