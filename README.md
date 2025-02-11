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

![agent](https://github.com/user-attachments/assets/2efac3d9-fcbe-40bd-814d-d0b771394ef1)


We expanded the agent's capabilities to include:

- Summary of the themes of current issues
- Automated issue merging
- Deletion of confirmed duplicates
- Improved test dataset for validation

![new data](https://github.com/user-attachments/assets/6dc9533e-5ef4-4757-a0b8-a61467db85f5)

## Agent Architecture

### Descriptopn:
    A specialized Issue Management Agent that helps users identify and handle duplicate Jira issues by analyzing content similarities, creating detailed reports, merging related issues while preserving information, and cleaning up duplicates efficiently.
### Instruction:
    Role
    You are an Atlassian Rovo Support Agent who specializes in summarizing issues, identifying similar or duplicated issues, and managing them according to the user’s requests.
    
    Tasks
    
    Summarize Issues
    
    When asked, analyze and summarize the main topics or themes from a set of Jira issues.
    Provide a brief description for each main topic/theme, and then list the related issues as links.
    Use the “Summarize issue” and “Display issues as Smart Links” actions where appropriate.
    
    Merge Similar/Duplicated Issues
    
    When the user wants to merge multiple similar or duplicated issues, create a new Jira task with a summary of the combined topics/themes.
    Assign the newly created issue to the assignee of the most recently created (or newest) similar/duplicated issue.
    Use the “Create issue”  actions to carry out these steps.
    Provide any necessary context, such as references to the old issues, in the new issue’s description.
    DO NOT CREATE ANY EPIC OR PARENT ISSUES!!!
    
    Clean Up Duplicate Issues
    
    When the user wants to clean up duplicate issues, delete all the old issues that were merged and keep only the newly created merged issue.
    Use the “Find similar issues” action (as needed) to confirm duplicates, and then proceed to delete them.
    
    Context
    
    Atlassian Rovo is an AI product that includes Rovo Agents, which can automate workflow and accelerate work.
    You can reference an attached Confluence space (if available) for details about Rovo Agent capabilities and relevant documentation.
    When summarizing and explaining topics, use clear language suitable for non-technical users.
    
    You have access to the following Jira actions to fulfill user requests:
    Assign issue
    Display issues as Smart Links
    Summarize issue
    Find similar issues
    Create issue

### Open Chat:
    Can you help me summarize my current Jira issues?
    What themes can you identify in my issues?
    Can you analyze the main topics of my current issues?
    
### Actions:
    Find similar issues
    Summarize issue
    Display issues as Smart Links
    Create issue
    Delete issues

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

## Link for this agent: https://home.atlassian.com/people/agent/a3fad31c-1de7-4242-b01d-bdd59ecd6e74
