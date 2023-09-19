### Description

Automate the process of tagging BPMN models via the Camunda Web Modeler API using this GitHub Action. This action is part of a suite of actions designed to streamline the CI/CD pipeline for managing BPMN process models.

### Usage

To use this action in your workflow, follow these steps:

**Set Up Camunda API Access:**

   Ensure you have correct credentials to authorize the [Camunda Modeler API](https://docs.camunda.io/docs/next/apis-tools/web-modeler-api/)

You can simply refer to this GitHub action in any GitHub workflow.:

   ```yaml
         - name: Tag BPMN Models
           uses: apendo-c8/download-bpmn-models-action@v1
           with:
             source: 'Project Id'
             tag: 'Name of milestone to use'
             client_id: 'Camunda Modeler API Client ID'   
             client_secret: 'Camunda Modeler API Client Secret'
