<div align="center">

# PA4 Submission: TaskFlow Pipeline

<img alt="GitHub only" src="https://img.shields.io/badge/Submit-GitHub%20URL%20Only-10b981?style=for-the-badge">
<img alt="Total points" src="https://img.shields.io/badge/Total-100%20points-7c3aed?style=for-the-badge">

</div>

<div style="background:#f5f3ff;color:#111827;border-left:6px solid #6330bc;padding:14px 18px;border-radius:10px;margin:18px 0;">
Copy this file to <code style="color:#111827;background:#ddd6fe;padding:2px 4px;border-radius:4px;">SUBMISSION.md</code>. Put every screenshot in <code style="color:#111827;background:#ddd6fe;padding:2px 4px;border-radius:4px;">docs/</code>, embed it under the correct task, and write a short description below each image explaining what it proves. The grader should not need any file outside this repository.
</div>

## Student Information

| Field | Value |
|---|---|
| Name | TODO |
| Roll Number | TODO |
| GitHub Repository URL | TODO |
| Resource Group | `rg-sp26-TODO` |
| Assigned Region | TODO: `uaenorth` or `ukwest` |

## Evidence Rules

- Use relative image paths, for example: `![AKS nodes](docs/aks-nodes.png)`.
- Every image must have a 1-3 sentence description below it.
- Azure Portal screenshots must show the resource name and enough page context to identify the service.
- CLI screenshots must show the command and output.
- Mask secrets such as function keys, ACR passwords, and storage connection strings.


## Task 1: App Service Web App (15 points)

### Evidence 1.1: Forked Repository

TODO: Embed screenshot of your forked GitHub repository.
<img width="1600" height="767" alt="image" src="https://github.com/user-attachments/assets/962e6909-5a49-4545-8476-e907c0c97e31" />


Description: TODO: Explain that this is your working fork and that it contains the PA4 starter structure.

### Evidence 1.2: App Service Overview

TODO: Embed screenshot of the Web App overview page showing `webapp-<rollnum>` and Running status.
<img width="1603" height="823" alt="image" src="https://github.com/user-attachments/assets/a76eafd1-4072-4185-9f0b-b95af0e7ed8d" />


Description: TODO: State the resource group, region, runtime, and public URL.

### Evidence 1.3: Deployment Center / GitHub Actions

TODO: Embed screenshot of Deployment Center or the successful GitHub Actions deployment.
<img width="1427" height="553" alt="image" src="https://github.com/user-attachments/assets/21fa775d-a084-4afa-a7a1-20c818abf541" />

<img width="1614" height="903" alt="image" src="https://github.com/user-attachments/assets/177c3da8-f879-4cfd-b29a-4247286d2fd4" />


Description: TODO: Explain how the Web App is connected to your GitHub fork.

### Evidence 1.4: Live Web UI

TODO: Embed screenshot of the TaskFlow page loaded in a browser.
<img width="1599" height="802" alt="image" src="https://github.com/user-attachments/assets/36a78343-30aa-4a10-8cda-74401cd5f7d7" />
<img width="1392" height="789" alt="image" src="https://github.com/user-attachments/assets/21d94fcb-f481-40f1-9875-f81046cc406f" />


Description: TODO: Explain that the App Service is serving the frontend successfully.

---

## Task 2: Azure Container Registry (15 points)

### Evidence 2.1: ACR Overview

TODO: Embed screenshot of `crpa4<rollnum>` overview.
<img width="1417" height="774" alt="image" src="https://github.com/user-attachments/assets/9c31a653-87c2-4a1c-a63b-ed55e67fcc38" />

Description: TODO: Identify the registry SKU and resource group.

### Evidence 2.2: Docker Builds

TODO: Embed screenshot showing successful local builds for `validate-api`, `report-job`, and `func-app`.
<img width="1412" height="721" alt="image" src="https://github.com/user-attachments/assets/50006e56-53fd-40fd-a4dd-7887e7a0c6e9" />
<img width="700" height="600" alt="image" src="https://github.com/user-attachments/assets/902eb4b6-c4df-4f0d-a78d-29c553434353" />
<img width="697" height="510" alt="image" src="https://github.com/user-attachments/assets/1097a868-ea8b-4ce3-a322-57aed0a35c7e" />
<img width="794" height="593" alt="image" src="https://github.com/user-attachments/assets/d16aa22b-07b8-4b5a-83f6-e3f74033d7e1" />
<img width="795" height="475" alt="image" src="https://github.com/user-attachments/assets/f8f90816-c0f0-41bf-9ea3-c849832ff41e" />


Description: TODO: Explain which folder produced each image.

### Evidence 2.3: ACR Repositories

TODO: Embed screenshot or CLI output showing all three repositories in ACR.
<img width="1390" height="567" alt="image" src="https://github.com/user-attachments/assets/25e1a6af-33a0-476d-8ec6-cf1db76b8648" />
<img width="976" height="674" alt="image" src="https://github.com/user-attachments/assets/bf3fe5a1-232c-4a8f-9b92-88528a5f0198" />


Description: TODO: Confirm `validate-api:v1`, `report-job:v1`, and `func-app:v1` were pushed.

---

## Task 3: Durable Function Implementation (12 points)

### Evidence 3.1: Completed Function Code

TODO: Link to your completed file: `[function_app.py](function-app/function_app.py)`.
https://github.com/idahludba2/CS487-PA4/blob/main/function-app/function_app.py


Description: TODO: Summarize how your orchestrator chains validation and report generation.

### Evidence 3.2: Local Function Handler Listing

TODO: Embed screenshot of `func start` showing the HTTP starter, orchestrator, and activities.
<img width="1726" height="577" alt="image" src="https://github.com/user-attachments/assets/145f5dea-dd90-480b-b795-c0e0d789eaee" />
<img width="1051" height="869" alt="image" src="https://github.com/user-attachments/assets/5457fa86-213d-4bad-832b-58119abed220" />


Description: TODO: Explain that the Durable Functions runtime discovered your handlers.

---

## Task 4: Function App Container Deployment (8 points)

### Evidence 4.1: Function App Container Configuration

TODO: Embed screenshot showing the Function App uses your `func-app:v1` image from ACR.
<img width="1590" height="761" alt="image" src="https://github.com/user-attachments/assets/17c95e2b-f35c-426a-9f39-b59d7feddf68" />
<img width="1617" height="904" alt="image" src="https://github.com/user-attachments/assets/711782eb-bd12-4998-a8b7-bb319707e10a" />
<img width="1583" height="856" alt="image" src="https://github.com/user-attachments/assets/7dca0b96-c3eb-416b-a1c2-583a22b4d00b" />


Description: TODO: State the Function App name and image URI.

### Evidence 4.2: Orchestration Smoke Test

TODO: Embed screenshot of the `curl` output that starts an orchestration and returns status URLs.
<img width="1602" height="402" alt="image" src="https://github.com/user-attachments/assets/383258bb-d46d-4412-83dc-c59f9a6a6a64" />


Description: TODO: Explain what the returned `id` and `statusQueryGetUri` prove.

### Evidence 4.3: Expected Failed Status Before Downstream Wiring

TODO: Embed screenshot of the status query JSON showing the expected failure before `VALIDATE_URL` is configured.

<img width="1579" height="291" alt="image" src="https://github.com/user-attachments/assets/fc1bca92-408b-4c79-afa8-3c2f0cb31512" />
<img width="1558" height="651" alt="image" src="https://github.com/user-attachments/assets/7037bb91-ddb9-4148-bc58-4e828505e666" />

Description: TODO: Explain why this failure is expected at this stage.

---

## Task 5: AKS Validator (15 points)

### Evidence 5.1: AKS Cluster

TODO: Embed screenshot of AKS overview showing `aks-<rollnum>` succeeded.


Description: TODO: State node count, node size, region, and resource group.

### Evidence 5.2: Kubernetes Nodes and Pods

TODO: Embed screenshot of `kubectl get nodes` and `kubectl get pods`.

Description: TODO: Explain that the validator pod is scheduled and running.

### Evidence 5.3: Kubernetes Service

TODO: Embed screenshot of `kubectl get service validate-service`.

Description: TODO: Identify the external IP and port exposed by the LoadBalancer.
<img width="1448" height="975" alt="image" src="https://github.com/user-attachments/assets/39f5b898-d240-4f88-b37b-daed6d653bd4" />

### Evidence 5.4: Validator API Tests

TODO: Embed screenshot of `curl /health`, a valid `curl /validate`, and an invalid `curl /validate`.
<img width="1434" height="742" alt="image" src="https://github.com/user-attachments/assets/2e2ab3f6-e203-4135-92f7-4a19f9d332da" />

Description: TODO: Explain the accepted path and the `qty > 100` rejection rule.

### Evidence 5.5: Function App `VALIDATE_URL`

TODO: Embed screenshot showing the Function App application setting `VALIDATE_URL`.
<img width="1370" height="826" alt="image" src="https://github.com/user-attachments/assets/e235c059-8c18-414f-b841-7821244e6030" />

Description: TODO: Explain how the Durable Function reaches the AKS validator.

### Evidence 5.6: AKS Idle Behavior

TODO: Embed AKS metrics screenshot and/or `kubectl` output after the service is idle.

Description: TODO: Explain that the AKS node remains running even when there are no orders.

---

## Task 6: ACI Report Job (15 points)

### Evidence 6.1: Blob Container

TODO: Embed screenshot of the `reports` blob container.
<img width="1481" height="286" alt="image" src="https://github.com/user-attachments/assets/008db1eb-4314-46a6-a1c8-df5072a591f6" />

<img width="1435" height="781" alt="image" src="https://github.com/user-attachments/assets/420e5543-2a4c-48d2-b702-e2f960a31691" />

Description: TODO: Explain where generated PDFs are stored.

### Evidence 6.2: Manual ACI Run
<img width="1427" height="895" alt="image" src="https://github.com/user-attachments/assets/78522c7b-cdf0-44f7-ac29-76f9698e8ec9" />

TODO: Embed screenshot of `az container show` for `ci-report-test`.

Description: TODO: State the final container state and why the job exits.

### Evidence 6.3: ACI Logs

TODO: Embed screenshot of `az container logs`.

Description: TODO: Explain what the report job printed after generating and uploading the PDF.

### Evidence 6.4: Generated PDF

TODO: Embed screenshot showing `TEST-001.pdf` in Blob Storage or opened from Blob Storage.

Description: TODO: Explain how this proves the ACI wrote to storage.

### Evidence 6.5: Function App Managed Identity and IAM

TODO: Embed screenshots of system-assigned identity enabled and Contributor role assignment on your resource group.
<img width="1444" height="574" alt="image" src="https://github.com/user-attachments/assets/be219f5b-3358-4ef5-9ae2-e41e4aa9a17e" />

Description: TODO: Explain why the Function App needs this permission to create ACIs.

### Evidence 6.6: Report App Settings

TODO: Embed screenshot of `REPORT_*`, `ACR_*`, `STORAGE_CONN`, and `SUBSCRIPTION_ID` settings.
<img width="1433" height="709" alt="image" src="https://github.com/user-attachments/assets/b8f1f2ab-44a3-4b96-8717-c4b4b88dfb50" />
<img width="1152" height="409" alt="image" src="https://github.com/user-attachments/assets/433262c0-249e-472a-a121-e2b258af5cc0" />

Description: TODO: Explain what each group of settings is used for. Mask secrets.

---

## Task 7: End-to-End Pipeline (15 points)

### Evidence 7.1: Web App Wiring

TODO: Embed screenshot showing `FUNCTION_START_URL` and `FUNCTION_STATUS_URL` configured on the Web App.

Description: TODO: Explain how the frontend starts and polls the Durable orchestration.
<img width="1425" height="767" alt="image" src="https://github.com/user-attachments/assets/a5b5a42c-ff11-4b94-975a-6b629b9bfc15" />

### Evidence 7.2: Happy Path UI

TODO: Embed screenshots of the form before submit, Running status, and Completed status with report URL.
<img width="1414" height="880" alt="image" src="https://github.com/user-attachments/assets/53267f10-9ad5-4d3d-87fd-4be424988c19" />
<img width="1080" height="588" alt="image" src="https://github.com/user-attachments/assets/9ab3821d-9a34-4a80-b270-fd6d1a93d55f" />
<img width="1234" height="569" alt="image" src="https://github.com/user-attachments/assets/8ee9c490-6fe3-4c2d-8758-c3538c885173" />

Description: TODO: Explain the valid order payload and final result.

### Evidence 7.3: Backend Participation

TODO: Embed screenshots showing Function App invocation, AKS validator evidence, ACI evidence, and Blob PDF evidence.

Description: TODO: Trace the same order ID across services.

### Evidence 7.4: Reject Path UI

TODO: Embed screenshot of an order with `qty > 100` being rejected.

Description: TODO: Explain why no report ACI should be created for this order.

---

## Task 8: Write-up and Architecture Diagram (5 points)

### Evidence 8.1: Architecture Diagram

TODO: Embed your architecture diagram from `docs/`.
<img width="1489" height="900" alt="image" src="https://github.com/user-attachments/assets/609102f4-a461-432b-b43a-65f59d8209e3" />

Description: TODO: Confirm that it shows GitHub, App Service, Durable Function, AKS, ACI, Blob Storage, ACR, and IAM.

### Question 8.2: Service Selection

TODO: In 3-4 sentences each, explain why TaskFlow uses App Service, Durable Functions, AKS, and ACI for their specific roles.
App Service: Chosen for the frontend dashboard because it provides a fully managed platform for hosting web applications. It simplifies the deployment process through GitHub integration and handles infrastructure tasks like SSL termination and scaling automatically, allowing the developer to focus on the Node.js application logic.

Durable Functions: Used as the middleware orchestrator to manage the stateful, sequential workflow of order processing. It ensures that the transition between the validation and report-generation phases is reliable, handling potential delays or retries without the overhead of maintaining an active server thread.

Azure Kubernetes Service (AKS): Employed for the validator microservice to provide a high-availability environment for long-running processes. AKS offers robust container orchestration, internal load balancing, and the ability to scale pods independently, which is ideal for a service that must always be ready to receive validation requests.

Azure Container Instances (ACI): Utilized for the report-job because the task is ephemeral and short-lived. ACI allows for "serverless container" execution, where billing is calculated per second of usage, making it significantly more cost-effective than keeping a dedicated VM running for a task that only takes 10–15 seconds to complete.
### Question 8.3: ACI vs AKS

TODO: Compare idle behavior, cost behavior, and operational model for AKS and ACI using your screenshots.
The primary difference between AKS and ACI in the TaskFlow architecture lies in their persistence and billing models. **AKS** operates as a managed cluster where nodes remain in a "Ready" state 24/7 to ensure the validator microservice can provide immediate responses to incoming HTTP traffic. This results in a static cost model where the user is billed hourly for the underlying VM resources (Standard_B2s), regardless of whether the service is idle or active. In contrast, **ACI** is an ephemeral, serverless container service used for one-shot report generation. It has no idle state; the container is provisioned on-demand by the orchestrator, performs its task, and is immediately terminated. Consequently, the cost behavior for ACI is strictly consumption-based, with billing calculated per second of execution, resulting in zero cost when the system is idle.

Operationally, the two services serve distinct roles within the pipeline. **AKS** requires a more complex management model involving Kubernetes manifests, pod health monitoring, and internal load balancing to maintain high availability for the validation logic. This makes it suitable for "always-on" microservices that require low-latency communication within the virtual network. **ACI** provides a much simpler operational model for the report-job, as it removes the need for cluster management entirely. The Durable Function simply requests a container instance to run a specific image with environment variables, making it the ideal choice for heavy, short-lived workloads like PDF generation that would otherwise waste resources if hosted on a persistent server.
### Question 8.4: Durable Functions vs Plain HTTP

TODO: Explain at least two problems that Durable Functions solves for this sequential workflow.
Handling Timeouts: In a plain HTTP chain, if the report generation takes longer than the client-side timeout (e.g., 230 seconds in Azure), the connection drops and the process fails. Durable Functions solve this by using an asynchronous polling pattern, where the client receives a 202 Accepted and checks a status URL until the job is done.

Reliable State Persistence: If a server restarts during a plain HTTP workflow, all progress is lost. Durable Functions use Event Sourcing to record every step in Table Storage. If the app crashes, the orchestrator "replays" its history and resumes exactly where it left off, ensuring that an order is never validated without a report being generated.
### Question 8.5: Cost Review

TODO: Embed Cost Management screenshot scoped to your resource group.

Description: TODO: Identify the most expensive resource and explain why.
Most Expensive Resource: App Service plan (pa4-27100307)

Description: Based on the CostByResource breakdown, the App Service plan is the single most expensive component, accounting for $2.95 of the total spend. This is because the plan (likely on the B1 tier) provides a dedicated virtual machine instance that stays powered on 24/7 to host the frontend web application. Unlike serverless components, you are billed for the reserved capacity of this plan regardless of how much traffic the dashboard receives.

Comparative Analysis:
The effectiveness of the ephemeral model is proven by the Container Instances (ci-report-ord-001 and ci-report-test), which both show a cost of <$0.01. Because these containers were only provisioned for the duration of the PDF generation and then immediately deleted, they incurred virtually no cost compared to the persistent App Service plan. While the Kubernetes service appears low at $0.06 in this view, it is worth noting that the actual compute nodes for the cluster are typically billed in a separate "Node Resource Group" (the MC_ group), which handles the heavier VM costs.
### Question 8.6: Challenges Faced

TODO: Describe at least two real issues you hit and how you debugged them.
Non-Deterministic Workflow Detection: During Task 4, the orchestrator failed with an error stating a change was made to the code after an instance started. I debugged this by checking the output field in the instance status JSON and learned that Durable Functions require deterministic code. I resolved it by ensuring no random numbers or direct date-time calls were inside the orchestrator and by clearing old Task Hub instances.

PublicAccessNotPermitted (Task 7): After the first successful E2E run, the PDF link in the dashboard returned an XML error instead of the file. I debugged this by reviewing the Storage Account settings and realized that public blob access was disabled by default. I resolved it by enabling "Allow Blob public access" in the configuration and changing the reports container access level to "Blob".
---
