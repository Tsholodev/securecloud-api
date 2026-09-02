# SecureCloud API

SecureCloud API is a security-focused REST API project designed to demonstrate the practical integration of cybersecurity principles, software engineering, and cloud computing.

The project simulates a small payment platform where users can authenticate, access protected resources, and perform payment-related operations.

The primary goal is to demonstrate how security can be integrated throughout the software development and cloud deployment lifecycle rather than treated as an afterthought.

## Project Goals

* Build a functional REST API
* Implement secure authentication and authorization
* Protect sensitive application data
* Apply secure database practices
* Containerize the application with Docker
* Automate testing and builds using CI/CD
* Perform automated security checks
* Deploy the application to a cloud environment
* Document security risks, mitigations, and architectural decisions

## Planned Security Controls

The project will progressively implement:

* Password hashing
* Authentication
* Role-based authorization
* Input validation
* Parameterized database queries
* Secure secret management
* Security-focused logging
* API rate limiting
* Dependency vulnerability scanning
* Automated security testing

## Planned Technology Stack

| Technology     | Purpose                         |
| -------------- | ------------------------------- |
| Java           | Application development         |
| Maven          | Build and dependency management |
| PostgreSQL     | Relational database             |
| Docker         | Application containerization    |
| GitHub Actions | CI/CD automation                |
| Terraform      | Infrastructure as Code          |
| AWS            | Cloud deployment                |
| OWASP tooling  | Security testing                |

## Architecture

The planned architecture is:

```text
                Internet
                   |
                   v
            +-------------+
            |   REST API   |
            +------+------+
                   |
          +--------+--------+
          |                 |
          v                 v
   Authentication       Application
      & Security          Services
                            |
                            v
                     +-------------+
                     | PostgreSQL  |
                     +-------------+

          CI/CD Pipeline
                |
                v
       GitHub Actions
                |
        +-------+-------+
        |               |
       Test         Security Scan
        |               |
        +-------+-------+
                |
                v
             Docker
                |
                v
              Cloud
```

## Project Structure

```text
securecloud-api/
├── src/
│   ├── main/
│   │   └── java/
│   └── test/
├── docs/
├── security/
├── .github/
│   └── workflows/
├── .env.example
├── .gitignore
├── pom.xml
└── README.md
```

## Security Documentation

Security documentation will be maintained in the `security/` directory.

Planned documentation includes:

* Threat model
* Security controls
* Vulnerability assessment
* Security testing results
* Risk assessment

## Development Roadmap

### Phase 1 — Foundation

* [x] Create repository
* [x] Establish project structure
* [ ] Create Maven project
* [ ] Implement basic API

### Phase 2 — Security

* [ ] Implement authentication
* [ ] Implement authorization
* [ ] Add password hashing
* [ ] Add input validation
* [ ] Secure database queries
* [ ] Add security logging

### Phase 3 — Cloud & DevOps

* [ ] Create Docker configuration
* [ ] Add GitHub Actions pipeline
* [ ] Add automated security scanning
* [ ] Create infrastructure using Terraform
* [ ] Deploy application to the cloud

### Phase 4 — Testing & Documentation

* [ ] Unit tests
* [ ] Integration tests
* [ ] Security testing
* [ ] Threat model
* [ ] Architecture documentation
* [ ] Final technical demonstration

## Status

🚧 **In development**

This repository is being developed as a practical cybersecurity and cloud computing project.

## Author

Tsholofelo Moralo
