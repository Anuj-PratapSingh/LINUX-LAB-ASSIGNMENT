Question 2: File & Directory Management

    Project Workspace Setup Command: mkdir ~/documents Explanation: This command creates a new directory named documents located directly within the current user's home directory to serve as the workspace for project files.

    File Creation Command: cd ~/documents; touch plan.txt Explanation: The cd command changes the current working directory to the new documents folder, and touch creates an empty file named plan.txt within it.

    Content Addition Command: echo "Initial project draft and notes." > plan.txt Explanation: The echo command takes the provided string of text and redirects it into plan.txt, adding content to the previously empty file.

    File Metadata Verification Command: ls -l plan.txt Explanation: This command lists the file details in long format, displaying the read/write permissions, the owner (which matches my username), the file size, and the modification timestamp.

    File Duplication Command: cp plan.txt plan_copy.txt Explanation: The cp command creates an exact duplicate of the existing plan.txt file and names the new copy plan_copy.txt in the same directory.

    Directory Renaming Command: mv ~/documents ~/project_documents Explanation: The mv command is used here to rename the directory. It takes the existing documents folder and changes its name to project_documents to better reflect the scope of the work.

    Archival Structure Command: mkdir ~/project_documents/archive Explanation: This creates a new subdirectory named archive inside the recently renamed project_documents folder to serve as a storage location for backup files.

    File Organization Command: mv ~/project_documents/plan_copy.txt ~/project_documents/archive/ Explanation: The mv command moves the plan_copy.txt file from the main project directory into the nested archive subdirectory, organizing the file structure.

    Recursive Listing Command: ls -R ~/project_documents Explanation: The ls command with the -R (recursive) flag displays the contents of the main directory and automatically lists the contents of all subdirectories, showing the complete file tree.

    Path Verification Command: readlink -f ~/project_documents/archive/plan_copy.txt Explanation: This command resolves and displays the full absolute path of the moved file, confirming its exact location on the disk starting from the root directory.
