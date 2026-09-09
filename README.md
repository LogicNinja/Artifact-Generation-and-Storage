# Artifact Generation and Storage

## Problem Statement

Build an automated GitHub Actions workflow that packages an application project into a production-ready ZIP archive and stores the generated package as a downloadable artifact.

The workflow should execute in the cloud, generate the application distribution package, verify the generated ZIP file, and use the official `actions/upload-artifact` action to store the package at the end of the pipeline run.

The final artifact must be available for download from the **Artifacts** section of the GitHub Actions workflow run summary.

## Objective

The objective of this project is to demonstrate automated build artifact generation and storage using GitHub Actions.

The workflow:

1. Checks out the project source code.
2. Packages the application files into a ZIP archive.
3. Verifies the generated ZIP file.
4. Uploads the ZIP as a GitHub Actions artifact.
5. Makes the artifact available for download from the workflow run.

## Project Structure

```text
Artifact-Generation-and-Storage/
│
├── app/
│   ├── index.html
│   └── style.css
│
├── .github/
│   └── workflows/
│       └── build-artifact.yml
│
└── README.md
