# start-safe-framework
Solutions Architect Framework for Enterprises (SAFE)

Initial thoughts...



1. Request (Recon)
    1. 5 User U's 
2. Requirements
    1. Functional
        1. Feature
        2. Flow (UX)
    2. Calculate
        1. Initial
        2. Network/Service
        3. Cost, quotas
    3. Non-functional
        1. Features/Limitations
        2. APIs/Data
        3. Flow (more detail)
        4. DevOps
    4. Extended
3. Review
4. Resolve
5. Realize

REQUEST and CLARIFY USERS
5 U's
1. U want the app to.... do what? (nutshell, 1min. pitch)
    1. User Problem -> Action -> Solution -> Benefit
    2. Simple no acronyms
2. User roles- types/roles/number of users?
3. UI - what five things on the nav menu?
4. UX, user paths, screens
5. User growth prospects

REQUIREMENTS

1. Functional (Business/UX) requirements
    1. Features
    2. Implementation details
2. Calculate requirements
    1. Network/Services
    2. Cost
3. Non-functional (system) requirements
    1. Features
    2. APIs/Data
    3. Implementation
    4. DevOps
4. Extended requirements

1. Functional requirements
    * User Features
        * Features itemized
        * Expansion of 5Us
    * Implementation
        1. User stories
        2. User routes
        3. UI/UX must-haves
        4. Compliance/Org req.
        5. Business rules (ie. prices, shipping, payment)

2. Calculate requirements: Calculation of constratins

* Initial Calculation flow:
    1. DAU (ie. 100mil)
    2. APU Actions per user/day (ie. 10)
    3. DAPU Total actions/day (ie. 1 billion/day)
    4. RPS - requests per second 1B/24hrs*3600sec.(86400)= 12k req/s
    5. Bandwidth consumed: 400GB/24hrsx3600 seconds = ~5MB/second
    6. Available Bandwidth = (Total Bandwidth - (Bandwidth consumed by other systems))
    7. Throughput = (Request per Second * Average Request Size)
    8. Network Latency = (Physical Distance / Speed of Light)
    9. CPU Utilization = (Total CPU Time / Total Time)
    10. Memory Utilization = (Used Memory / Total Memory)
    11. Disk I/O = (Number of Disk Reads + Number of Disk Writes) / Total Time
    12. Disk Throughput = (Disk I/O * Block Size) / Total Time
    13. Error rate = (Number of Errors / Total Requests)
    14. DB Storage 1B*400 bytes = 400GB/day
    15. DB 10years = 1.4PB
    16. Media Storage day/month/year

* Network & Service limitations
    * IPs
    * Bandwidth (req/alloc))
        * 1 billion requests per day translate into 12K requests per second.
    * Concurrency
        * More concurrency is better for availability, resiliency
    * Reliability model
        * DR Options: 
            * Starting from Low cost, Low RPO/RTO
            * Backup/Restore  < Pilot Light < Warm Standby < Mutli active/active 
        * DR - RPO -  Recovery Point Objective (RPO)
        * DR - RTO -  Recovery Time Objective (RTO)
        * Resiliency - MTBF - Mean Time Between Failures
        * Resiliency - MTTR - Mean Time to Recover
    * Latency
    * Thoroughput
        * 400 GB of ingress/day, require minimum bandwidth of around 4 MB per second
    * Storage
        * each message on average is 400 bytes, we will require about 400 GB of database storage every day
* Cost
    * Cost for each service
    * AWS Cost Explorer: visualize, understand, and manage your AWS costs and usage.
    * AWS Trusted Advisor:  recommendations for improving cost efficiency, performance, security, and fault tolerance.
    * AWS Budgets: set custom budgets that alert you when your costs or usage exceed your budgeted amount.
    * AWS Cost and Usage Report: detailed information about your AWS costs and usage.
    * AWS Application Cost Profiler
    * AWS Billing & Cost Management
    * AWS Pricing Calculator
    * Savings Plans
* AWS Resource Limitation
    * Quotas and limits
* Performance optimization
    * Read/write speed
    * Compute speed
    * Cold start

3. Non-functional requirements

* Features (technical)
    * Services:
        * IAM, 
        * Network, 
        * Compute, 
        * Storage, 
        * Database, 
        * Search, 
        * API, 
        * DevOps
        * Metrics/Logging
    * Limits (tech)
        * Organizational limits
        * Governance limits
        * Security limits
* APIs/DataModel
    * API: main types of requests
    * Data: main table or class names
* Implementation
    * UCROPS
    * Network - VPC, CDN, Edges, DNS, Hosting
    * Compute - server/serverless/container
    * Database - MySQL/NoSQL
    * Storage - file/block/object/archive

4. Extended requirements (future, nice to have)
    * Metrics
    * Security
    * DevOps

REVIEW

* TECH: 
    * Email outline to Team
* PM: 
    * Email outline to Product Manager
* LEADERSHIP
    * Validate with leadership
* CLIENT: 
    * After consensus, email outline to Project Owner

RESOLUTION

* Final agreement
* Working contract
* API contracts
* Staffing
* Cost contracts
* Timelines


REALIZE
* Implementation
* Tech lead role
