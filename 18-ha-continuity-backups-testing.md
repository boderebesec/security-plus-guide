# High Availability, Continuity, Backups, and Testing — Domain 3: Security Architecture

Topic: HA, Business Continuity, Backup Strategies, and Resilience Testing  
Domain: 3.0 Security Architecture

---

## Purpose of Security Architecture

Security architecture principles and controls are designed to protect data and resources across different environments—Cloud, Network, Virtualization, IoT, and SCADA—by reducing risk, enforcing segregation, and enabling continuous monitoring.

---

## 1. High Availability (HA) & Site Considerations

High availability ensures uninterrupted system functionality and minimizes downtime during disruptions.

**Key Components:**
- **Load Balancing:** Distributes traffic evenly across multiple servers to avoid overload  
- **Clustering:** Enables redundancy by having nodes take over tasks if one fails  
- **Site Types:**  
  - **Hot Site:** Immediate failover capability  
  - **Warm Site:** Partial readiness; requires configuration  
  - **Cold Site:** Infrastructure available but not pre-configured  
- **Geographic Dispersion:** Use of geographically diverse sites for resilience  

---

## 2. Continuity of Operations & Capacity Planning

### Business Continuity

A robust continuity strategy ensures operations persist with minimal disruption during crises.

**Key Practices:**
- **Disaster Recovery Planning:** Data restoration and redundancy strategies  
- **Cybersecurity Measures:** Protect digital systems against breaches  
- **Cloud & Remote Work Enablement:** Support flexibility during disruptions  
- **Testing:** Validate readiness through drills and assessments  

### Capacity Planning

Effective capacity planning addresses:  
- **People:** Staffing levels, training, and skills alignment  
- **Technology:** Scalable infrastructure, network capacity, and storage  
- **Infrastructure:** Datacenter and cloud capabilities to support growth and emergencies  

---

## 3. Backup Strategies

Backup systems ensure data recovery and continuity.

**Core Components:**
- **Onsite vs Offsite:**  
  - **Onsite:** Fast restoration but vulnerable to local disasters  
  - **Offsite:** Protection from environmental threats, often cloud-based  
- **Frequency:** From real-time (critical data) to weekly (less sensitive data)  
- **Encryption:** Protect backups during storage and transfer  
- **Snapshots:** Capture system states for point-in-time recovery  
- **Replication:** Mirror data across multiple systems or locations  
- **Journaling:** Track changes to optimize incremental backups  
- **Recovery Testing:** Ensure the backup system works as expected  

---

## 4. Resilience & Disaster Testing

Testing validates security architecture resilience.

**Testing Methods:**
- **Tabletop Exercises:** Simulated discussions to prepare for incidents  
- **Failover Testing:** Verify systems maintain security during switchover  
- **Simulations:** Controlled emulations of real-world threats to identify gaps  
- **Parallel Processing:** Concurrent security assessments for efficiency and depth  

---

## Summary Table

| Area              | Key Focus                    | Implementation Tools                               |
| ----------------- | ---------------------------- | -------------------------------------------------- |
| High Availability | Load balancing, clustering   | Clusters, geographic distribution, failover setups |
| Continuity        | Operations during disruption | DR plans, remote enablement, simulations           |
| Backups           | Recovery and data integrity  | Offsite storage, encryption, journaling            |
| Testing           | Preparedness and validation  | Tabletop exercises, simulations, failover tests    |

---

## References

- 7 Factors to Consider in Network Redundancy Design: https://www.techtarget.com/searchnetworking/tip/7-factors-to-consider-in-network-redundancy-design
- What is Business Continuity and Why is it Important?: https://www.techtarget.com/searchdisasterrecovery/definition/business-continuity
- CompTIA Guide to Business Continuity and Data Recovery: https://connect.comptia.org/content/guides/comptia-quick-start-guide-to-business-continuity-and-data-recovery
- How to Conduct a Cyber-Resilience Assessment: https://www.techtarget.com/searchsecurity/tip/How-to-conduct-a-cyber-resilience-assessment