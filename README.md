# pc-troubleshooting-toolkit-project
Help Desk Final Project for CIS20638A0 Trevor Lewis

## Project Purpose
- Technicians initially had trouble finding the right tools to be able to solve issues for users
- This PC troubleshooting toolkit should help technicians find the all the tools they need in one convenient package
- This toolkit is meant to be used by help desk and IT support technicians to carry out their tasks and responsibilities
- With this toolkit, technicians should be able to troubleshoot more efficiently and be able to move on to the next user that needs help

## Tools & Technologies Used
- PowerShell
- GitHub
- Git
- Windows environment
- ChatGPT
- Visual Studio Code

## Setup Instructions

### 1. **Prerequisites**
- PowerShell (execute scripts)
- GitHub (repository)
- Git (version control)
- Visual Studio Code (IDE)
- Windows 11

### 2. **Installation**
- Clone the repository:

  git clone https://github.com/atnguyen246/pc-troubleshooting-toolkit-project

- Set Your Global Git Username & Email
  
  These settings apply to all repositories on your system:

    git config --global user.name "Your Name"
    
    git config --global user.email "you@example.com"

- Set Username & Email for a Single Repository Only

  Run these inside the project folder:

    git config user.name "Your Name"
    
    git config user.email "you@example.com"

- Verify Your Settings
  
  All repositories:

    git config --global --list

  or for repo-specific settings:

    git config --list

### 3. File/Folder Structure
help-desk-docs/ – Contains internal documentation, knowledge base articles, and troubleshooting guides

scripts/ – Contains a diagnostic script and user issue logger script

ai/ – Contains ChatGPT prompts and transcripts used to build this project

assets/ – Contains assets used in the project like diagrams, images, logs, reports, and screenshots

### 4. How to Run
- Use troubleshooting flowchart to help in identifying user issue
- Utilize diagnostic script to find information about device:
  - Open PowerShell
  - Navigate to scripts directory in the cloned repository
  - Execute script using this command:
    - ./diagnostic_script.ps1
- Initiate user issue logger script to create initial log:
  - Open PowerShell
  - Navigate to scripts directory in the cloned repository
  - Execute script using this command:
    - ./user_issue_logger_script.ps1
- If problem is a common issue, use resolving_common_issues knowledge base article to solve it
- Use test_result_template to record information about the user, device, problem, steps taken, and the follow-up
- Send response to user using it_issue_email_response_template to help 

## How AI Was Used in This Project
Drafting documentation (document templages, troubleshooting flowchart, KB articles)

Generating or refining code snippets

Brainstorming workflows or automation logic

Providing template structures (like this README)

Assisting with project planning or problem-solving

AI-generated parts:
- Repository structure
- help-desk-docs
- project-assets
- scripts

Manually reviewed or modified parts:
- README.md
- chatgpt_prompts
- chatgpt_output
- File names

## Additional Notes

Add any final remarks, credits, or future improvements:

Planned features

Known issues

Contribution guidelines

License information