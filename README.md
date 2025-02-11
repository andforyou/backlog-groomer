# backlog-groomer

## Overview
Backlog Groomer is an intelligent agent designed to maintain a clean Jira environment through automated duplicate issue detection and management. The agent streamlines issue management by proactively identifying similar issues, facilitating consolidation, and improving overall project organization.

## Core Capabilities
- **Real-time Duplicate Detection**: Automatically scans and identifies potential duplicate issues as they are created
- **Smart Issue Comparison**: Utilizes advanced comparison algorithms to analyze issue descriptions and identify similarities
- **Interactive Consolidation**: Guides users through the process of selecting and managing duplicate issues
- **Automated Cleanup**: Streamlines the process of merging or removing confirmed duplicate issues

## Development Journey

### Phase 1: Basic Duplicate Detection

![detect duplicate](https://github.com/user-attachments/assets/e1f687de-78f0-4ee6-8f1f-928ff80dafd1)

In the first phase, we implemented basic duplicate detection capabilities:
- Configured core knowledge base for issue comparison
- Established initial action set for duplicate detection
- Created test dataset for validation

![test data](https://github.com/user-attachments/assets/cecd7b47-bb8d-4bac-8b76-f2f1a10c384c)

### Phase 2: Enhanced Functionality

[Screenshot placeholder: Updated agent configuration with expanded capabilities]

We expanded the agent's capabilities to include:

- Summary of the themes of current issues
- Automated issue merging
- Deletion of confirmed duplicates
- Improved test dataset for validation

![new data](https://github.com/user-attachments/assets/6dc9533e-5ef4-4757-a0b8-a61467db85f5)

## Agent Architecture

![agent](https://github.com/user-attachments/assets/abecc35b-8afb-40f5-a69d-8466090cbf8c)

## Testing and Validation

Our testing process involved:
- Making a summary of current issues
  
  ![summary current tasks](https://github.com/user-attachments/assets/7eb9f38f-4041-4ebc-ac38-409053732506)

- Creating a new merged issue
  
  ![create task-0](https://github.com/user-attachments/assets/b9c2e37e-899b-4076-b61a-77552e06555b)

  ![create task-1](https://github.com/user-attachments/assets/5b5ccd10-cab1-4395-864b-4a3e81cbf6e5)

- Deleting the duplicated issues

  ![delete old tasks](https://github.com/user-attachments/assets/b35ff6a5-a929-4b6b-9ac6-44888e647712)

  ![confirm delete](https://github.com/user-attachments/assets/2d8b924a-f436-4647-9b5b-e1b773bfcba3)

