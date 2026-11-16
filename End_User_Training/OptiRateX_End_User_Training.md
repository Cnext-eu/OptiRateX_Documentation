# <img src="OptiRateX_End_User_Training.assets/jira-logo-scaled.png" alt="Manuport Logistics" width="210" style="float:left; margin:0 28px 12px 0;">Training for OptiRateX

Co-created with <img src="OptiRateX_End_User_Training.assets/kairos-logo-blue.png" alt="karios" width="100" style="margin:0 5px 5px 0;">by <img src="OptiRateX_End_User_Training.assets/cnext-logo.png" alt="CNEXT" width="100" style="margin:0 10px 5px 0;">

## To do

- Check against Business Requirements to ensure that
  - Bugs are being resolved
  - All Requirements in scope are included
  - No extra Requirements
- Flows
- Screens > Claude-scan the application 
- Desired outcomes

## Introduction

Phase 1 BIG 

Context diagram

## Buy Rate Configuration

**Roles:** `Cost Rate Administrator`

### Service Definition

### Selected Drivers

### Vocabulary for ManuPort Logistic

## Buy Rate Ingestion & Updating

**Roles:** `Procurement` `Cost Rate Administrator`

### Smart AI Import

#### Requirements

| Issuecode | Samenvatting                                                 |
| --------- | ------------------------------------------------------------ |
| ORX-89    | How to ingest a Driver with Knowledge  (ex: Barge types)?    |
| ORX-3     | [Analysis] XML ingestion (TenderEasy  automated import) - Tender process |
| ORX-1     | Sales role should be able to ingest  tariffs that will be auto approved |
| ORX-2     | Excel ingestion (multiple supplier  templates)               |

#### Steps

```mermaid

flowchart LR
    A[Receive<br>buy rate sheet] --> B[Choose saved<br>import configuration]
    B --> C[Import and<br>validate]
    C --> D{Valid?}
    D -- No --> E[Correct sheet<br>or mapping]
    E --> C
    D -- Yes --> F[Review<br>buy rate state]
    F --> G[Activate<br>buy rates]
    G --> H[Apply<br>surcharge updates]
    C -.-> L[(Import<br>audit log)]
    H -.-> L 

```

#### Forms

![Smart AI 1](OptiRateX_End_User_Training.assets/Smart_AI_1.png)

![Smart AI 2](OptiRateX_End_User_Training.assets/Smart_AI_2.png)

![Smart AI 3](OptiRateX_End_User_Training.assets/Smart_AI_3.png)

#### Desired Outcomes

### Buy Rate Sheets

### Buy Rate State

### Import Audit Log

### Saved Import Configurations

### Surcharge Updates

## Buy Rate Search & Comparison

**Roles:** `Sales` `Operations`

### Buy Rate Lookup

### Compare Buy Rates

### Compare Spot Rates

### Buy Rate History