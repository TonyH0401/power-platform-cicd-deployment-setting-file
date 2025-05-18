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

_Ordered from newest to oldest_

## 2025-05-16

My original implementation of the Azure pipeline with a solution was normal because the solution was simple, so there wasn't any problem arised. However, there are solutions which are complex because there are a lot of customizations. For those solutions, before running the pipeline, you need to import the PCF, the plugins with the plugin steps (no need to configure anything) and the connection references (or connection).

A little note with the PCF, changing the PCF will not be reflected in the managed solution (it will be reflected in the unmanaged solution), you need to change the version in the manifest file in order for the PCF to be reflected in the managed solution.
