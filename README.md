# MyDotNetApp

A basic .NET Core Web API application deployed to Azure using GitHub Actions.

## Prerequisites

- .NET 6.0 SDK
- Azure Subscription
- GitHub Account

## Setup Instructions

1. Create an Azure Web App
2. Get your Azure Web App publish profile and add it as a secret in your GitHub repository:
   - Go to your Azure Portal
   - Navigate to your Web App
   - Download publish profile
   - In your GitHub repository, go to Settings -> Secrets -> Actions
   - Add a new secret named `AZURE_WEBAPP_PUBLISH_PROFILE` with the publish profile content
3. Update the workflow file:
   - Open [.github/workflows/azure-deploy.yml](cci:7://file:///c:/Users/HAroon%20trader/Desktop/exam%20prep/MyDotNetApp/.github/workflows/azure-deploy.yml:0:0-0:0)
   - Replace `your-app-name` with your actual Azure Web App name

## Running Locally

```bash
dotnet run
```

The application will be available at `https://localhost:5001`
