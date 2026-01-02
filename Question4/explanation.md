Here is the content for Question 4, formatted exactly as requested.

Question 4: Processes and System Monitoring

    System Uptime Verification Command: uptime -p Explanation: The uptime command with the -p flag displays the system's operational duration in a "pretty" format, making it easy to read exactly how long the system has been running since the last boot.

    User Process Listing Command: ps -u $(whoami) Explanation: This command uses ps to snapshot the current processes and filters them with the -u flag to show only those owned by the current logged-in user.

    CPU Usage Analysis Command: top -n 1 -o %CPU Explanation: The top command provides a dynamic view of system processes. Running it with -n 1 performs a single iteration, and -o %CPU sorts the output to immediately highlight the process consuming the most processor resources.

    Background Process Execution Command: sleep 500 &; jobs Explanation: The sleep 500 & command starts a dummy process that pauses for 500 seconds, and the ampersand symbol & instructs the shell to run it in the background. The jobs command then confirms that the process is active and running without blocking the terminal.

    Process Priority Management Command: renice -n 10 -p 12345 Explanation: The renice command alters the scheduling priority of an existing process. By setting the niceness value to 10 for the specified process ID (PID), I lowered its priority, meaning it will claim fewer CPU resources compared to other tasks.

    Memory Usage Monitoring Command: free -h Explanation: The free command displays the total amount of free and used physical and swap memory in the system. The -h flag ensures the values are presented in human-readable units like megabytes and gigabytes.

    Disk Space Inspection Command: df -h ~ Explanation: The df command reports file system disk space usage. By targeting the home directory (~), it displays the specific partition where my user data resides, showing available and used space in a readable format.

    Shell Identification Command: echo $SHELL Explanation: This command prints the value of the SHELL environment variable, which identifies the absolute path of the command-line interpreter (shell) currently being used by the session.

    Output Redirection Command: uname -a > system_report.txt Explanation: The uname -a command gathers all available system information. Instead of printing it to the screen, the > operator redirects this output into a new file named system_report.txt.

    Disk Usage Visualization Command: ncdu Explanation: The ncdu (NCurses Disk Usage) tool launches an interactive, text-based graphical interface that scans the directory structure. It provides a visual and navigational way to analyze disk usage and identify which specific directories or files are consuming the most space.
