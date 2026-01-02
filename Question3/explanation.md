Question 3: Links and Disk Usage

    File Creation Command: echo "Original Data" > ~/sample_data.txt Explanation: This command creates a text file named sample_data.txt in the home directory and initializes it with the text string Original Data.

    Hard Link Creation Command: ln ~/sample_data.txt sample_hard.txt Explanation: The ln command creates a hard link named sample_hard.txt. This new file entry points to the exact same physical data location (inode) on the hard drive as the original file.

    Symbolic Link Creation Command: ln -s ~/sample_data.txt sample_soft.txt Explanation: The ln command with the -s flag creates a symbolic (soft) link named sample_soft.txt. This file acts as a shortcut that points to the file path of the original file rather than the data itself.

    Inode Verification Command: ls -i ~/sample_data.txt sample_hard.txt sample_soft.txt Explanation: The ls command with the -i option lists the files along with their inode numbers, revealing that the original file and hard link share the same number, while the soft link has a unique number.

    Inode Analysis Command: ls -li ~/sample_data.txt sample_hard.txt sample_soft.txt Explanation: The output confirms that sample_data.txt and sample_hard.txt share the same inode because they are effectively the same file data accessed via different names. The sample_soft.txt file has a different inode because it is a separate file that simply contains a text pointer to the original file's location.

    File Metadata Inspection Command: stat ~/sample_data.txt Explanation: The stat command displays comprehensive metadata for the file, including its exact size in bytes, block count, inode number, file type, and precise access/modification timestamps.

    Disk Usage Check Command: du -h ~ Explanation: The du (disk usage) command estimates the file space usage for the home directory, and the -h flag ensures the output is presented in a human-readable format (e.g., KB, MB) rather than block counts.

    File Size Overview Command: ls -lh ~ Explanation: This command lists the files in the home directory with their specific file sizes displayed in human-readable units, making it easier to identify how much space each individual file consumes.

    Link Deletion Test Command: rm sample_soft.txt; cat ~/sample_data.txt Explanation: The rm command deletes the symbolic link, and the subsequent cat command prints the content of the original file. This demonstrates that deleting a soft link removes only the shortcut, leaving the original data intact.

    Disk Utility Demonstration Command: df -h Explanation: The df command reports the file system disk space usage. The -h option makes the output readable, showing the total size, used space, and available free space for the file system where the home directory resides.
