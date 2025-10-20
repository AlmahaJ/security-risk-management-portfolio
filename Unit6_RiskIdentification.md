# Unit 6 – Risk Identification (Pampered Pets)

## Why we used OCTAVE
OCTAVE fits small and medium businesses. It looks at important assets, key threats, and simple, low-cost fixes. It does not need a large security team.

## Main risks and fixes
1. **Shared Wi-Fi (staff and business)**  
   Risk: malware spreads and data can leak.  
   Fix: WPA3, separate SSIDs, strong passwords, change default router admin password.

2. **Warehouse spreadsheets on one old PC**  
   Risk: loss, errors, tampering.  
   Fix: move to a small database, turn on backups, restrict access, keep a restore test.

3. **Front-desk single machine for sales and tax**  
   Risk: one failure stops sales.  
   Fix: patch OS, use EDR/antivirus, least privilege, create a disk image to restore fast.

4. **Email orders**  
   Risk: phishing and fraud.  
   Fix: staff training, email security filter, MFA on admin systems.

## Small risk table
| Risk                     | Impact | Likelihood | Treatment                          |
|--------------------------|:------:|:----------:|------------------------------------|
| Shared Wi-Fi             | High   |  Medium    | Segment networks; WPA3             |
| Old PC spreadsheets      | High   |  Medium    | Migrate to DB; backups; access ctl |
| Single sales PC          | High   |  Medium    | Patch; EDR; image restore          |
| Phishing on orders       | Medium |   High     | Training; filter; MFA              |

## Outcome
OCTAVE gave quick, practical wins the owner can apply soon.  
This set a base for deeper work later with ISO 31000 and NIST.
