# Instruction for deployment on Codesphere

1. Create a new workspace: 
- Use the HTTP url of this repo to create a New Workspace in Codesphere

2. Go to "CI & Deploy": 
- Run the Prepare Stage (this might take a couple minutes)
- When the Prepare Stage is ready, start the Run Stage

3. Use 'Open Deployment' in the top right corner to open N8N.

## Bonus: Ollama Model hosted on Codesphere

Together with N8N, this template deploys an Ollama `qwen` model hosted on Codesphere. 
To use it in N8N, add an `Ollama` node (from the AI category) and configure it: 

```
# Replace WORKSPACE_ID with your current Workspace ID!
Base URL: http://ws-server-WORKSPACE_ID-ollama-service.workspaces.svc.cluster.local:3000
API Key: <none>
```
