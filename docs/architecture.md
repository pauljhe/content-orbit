# Architecture Overview

ContentOrbit follows an event-driven, serverless architecture.

- Data is periodically collected from external sources using AWS Lambda.
- Raw data is stored in Amazon S3 for durability and reprocessing.
- Transformed data is stored in Amazon RDS for structured querying.
- A React-based dashboard consumes processed data via API endpoints.
- Infrastructure is managed using Terraform.
