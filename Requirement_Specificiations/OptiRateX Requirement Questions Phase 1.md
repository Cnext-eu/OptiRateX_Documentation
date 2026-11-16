# <img src="../Common_Images/jira-logo-scaled.png" alt="Manuport Logistics" width="210" style="float:left; margin:0 28px 12px 0;">OptiRateX Requirements Phase 1

Co-created with <img src="../Common_Images/kairos-logo-blue.png" alt="karios" width="100" style="margin:0 5px 5px 0;">by <img src="../Common_Images/cnext-logo.png" alt="CNEXT" width="100" style="margin:0 10px 5px 0;"> 

### Not visible in the application

| Story                                          | What we found                                                | Question for the developer                                   |
| ---------------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| ORX-48 Approval workflow (also ORX-58, ORX-82) | 44,119 draft rates against 6,620 approved. Neither the demo nor the scan shows how a rate gets published. | How does Procurement approve: per rate, per selection or per batch? What does “automated validation” check? |
| ORX-36 / ORX-88 Spot (offline)                 | Spot offers come only from the live lookup; no way to upload a spot rate for other carriers. | How is an offline spot rate entered and recognised?          |
| ORX-91 / ORX-45 Service types                  | Customs, Container Actions (0 rates) and Value Added Service exist. No warehousing, rental, heating or THC service. | Which services will exist at go-live, and is THC a service or a surcharge? |
| Transport modes (contract)                     | Sea and road have rates; barge has a service with 0 rates; no air or rail. | Is there BIG data for barge, air and rail?                   |
| ORX-1 Sales ingest with auto-approval          | Not seen.                                                    | Is this built?                                               |
| ORX-73 / ORX-75 Regions                        | Nothing on carrier regions.                                  | How are regions handled in surcharge updates?                |

### Partly there, needs proof

- **ORX-68 / ORX-86 Charge codes:** the master list exists, but the backfill screen reports 183,739 surcharges still unmapped. Unmapped surcharges do not line up in Compare Rates. Initial Upload?
- **ORX-87 / ORX-99 Terminology:** two drivers are both named “Container Type” (CONTAINER and CONTAINER_TYPE), and the container filter in the lookup screenshot still showed raw values such as 20', 20'dv and 22G1.
- **ORX-70 “Supplier”:** the lookup screenshot still says “Provider”.
- **ORX-83:** the button is still called “Import Excel”.
- **ORX-61 Surcharge validity:** Rate state has a “Surcharges expiring” column, showing 0. Ask for an import that proves surcharges get their own validity.
- **ORX-67 Named Accounts:** the screen exists but holds no data.
- **ORX-89 Barge types:** the barge service has no rates, and the BIG barge test file was never run.

### Probably resolved, ask for confirmation

- **ORX-94 Large files:** two imports of 19,439 rates succeeded on 10 Nov.
- **ORX-85 Original source:** Rate History has a “Download source” button.
- **ORX-95 New drivers:** the service editor has “+ Create New Driver”.

Not checked on ORX-78 (intermediate save), ORX-79 (MSC DTHC parsing), ORX-76 (speed), ORX-62 (Rate state for all roles) or ORX-80 (access off-VPN).
