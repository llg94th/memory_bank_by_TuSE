[Vietnamese version (Phiên bản tiếng Việt)](README_vi.md)
[memory-bank-instructions](rule/memory-bank-instructions.md)

# How to use Memory Bank and Modes to make work faster
## Principles of operation
### Memory Bank:

Memory Bank is a set of resources needed to complete tasks automatically for a project. It includes resources related to tools, systems, classes, and basic terminology. It is used to solve problems related to common tasks and difficulties in bringing a project to completion.

### Modes:

Modes is a set of questions and goals for a project. It includes questions and goals related to common tasks and difficulties in bringing a project to completion. It is used to solve problems related to common tasks and difficulties in bringing a project to completion.

## How to setup:
### Cursor: custom Modes 
    - https://docs.cursor.com/en/agent/modes#agent
### VS Code: custom Chat Modes
    - https://code.visualstudio.com/docs/copilot/customization/overview
### Custom Rules
    Use memory-bank-instructions.md to create custom rules.
    
## How to use Memory Bank:
### Working with Memory Bank
#### Core Workflows
Memory Bank Initialization
The initialization step is critically important as it establishes the foundation for all future interactions with your project. When you request initialization with the command initialize memory bank, XYZ Code will:

1. Perform an exhaustive analysis of your project, including:
    - All source code files and their relationships
    - Configuration files and build system setup
    - Project structure and organization patterns
    - Documentation and comments
    - Dependencies and external integrations
    - Testing frameworks and patterns
2. Create comprehensive memory bank files in the ./memory-bank folder
3. Provide a detailed summary of what it has understood about your project
4. Ask you to verify the accuracy of the generated files

***Important***:

Take time to carefully review and correct the generated files after initialization. Any misunderstandings or missing information at this stage will affect all future interactions. A thorough initialization dramatically improves XYZ Code's effectiveness, while a rushed or incomplete initialization will permanently limit its ability to assist you effectively.

#### Memory Bank Updates
Memory Bank updates occur when:

1. XYZ Code discovers new project patterns
2. After implementing significant changes
3. When you explicitly request with update memory bank
4. When context needs clarification

To execute a Memory Bank update, XYZ Code will:

1. Review ALL project files
2. Document the current state
3. Document insights and patterns
4. Update all memory bank files as needed

You can direct XYZ Code to focus on specific information sources by using commands like update memory bank using information from @/Makefile.

#### Regular Task Execution
At the beginning of every task, XYZ Code:

1. Reads ALL memory bank files
2. Includes [Memory Bank: Active] at the beginning of its response
3. Provides a brief summary of its understanding of your project
4. Proceeds with the requested task

At the end of a task, XYZ Code may suggest updating the memory bank if significant changes were made, using the phrase: "Would you like me to update memory bank to reflect these changes?"

#### Add Task Workflow
When you complete a repetitive task that follows a similar pattern each time, you can document it for future reference. This is particularly useful for tasks like adding features that follow existing patterns

To document a task, use the command add task or store this as a task. XYZ Code will:

1. Create or update the tasks.md file in the memory bank folder
2. Document the task using current context:
    - Task name and description
    - List of files that need to be modified
    - Step-by-step workflow
    - Important considerations
    - Example implementation

When starting a new task, XYZ Code will check if it matches any documented tasks and follow the established workflow to ensure no steps are missed.

#### Key Commands

- initialize memory bank - Use when starting a new project
- update memory bank - Initiates a comprehensive re-analysis of the contextual documentation for the current task. Caution: This is resource-intensive and not recommended for "lightweight" models due to potentially reduced effectiveness. Can be used multiple times, well combinable with specific instructions, e.g. update memory bank using information from @/Makefile
- add task or store this as a task - Documents a repetitive task for future reference

#### Status Indicators
XYZ Code uses status indicators to clearly communicate Memory Bank status:

- [Memory Bank: Active] - Indicates Memory Bank files were successfully read and are being used
- [Memory Bank: Missing] - Indicates Memory Bank files could not be found or are empty
These indicators appear at the beginning of XYZ Code's responses, providing immediate confirmation of Memory Bank status.

#### Documentation Updates
Memory Bank updates should automatically occur when:

- You discover new patterns in your project
- After implementing significant changes
- When you explicitly request with update memory bank
- When you feel context needs clarification
