# Vercel monorepo example

This repository demonstrates how Vercel creates deployments for monorepos and how to configure DeployFreeze for this setup.

This is an example repository created using `npx create-turbo`.

## Quick configuration (Repo Admin privileges required)
1.  Go to your repository Settings -> Environments. <img width="1920" height="1080" alt="repo-settings" src="https://github.com/user-attachments/assets/1722206b-28b9-436f-be73-f3168405c091" />   
2. For each environment, enable DeployFreeze under "Deployment protection rules."
<img width="1920" height="1080" alt="save-configuration" src="https://github.com/user-attachments/assets/3c5f8714-09c7-42e8-9068-15ec8b8bfe23" />

If you do not see DeployFreeze as an option, make sure it is installed on your repository.

## In depth: Github Environments with Vercel 
If your repository contains multiple Vercel projects, then Vercel will create project-scoped environments and deployments in your repository. For example, in this repository, there are two NextJS apps, `docs` and `web`, and two corresponding Vercel projects, `vercel-monorepo-example-docs` and `vercel-monorepo-example-web` respectively. 

One can see this under `Deployments` on the main page that we have active deployments for two different 'Production' environments: one corresponding to each of the two NextJS apps & Vercel projects.
<img width="1920" height="1080" alt="deployments-highlight" src="https://github.com/user-attachments/assets/f6bdb510-261d-4b0a-9a77-016bfcf0c5c8" />
Following that `Deployments` link to the [/deployments](https://github.com/deploy-freeze/vercel-monorepo-example/deployments) page, we our full history of deployments. On the left, we have the ability to filter by environments and view deployments for just that environment: these align one-to-one with deployments on the Vercel project.
<img width="1920" height="1080" alt="deployments-page-environments-highlight" src="https://github.com/user-attachments/assets/8ae2a9ba-4e45-4f41-b72e-4a2b51244b28" />
