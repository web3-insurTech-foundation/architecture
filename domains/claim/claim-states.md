# Claim State
Claim state diagram, for the general insurance claim case, we detail out the process of a claim submission and execution.

Clearly there are many sub steps to this process

```mermaid
stateDiagram-v2
    [*] --> Created
    Created --> Pending
    Pending --> Submitted
    Submitted --> Validation
    Validation --> Approved
    Validation --> Rejected
    Rejected --> Pending
    Rejected --> Expired    
    Rejected --> Cancelled
    Approved --> Scheduled
    Scheduled --> Setup
    Setup --> Remediation
    Setup --> Scheduled
    Remediation --> Completed
    Remediation --> Scheduled
    Remediation --> Cancelled
    Completed --> Settled
    Settled --> [*]
    Cancelled --> [*]
    Expired --> [*]
```

As we explore the relationships between different Insurance Domains as they pertain to Claims (ie, and auto claim versus home property claim), there are nuances around legal requirements, risk evaluation, quality of work etc.