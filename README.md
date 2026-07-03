# Mediledger 2.0

Mediledger 2.0 is a blockchain-based healthcare and pharmaceutical supply chain management system designed to detect counterfeit drugs while ensuring secure storage of patient medical records. The application combines blockchain, AI-based anomaly detection, Zero-Knowledge Proofs (ZKPs), and cloud computing to provide transparency, security, and traceability across the pharmaceutical supply chain.

The project was developed as part of the Cloud Architecture Design course and demonstrates the integration of decentralized technologies with AI and cloud infrastructure.

## Features

* Drug batch registration on Ethereum Sepolia
* Supply chain tracking with complete transfer history
* Counterfeit drug detection using Isolation Forest
* AI-powered risk assessment using Gemini API
* Secure medical record storage using Zero-Knowledge Proofs
* Off-chain storage using IPFS
* Cloud infrastructure simulation using CloudSim Plus
* Performance analysis and visualization

## Technologies Used

* Solidity
* Ethereum Sepolia Testnet
* IPFS
* Zero-Knowledge Proofs (zkSNARKs)
* Circom
* snark.js
* Python
* Isolation Forest
* Gemini 2.0 Flash API
* CloudSim Plus
* Java

## System Overview

The application consists of four major components:

### Blockchain Layer

* Registers drug batches on Ethereum.
* Stores ownership transfers on-chain.
* Maintains immutable transaction history.
* Stores commitments for medical records.

### AI Risk Detection

An Isolation Forest model detects anomalies in pharmaceutical data. The prediction is then passed to Gemini 2.0 Flash, which generates a detailed risk analysis report based on transaction history and detected anomalies.

### Medical Record Security

Medical records are stored securely using IPFS, while cryptographic commitments are stored on the blockchain. Zero-Knowledge Proofs ensure that records can be verified without revealing their contents.

### Cloud Infrastructure

CloudSim Plus is used to simulate deployment across multiple virtual machines and evaluate system performance under different workloads.

## Project Modules

### Drug Registration

* Register new drug batches
* Generate unique Batch IDs
* Store transactions on Ethereum

### Supply Chain Tracking

* Transfer ownership
* View complete transfer history
* Verify authenticity of drugs

### Anomaly Detection

* Isolation Forest model
* Synthetic pharmaceutical dataset
* AI-generated risk assessment

### Medical Records

* Secure upload
* IPFS storage
* ZKP generation and verification

### Cloud Performance

* Multi-VM deployment simulation
* Resource allocation
* Cloudlet scheduling
* Execution time analysis

## Performance Evaluation

The project evaluates the following aspects:

### Blockchain

* Drug registration transactions
* Transfer transactions
* Medical record commitments
* Gas usage analysis
* Transaction verification using Sepolia Etherscan

### Machine Learning

Model performance includes:

* Training Accuracy: 87%
* Testing Accuracy: 86.6%
* Precision: 47.1%
* Recall: 29.6%
* F1 Score: 36.4%
* Specificity: 95%
* ROC-AUC: 64.5%

The classification model is trained on a synthetically generated pharmaceutical dataset due to the limited availability of real-world datasets.

### AI Risk Assessment

Gemini API is used to:

* Analyze anomaly detection results
* Evaluate transfer history
* Generate detailed risk reports

### Zero-Knowledge Proofs

The implementation ensures:

* Privacy of patient records
* Local proof generation
* Proof verification using Circom and snark.js
* On-chain commitment verification

### Cloud Simulation

CloudSim Plus simulates three virtual machines handling different workloads:

* API Calls (Light)
* Blockchain Transactions (Medium)
* AI Anomaly Detection (Heavy)

The simulation measures:

* VM utilization
* Cloudlet execution time
* Resource allocation
* Processing delays
* Performance comparison between workloads

## Project Structure

```text
Mediledger-2.0/
│
├── blockchain/
├── smart-contracts/
├── ai-model/
├── zkp/
├── ipfs/
├── cloudsim/
├── frontend/
├── backend/
├── reports/
└── README.md
```

## How to Run

1. Clone the repository.

```bash
git clone https://github.com/prekscript/Mediledger
```

2. Install the required dependencies.

3. Configure the environment variables.

4. Deploy the smart contracts to the Sepolia Testnet.

5. Start the backend server.

6. Run the frontend application.

7. Execute the CloudSim Plus simulation for performance evaluation.

## Future Improvements

* Use real pharmaceutical datasets for anomaly detection.
* Improve machine learning accuracy using larger datasets.
* Deploy smart contracts on a production blockchain.
* Add role-based authentication.
* Support larger healthcare organizations.
* Optimize cloud resource allocation.
* Improve scalability for enterprise deployment.

## Screanshots

<img width="1364" height="680" alt="image" src="https://github.com/user-attachments/assets/7a815635-8f81-4b37-a12a-ee01d09b025e" />

<img width="1370" height="542" alt="image" src="https://github.com/user-attachments/assets/df010e75-8d46-4ca1-8311-5880f05c7bef" />
<img width="1378" height="558" alt="image" src="https://github.com/user-attachments/assets/c602f78d-5e27-4708-9d70-79389945c543" />
<img width="1396" height="398" alt="image" src="https://github.com/user-attachments/assets/58678eef-4ed5-49a2-b5be-c3579b74043b" />
<img width="1380" height="570" alt="image" src="https://github.com/user-attachments/assets/82137797-4875-44f9-94f5-03b5acb319d1" />
<img width="1358" height="560" alt="image" src="https://github.com/user-attachments/assets/5649d3c8-157a-4e34-a8c8-1bd1a2480560" />
<img width="1396" height="866" alt="image" src="https://github.com/user-attachments/assets/bbd1738f-97d4-4e5c-8f94-8362951db1e3" />

