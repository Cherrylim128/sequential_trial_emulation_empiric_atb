# Impact of different empiric AWaRe antibiotic treatment strategies

### Summary
This is a repository for the protocols of target trials, analysis plan and analysis code.

### Aim of the study
To evaluate the impact on 28-day mortality of different empiric AWaRe antibiotic treatment strategies

### Method
I emulated two target sequential trials:
1. Target trial 1 utilised the Infections in Oxfordshire Research Database (IORD) from the United Kingdom
2. Target trial 2 utilised data from a prospective surveillance study of HAI in a Thai tertiary hospital

#### Treatment strategy 
Three empiric antibiotic treatment arms in both target trial:
1. “continue empiric antibiotic treatment from the same AWaRe group”,
2. “step-down empiric antibiotic strategy”,  or
3. “step-up empiric antibiotic strategy”. 

Marginal structure model with inverse probability of censoring weights (IPCW) were fitted separately to each dataset to estimate 28-day mortality under different empiric antibiotic treatment strategies. Pre-defined time-fixed and time-varying confounders were selected based on directed acyclic graph (DAG) in the DAG.pdf file.

#### Definitions used
- Low-Watch antibiotics: all antibiotics under the “Watch” category of the AWaRe system, except carbapenems, linezolid and vancomycin
- High-Watch antibiotics included carbapenems, linezolid and vancomycin
- Step-down antibiotic strategy was defined if:
  i) switching from “high-Watch” to “low Watch” or “Access” antibiotic; or
  ii) switching from “low-Watch” to “Access” antibiotic
- Step-up antibiotic strategy was defined if:
  i) switching from “Access” to “Low-Watch” or “High-Watch) antibiotic; or
  ii) switching from “Low-Watch” to “High-Watch” antibiotic.

Detailed protocols of the two target trials and summaries of how the target trials are emulated using the two observational data sets are in the "Target trial 1 protocol" and "Target trial 2 protocol" files.
