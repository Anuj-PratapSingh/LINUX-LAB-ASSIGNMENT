Question 1: Environment Verification

    User Identity Verification Command: id Explanation: This command displays the current user's ID (uid), group ID (gid), and group memberships, confirming the identity of the user currently logged into the system.

    Workspace Validation Command: pwd; ls -l Explanation: pwd prints the absolute path of the current working directory, and ls -l lists all files and directories in that location using the long format to show detailed permissions and ownership.

    Environment Confirmation File Command: echo "Linux user environment verified" > user_info.txt Explanation: The echo command generates the specified text string, and the > redirection operator writes that output into a new file named user_info.txt.

    File Integrity Check Command: wc -c user_info.txt Explanation: The wc (word count) command with the -c option counts and displays the specific number of bytes (characters) contained in the user_info.txt file.

    Learning the Tools Command: man mkdir Explanation: This command opens the manual page for mkdir. A useful option identified is -p, which allows the creation of parent directories if they do not already exist (e.g., creating a nested folder structure in one command).

    Home Directory Inspection Command: ls -l ~ | sort Explanation: ls -l ~ lists the contents of the home directory in long format, and the pipe | sends this output to sort, which arranges the lines alphabetically.

    Log Investigation Command: grep "admin" log.txt Explanation: The grep command searches through the contents of log.txt for the specific string "admin" and prints only the lines where a match is found.

    System Information Check Command: uname -r Explanation: The uname command with the -r flag displays the specific release version of the Linux kernel that is currently running on the system.

    Network Connectivity Test Command: ping -c 4 www.google.com Explanation: This sends 4 ICMP echo request packets to the specified domain (Google) to verify that the system has active internet connectivity and can receive responses.

    System Health Awareness Command: uptime Explanation: This command provides a summary of system status, including how long the system has been running, the number of active users, and the system load averages over the last 1, 5, and 15 minutes.
