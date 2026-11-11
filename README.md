<h1 align="center">Noah Kivett</h1>
<h2 align="center">Software Engineer | Java · Spring Boot · AWS · Kubernetes | OAuth2/OIDC Identity Platforms</h2>

<p align="center">
  <a href="https://nkivett.com/">
    <img src="https://img.shields.io/badge/Portfolio-9cf?style=for-the-badge" />
  </a>
  <a href="https://linkedin.com/in/nkiv" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-blue?style=for-the-badge" alt="LinkedIn"/>
  </a>
  <a href="https://github.com/nkiv/nkiv/blob/main/resume/Noah-Kivett.pdf">
    <img src="https://img.shields.io/badge/Resume-A47764?style=for-the-badge" />
  </a>
</p>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=nkiv&style=flat-round" />
</p>

---

## About Me

I'm a backend engineer on the identity platform at Charter Communications. It's a large OAuth2/OIDC system that handles login and token refresh for consumer and enterprise products, with more than a hundred components shipped together on a shared release.

I dig into pre-production issues with tracing and logging tools, design and build new service features, and ship them through CI/CD to Kubernetes. I own platform releases and the regression suite that decides when code is ready to merge.

I understand a system before I change it, I use AI to ask my dumbest questions, and I learn through failing. When something goes wrong I think of every way I could fix it and plan out the fix before I change anything. I'm careful with every action I take so as few failures as possible are created.

AI is a big part of how I work faster. I turned the tasks I repeat most into agent skills and tools.

Outside of work, I self-host projects on a Raspberry Pi and make small games in Godot and Pico-8 game engines. I  build software tools I find useful for cost saving and automation in my personal life. 

---

## Enterprise Experience

### Charter Communications (Spectrum)
**Software Developer I** · OAuth Platform Team · *Nov 2025 to Present*

Enterprise AuthN/AuthZ. More than a hundred components handling login, token refresh and device authentication for consumer and enterprise products, built with Java and Spring on AWS and Kubernetes.

![Release Management](https://img.shields.io/badge/Release_Management-0D47A1?style=for-the-badge&logo=gitlab&logoColor=white)
- I own platform releases. I sequence rollouts across environments, make sure database migrations go out first, write the change records and release notes, keep the release calendar up to date, and run pre-prod deployments. With up to 4 releases happening concurrently.

![Test Automation](https://img.shields.io/badge/Test_Automation_&_Quality-2E7D32?style=for-the-badge&logo=testinglibrary&logoColor=white)
- Resolved 500+ regression failures by tracing each one to its root cause: code defects, test defects, bad test data, or upstream dependencies
- Triaged before/after test summaries to find failure clusters and resolve the new errors before leaving pre-production.
- Built a Python triage toolchain that fingerprints test runs, figures out which environment they came from, and builds failure trend dashboards

![Architecture](https://img.shields.io/badge/Architecture-0D47A1?style=for-the-badge&logo=blueprint&logoColor=white)
- Designed and built a response simulation plugin for the performance team. It returns delays, status codes and bodies by percentage, so they can test how services behave when upstreams are slow or failing
- Wrote up two ways to build that plugin, got the leads to sign off on one, then built it
- Reviewed and fixed AI-generated documentation across 37 service repos for security and accuracy: repaired broken diagrams and changelogs and took out internal-only details

![Development](https://img.shields.io/badge/Development-2E7D32?style=for-the-badge&logo=spring&logoColor=white)
- Built WireMock integration test suites for OAuth flows, running against a local Cassandra, Redis and WireMock setup
- Moved legacy tests over to modern Spring Boot pattern. Reducing code bloat by thousands of lines. 
- Fixed a circuit breaker that could never open because a new one was created on every request.
- Modernized 9 services: Java 11 to 21, Spring Boot 2.7 to 3.x, and Spring Data for Cassandra and reactive Redis

![Debugging](https://img.shields.io/badge/Debugging-E65100?style=for-the-badge&logo=bugsnag&logoColor=white)
- Tracked down recurring production errors using distributed tracing
- Root-caused a multi-service login slowdown that ran through the application, the JVM, Kubernetes and the service mesh
- Found a Spring dependency injection bug in a shared logging library that left a logging field blank across a service, and fixed it

![AI Tooling](https://img.shields.io/badge/AI_Tooling-6A1B9A?style=for-the-badge&logo=openai&logoColor=white)
- **Test triage:** a finished regression run gets a test summary verdict in less than a minute
- **Environment health:** a full pod check in about 3 seconds, shows us the environment health. Saving us a 30-minute testing run.
- **Daily records:** an agent rebuilds my work log from session history. It recovered 7 working days I hadn't written up and saving 10 minutes each day. 
- **Learning the system:** I curated knowledge bases and built a tutor agent with a course, so I get answers about a complex platform without digging through dozens of repos. Creating documentation, diagrams, and answering questions in seconds. 
- I connected my agents to the team's ticketing, docs, code and logging tools (MCP) so one request pulls everything I need, and each agent gets only the access it needs for assisting in everyday tasks with the right context. 

---

## Technical Skills

### Languages
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=black)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C++-0206E0?style=flat-square&logo=cplusplus&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnu-bash&logoColor=white)
![Lua](https://img.shields.io/badge/Lua-2C2D72?style=flat-square&logo=lua)
![SQL/CQL](https://img.shields.io/badge/SQL/CQL-4479A1?style=flat-square)

### Frameworks & Libraries
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=spring&logoColor=white)
![Spring Data](https://img.shields.io/badge/Spring_Data-6DB33F?style=flat-square&logo=spring&logoColor=white)
![Spring Reactive](https://img.shields.io/badge/Reactive_Redis-6DB33F?style=flat-square&logo=spring&logoColor=white)
![Resilience4j](https://img.shields.io/badge/Resilience4j-1F6FEB?style=flat-square)
![TestNG](https://img.shields.io/badge/TestNG-D35400?style=flat-square)
![JUnit 5](https://img.shields.io/badge/JUnit_5-25A162?style=flat-square&logo=junit5&logoColor=white)
![WireMock](https://img.shields.io/badge/WireMock-6DB33F?style=flat-square)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)

### Infrastructure & Data
![AWS](https://img.shields.io/badge/AWS_(IAM,_STS,_Kinesis)-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Helm](https://img.shields.io/badge/Helm-0F1689?style=flat-square&logo=helm&logoColor=white)
![Istio](https://img.shields.io/badge/Istio/Envoy-466BB0?style=flat-square&logo=istio&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Cassandra](https://img.shields.io/badge/Cassandra-1287B1?style=flat-square&logo=apache-cassandra&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Kafka](https://img.shields.io/badge/Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white)

### Observability & DevOps
![Datadog](https://img.shields.io/badge/Datadog-632CA6?style=flat-square&logo=datadog&logoColor=white)
![Splunk](https://img.shields.io/badge/Splunk-000000?style=flat-square&logo=splunk&logoColor=white)
![GitLab CI](https://img.shields.io/badge/GitLab_CI-FC6D26?style=flat-square&logo=gitlab&logoColor=white)

### Protocols & Security
![OAuth 2.0](https://img.shields.io/badge/OAuth_2.0-3C873A?style=flat-square)
![OIDC](https://img.shields.io/badge/OpenID_Connect-F78C40?style=flat-square&logo=openid&logoColor=white)
![JWT](https://img.shields.io/badge/JWT/JWE/JWS-000000?style=flat-square&logo=jsonwebtokens&logoColor=white)
![SAML](https://img.shields.io/badge/SAML_2.0-2B2D42?style=flat-square)
![mTLS](https://img.shields.io/badge/mTLS-2B2D42?style=flat-square)
![REST](https://img.shields.io/badge/REST-009688?style=flat-square)

### AI & Automation
![MCP](https://img.shields.io/badge/MCP-000000?style=flat-square)
![Agent Skills](https://img.shields.io/badge/Agent_Skills-6A1B9A?style=flat-square)

---

## Personal Projects

### Pi-Portfolio
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Raspberry Pi](https://img.shields.io/badge/Raspberry%20Pi-C51A4A?style=flat-square&logo=raspberry-pi)

[Repo](https://github.com/nkiv/pi-portfolio) · [Live](https://nkivett.com/)

My portfolio site, self-hosted on a Raspberry Pi. I moved it from PHP to React and got load times under a second. I handle the DNS, Apache config, SSL certs and uptime monitoring myself, on bare metal.

### Game Prototypes
![Lua](https://img.shields.io/badge/Lua-2C2D72?style=flat-square&logo=lua)
![Pico-8](https://img.shields.io/badge/Pico--8-FF004D?style=flat-square)

[Repo](https://github.com/nkiv/pico-8-projects) · [Play on itch.io](https://nkiv.itch.io/)

Small game demos created under time constraints for game jams held on itch.io. Created using javascript and lua using phaser or pico-8 game engines. 
---
