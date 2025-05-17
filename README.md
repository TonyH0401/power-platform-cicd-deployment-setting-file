# Introduction

A collection of CI/CD export and import pipeline (which can be done manually) + deployment setting files.

- Natively, power platform also support pipeline but we will use Azure DevOps CI/CD pipeline.

Each project will be in its own corresponding folder which is named based on `Solution Name`. Each folder will have a `YAML` file for the CI/CD and a deployment setting file.

- The Azure DevOps pipeline we used is a GUI Power Platform Tool but from that tool we can also generate the `YAML` file.

Here are the tutorials for the Azure DevOps export and import pipeline I used:

- Tiyani 365: https://youtu.be/BVKMyTaHjjc?si=o0kujuKjwliOdN0M.
  - Each free Azure DevOps account will have 1 free Microsoft host for running pipeline and 1-ish self-host for running pipeline. I used the self-host version.
- Dhruvin Shah: https://youtu.be/YO5S7xuFDNU?si=0tGXe9v4focj2mSQ. This is a series of 4 videos.

  - https://powerplatformtrainings.com/2023/09/19/azure-devops-deployment-pipeline-code-reference-part-03/.

# Development Note
