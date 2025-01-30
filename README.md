# Unofficial Google Gemini AI Integration for Chronicle SOAR/Security Operations


## Overview

**NOTE: Google has released official support for [Vertex AI in SecOps](https://cloud.google.com/chronicle/docs/soar/marketplace-integrations/vertex-ai). It is recommended to run the official integration.**


With the [release of Gemini on Google Cloud Vertex AI](https://cloud.google.com/vertex-ai/docs/generative-ai/model-reference/gemini), organizations can now leverage Gemini for integration into exisiting or new applications. With Chronicle SOAR/Security Operations, organizations can integrate 3rd-party APIs for use within automation & response workflows. This integration provides the ability to submit a prompt to Gemini and receive output.

## Pre-requisities
- Google Cloud Project - A project, with Vertex AI enabled, must be created.
- Service Account JSON Key - To interact with Gemini, a service account credential must be created with `aiplatform.endpoints.predict` permission.

## Installation
1. Navigate to Releases in this repo and download the .zip package.
2. In Chronicle SOAR/Security Operations, install the integration by opening the IDE and importing the package.
3. Set up an integration via Integrations, providing the project name, service account JSON, and the [region](https://cloud.google.com/vertex-ai/generative-ai/docs/learn/locations#available-regions) you wish to use.

## Example
In this example, we extract the detection name from an alert from Google Security Command Center Premium. We provide it to Gemini and ask for a remediation recommendation.

![Gemini](Gemini%20AI%20SOAR%20Action.png?raw=true)
