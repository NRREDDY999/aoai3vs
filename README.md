# Azure OpenAI Embeddings QnA

A simple web application for a OpenAI-enabled document search. This repo uses Azure OpenAI Service for creating embeddings vectors from documents. For answering the question of a user, it retrieves the most relevant document and then uses GPT-3 to extract the matching answer for the question.


## Deploy on Azure (WebApp + Batch Processing) with Azure Cognitive Search
[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FNRREDDY999%2Faoai3vs%2Fmain%2Finfrastructure%2Fdeployment_ACS.json)

Click on the Deploy to Azure button and configure your settings in the Azure Portal as described in the [Environment variables](#environment-variables) section.



Please be aware that you need:
-   an existing Azure OpenAI resource with models deployments (instruction models e.g. text-davinci-003, and embeddings models e.g. text-embedding-ada-002)

### Signing up for Vector Search Private Preview in Azure Cognitive Search
Azure Cognitive Search supports searching using pure vectors, pure text, or in hybrid mode where both are combined. For the vector-based cases, you'll need to sign up for Vector Search Private Preview. To sign up, please fill in this form: [https://aka.ms/VectorSearchSignUp](https://aka.ms/VectorSearchSignUp).

Preview functionality is provided under [Supplemental Terms of Use](https://azure.microsoft.com/en-us/support/legal/preview-supplemental-terms/), without a service level agreement, and isn't recommended for production workloads.

