# GoCloudScale

## Overview

GoCloudScale is a scalable backend system built using Go programming language and hosts on Amazon Web Service (AWS). This project aims to provide a robust infrastructure for handling a growing user base, ensuring high performance and reliability.

## Features

- **Scalability:** Easily scale from zero to million users.
- **Go Backend:** Utilizes the Go programming language for a performant and efficient backend.
- **AWS Integration:** Leverages AWS services for hosting, database, and other cloud-based functionalities.
- **Terraform Deployment:** infrastructure as Code (IaC) using Terraform for easy and consistent deployment.

## Architecture

See `doc` folder to learn more about the architecture

## Technologies Used

- Go
- AWS
- Terraform

### Pre-requisites

- Go
- AWS CLI
- Terraform
- Docker

### Installation

1. Clone the repository
1. Install Go dependencies: `go mod tidy`
1. Setup AWS credentials: `aws configure`
1. Deploy infrastructure: `cd deploy/infrastructure && terraform init && terraform apply`

## Usage 

1. Build the project: `go build -o GoCloudScale cmd/GoCloudScale/main.go`
1. Run the project: `./GoCloudScale`

## Testing 

- Run unit tests: `go test ./...`

## Deployment

1. Update configurations in `pkg/config` folder 
1. Deploy infrastructure: `cd deploy/infrastructure && terraform apply`
1. Build and deploy the service: `go build -o GoCloudScale cmd/GoCloudScale/main.go && ./GoCloudScale`

## Contributing

We welcome contributions! Please see [CONTRIBUTING.md](CONTRIBUTING.md) for details.

## Acknowledgements

Mention any resources or inspiration you used in your project.

