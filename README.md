# serverless-mock-automation

The following automation is intended to generate usage statistics for Insights.  It is a cross-platform automation which can be run as a linux container.  I use Docker Desktop so that I can run multiple automations concurrently on my local machine.

To run multiple cross-platform automations concurrently locally you will need to create a machine template for each container, https://docs.uipath.com/orchestrator/v0/docs/automation-cloud-robots-serverless

How to start a named container:

---
docker run --name <INSERT CONTIANER NAME> -e LICENSE_AGREEMENT=accept -e ORCHESTRATOR_URL="<INSERT ORCHESTRATOR URL>" -e MACHINE_KEY="<INSERT MACHINE KEY>" -tid registry.uipath.com/robot/runtime
---

