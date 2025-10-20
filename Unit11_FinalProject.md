# Unit 11 – Digitalisation Risk (Pampered Pets)

## Scope
The business will add an online shop, an ERP system, new suppliers, and automated warehouses.  
VIP clients need trust in quality and uptime.

## Method used
- ISO 31000 for process and governance  
- NIST SP 800-30 for risk steps  
- NIST SP 800-34 for DR testing  
- Simple 12-month probability model for quality and supply risks

## Quality risks (12-month probabilities)
- Supplier quality variance: 10%  
- Cold-chain or storage fault: 6%  
- Mis-label or mis-pack: 8%  
- ERP/WMS data error: 4%  
- Cyber-triggered process change: 3%

**Chance of at least one major quality incident:** about **27%** (combined).

## Supply and availability risks (12-month probabilities)
- Weather or route block: 40%  
- Supplier failure or quality hold: 20%  
- Peak-season capacity shortage: 25%  
- Customs or regulatory hold: 15%  
- Cyber attack on supplier/3PL: 15%  
- Warehouse automation outage: 10%  
- Online shop platform outage: 5%

**Chance of at least one major supply disruption:** about **78%** (combined).  
With buffers, second suppliers, alternate routes, and better packs, this can drop to about **45–55%**.

## DR and availability design
Two regions active-active, health-checked DNS and CDN/WAF, stateless app tier in both regions, cross-region DB replication (seconds lag), encryption and least privilege.  
**Targets:** changeover < 1 minute; data loss window < 1 minute.  
**Tests:** quarterly failover; monthly tabletop.  
This supports GDPR Article 32 (resilience and restore).

## Business actions (priority)
1. Quality at source (supplier audits, retain samples, two-person label checks)  
2. Cyber basics (MFA, patching, EDR, segmentation; contract clauses for partners)  
3. Supply resilience (safety stock for top SKUs, second suppliers, extra peak capacity)  
4. Two-region DR (automatic failover, tested scripts, publish results)  
5. Live risk register (owners, dates, reviews, ISO 31000 cycle)
