# AWS Event-Driven Data Processing

This project is a boilerplate for building scalable, event-driven data processing pipelines using AWS services. Use this as a starting point for future projects with similar event-driven needs. The data is handled using an AWS Lambda, if you need a bigger scale - consider using AWS EMR or AWS Glue with proper orchestration services. 

---

## Features

- Template-ready design for reuse in similar solutions
- Event-driven architecture using AWS services
- Multi-environment support: `dev`, `stage`, and `prod`
- Integrated with key AWS components:
  - **Amazon SQS** – queue-based message handling
  - **Amazon SNS** – pub/sub event distribution
  - **Amazon S3** – object-based event triggering
  - **AWS Lambda** – compute-on-event functions
  - **IAM**, **CloudWatch**, and more

---

## Stack

| Layer             | Technology         |
|------------------|--------------------|
| Compute          | AWS Lambda         |
| Messaging        | Amazon SNS, SQS    |
| Storage          | Amazon S3          |
| Infrastructure   | Serverless Framework |
| Runtime          | Node.js + Python |

---

## Project Structure

```bash
aws-event-driven-data-processing/
├── config/             # Environment-specific configs
├── functions/          # Lambda handlers
├── node_modules/       # Node.js dependencies (ignored in Git)
├── sls/                # Serverless templates
├── venv/               # Python virtual environment (ignored in Git)
├── .gitignore
├── .gitattributes      # Git attributes (e.g., line endings, linguist overrides)
├── package.json        # Node.js dependencies
├── sample.json         # Sample event
├── serverless.yml      # Main Serverless deployment config
├── requirements.txt    # Python dependencies
└── README.md
