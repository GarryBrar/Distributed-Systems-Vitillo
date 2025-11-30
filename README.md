# Distributed-Systems-Vitillo: Understanding Distributed Systems Notebooks

This repository contains my working Jupyter Notebooks for the concepts, architectural patterns, and system design exercises found in the practical guide, **Understanding Distributed Systems**, by **Roberto Vitillo**.

The primary goal of this repository is to track my progress and provide practical implementations and simulations of the distributed algorithms discussed in the book, focusing on **Python**.

---

### 🗂️ Repository Structure (Aligned with the Book)

The notebooks and code files are organized into directories that correspond directly to the book's official parts and chapters:

| Folder | Part / Chapter Title |
| :--- | :--- |
| `01_Introduction` | Introduction & Anatomy of a distributed system |
| **Part I** | **Communication** |
| `02_Reliable_links` | Reliable links (TCP patterns, Flow control) |
| `03_Secure_links` | Secure links (TLS, Encryption, Handshakes) |
| `04_Discovery` | Discovery (DNS, Load balancing patterns) |
| `05_APIs` | APIs (REST, Idempotency, Evolution) |
| **Part II** | **Coordination** |
| `06_System_models` | System models (Synchronous vs Asynchronous) |
| `07_Failure_detection` | Failure detection (Heartbeats) |
| `08_Time` | Time (Physical, Logical, and Vector Clocks) |
| `09_Leader_election` | Leader election (Raft implementation) |
| `10_Replication` | Replication (Consensus, Chain replication) |
| `11_Coordination_avoidance` | Coordination avoidance (CRDTs, CALM theorem) |
| `12_Transactions` | Transactions (ACID, Isolation levels) |
| `13_Async_transactions` | Asynchronous transactions (Sagas, Outbox pattern) |
| **Part III** | **Scalability** |
| `14_HTTP_caching` | HTTP caching & Reverse proxies |
| `15_Content_delivery_networks` | Content delivery networks (CDNs) |
| `16_Partitioning` | Partitioning (Range vs Hash partitioning) |
| `17_File_storage` | File storage (Blob storage architecture) |
| `18_Network_load_balancing` | Network load balancing (L4 vs L7) |
| `19_Data_storage` | Data storage (NoSQL, Replication strategies) |
| `20_Caching` | Caching (Policies, Write-through vs Look-aside) |
| `21_Microservices` | Microservices & API Gateways |
| `22_Control_planes` | Control planes and data planes |
| `23_Messaging` | Messaging (Pub/Sub, Queues, Fault isolation) |
| **Part IV** | **Resiliency** |
| `24_Common_failures` | Common failure causes |
| `25_Redundancy` | Redundancy & Correlation |
| `26_Fault_isolation` | Fault isolation (Shuffle sharding, Bulkheads) |
| `27_Downstream_resiliency` | Downstream resiliency (Timeouts, Retries, Circuit Breakers) |
| `28_Upstream_resiliency` | Upstream resiliency (Load shedding, Rate limiting) |
| **Part V** | **Maintainability** |
| `29_Testing` | Testing (Simulation, Formal verification) |
| `30_CICD` | Continuous delivery and deployment |
| `31_Monitoring` | Monitoring (SLIs, SLOs, Alerts) |
| `32_Observability` | Observability (Logs, Traces) |
| `33_Manageability` | Manageability |
| `00_Utilities` | Helper functions and simulation drivers |

---

### ⚙️ Local Environment Setup

To run these simulations and notebooks locally, use the following recommended environment configuration.

1.  **Clone the repository:**

    ```bash
    git clone [https://github.com/](https://github.com/)[YourUsername]/UDS-Vitillo.git
    cd UDS-Vitillo
    ```

2.  **Create a virtual environment (Recommended):**

    ```bash
    conda create -n uds_env python=3.11
    conda activate uds_env
    ```

3.  **Install dependencies:**
    This project uses `simpy` for discrete-event simulation (to model consensus/network delays) and `graphviz` for visualizing system architectures.

    ```bash
    pip install jupyter matplotlib numpy simpy requests graphviz
    ```

4.  **Launch Jupyter Lab:**
    ```bash
    jupyter lab
    ```
