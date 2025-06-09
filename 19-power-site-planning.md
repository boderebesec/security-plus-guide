# Power & Site Planning — Domain 3: Security Architecture

Topic: Environmental Controls, Site Planning, and Power Resilience  
Domain: 3.0 Security Architecture

---

## Purpose of Security Architecture

Security architecture principles and controls are designed to protect data and resources across different environments—Cloud, Network, Virtualization, IoT, and SCADA—by reducing risk, enforcing segregation, and enabling continuous monitoring.

---

## 1. Environmental Controls & Site Planning

Effective site planning ensures the safety and availability of critical infrastructure, especially in high-risk or regulated environments.

### Physical Considerations
- Location Risk Assessment: Evaluate threats like earthquakes, floods, and civil unrest  
- Facility Hardening: Reinforced structures, limited external windows, shielded server rooms  
- Perimeter Security: Fencing, security personnel, CCTV, layered badge access  
- Zoned Access: Separate sensitive areas from general-purpose facilities  

### Environmental Systems
- HVAC: Maintains temperature and humidity for optimal hardware function  
- Fire Suppression  
  - Clean Agent Systems (e.g., FM-200, Novec 1230): Non-damaging to electronics  
  - Water-Based Sprinklers: Secondary systems for broader emergencies  
- Leak Detection: Protects against HVAC or infrastructure-related flooding  
- Air Filtration: Prevents dust buildup and hardware degradation  

---

## 2. Power Redundancy & Electrical Resilience

Power infrastructure is a core element of physical security and uptime assurance.

### Power Infrastructure
- Dual Power Feeds: Separate utility lines reduce risk of total failure  
- Power Distribution Units (PDUs): Distribute power and monitor load levels  
- Grounding: Prevents electrical surges from damaging sensitive equipment  
- Surge Protection: Guards against spikes from lightning or grid instability  

### Backup Power Systems
- Uninterruptible Power Supply (UPS): Immediate power during outages for short-term continuity  
- Generators: Fuel-based backup that activates during longer outages  
- Automatic Transfer Switches (ATS): Shift power source from utility to backup automatically  
- Battery Testing: Ensures backup systems meet expected runtime and discharge capacity  

---

## 3. Resilience Strategies

Layered resilience helps prevent downtime and strengthens disaster recovery capacity.

- Power Load Balancing: Distribute electrical load evenly to prevent single-point overload  
- Monitoring and Alerting: Real-time alerts for overheating, power usage, and air quality  
- Routine Maintenance: Periodic inspections of HVAC, batteries, and fire suppression systems  
- Policy Enforcement: Document safety checks and risk assessments  

---

## Summary Table

| Area                  | Key Focus                         | Tools / Measures                              |
| ----------------------| --------------------------------- | ----------------------------------------------|
| Site Planning         | Physical and environmental safety | Location assessment, hardening, CCTV, zoning  |
| Power Resilience      | Continuous energy delivery        | UPS, generators, dual feeds, surge protection |
| Operational Readiness | Failure prevention & recovery     | Monitoring, maintenance, policy enforcement   |

---

## References

- NIST SP 800-12 Rev. 1: An Introduction to Information Security  
  https://csrc.nist.gov/publications/detail/sp/800-12/rev-1/final

- CompTIA Security+ SY0-701 Exam Objectives  
  https://www.comptia.org/en-us/certifications/security/#objectives

- TIA-942 Data Center Standards: Infrastructure Guidelines  
  https://tiaonline.org/resources/tia-942-data-center-standards/

- NIST SP 800-34 Rev. 1: Contingency Planning Guide  
  https://csrc.nist.gov/publications/detail/sp/800-34/rev-1/final  
