### Explanation of pwd

The pwd (print working directory) command displays the full, absolute path of the current working directory. It's a simple, essential tool for confirming your location in the filesystem, especially when navigating complex directory structures.

**Key Options and Usage**:

-   **No arguments**: pwd prints the absolute path of the current directory (e.g., pwd might output /home/yourusername).
-   **-L**: Print the logical path, including symbolic links (default behavior; e.g., if /var/log is a symlink, pwd -L shows /var/log).
-   **-P**: Print the physical path, resolving symbolic links (e.g., if /var/log links to /var/spool/log, pwd -P shows /var/spool/log).
-   **No directory argument**: pwd always operates on the current directory; it doesn't accept a directory path (e.g., pwd /etc is invalid).

**Common Notes**:

-   Outputs to stdout, so it can be redirected (e.g., pwd > dir.txt) or piped (e.g., pwd | grep home).
-   Exit status is 0 unless an error occurs (e.g., if the current directory is deleted).
-   Rarely encounters permission issues, as it reads the shell's current directory.

### 10 Problem Scenarios/Requirements for pwd (Basic to Advanced)

*Note*: Hints indicate if other commands are needed.

1.  **Basic: Display Current Directory**\
    Requirement: From your home directory, use pwd to print the current directory path. Confirm the output is /home/yourusername (replace yourusername with your actual username).\
    *Hint*: Uses pwd alone.
2.  **Basic: Verify Directory After Navigation**\
    Requirement: Navigate to /etc using cd /etc, then use pwd to confirm you're in /etc.\
    *Hint*: Requires cd with pwd.
3.  **Basic: Redirect Output to File**\
    Requirement: In your home directory, use pwd to print the current directory and redirect the output to a file named current_dir.txt. Display the file contents to verify.\
    *Hint*: Requires cat or similar with pwd.
4.  **Intermediate: Check Directory After Multiple Navigations**\
    Requirement: From your home directory, navigate to /var/log, then up two levels to /var, then to /tmp. Use pwd to confirm you're in /tmp.\
    *Hint*: Requires cd with pwd.
5.  **Intermediate: Compare with Previous Directory**\
    Requirement: Navigate to /usr/bin, use pwd to note the path, then move to /usr/local and use pwd again. Confirm the outputs differ and note the paths.\
    *Hint*: Requires cd with pwd.
6.  **Intermediate: Use in a Deep Directory Structure**\
    Requirement: Create a directory structure mkdir -p ~/projects/code/src. Navigate to src and use pwd to confirm the full path (e.g., /home/yourusername/projects/code/src).\
    *Hint*: Requires mkdir and cd with pwd.
7.  **Intermediate: Logical Path with Symlink**\
    Requirement: Create a symbolic link ln -s /var/log ~/log_link in your home directory. Navigate to log_link and use pwd with the logical path option to confirm it shows /home/yourusername/log_link.\
    *Hint*: Requires ln and cd with pwd.
8.  **Advanced: Physical Path with Symlink**\
    Requirement: Using the log_link from scenario 7, navigate to log_link and use pwd with the physical path option to confirm it shows the resolved path (e.g., /var/log). Compare with scenario 7's output.\
    *Hint*: Requires ln and cd with pwd.
9.  **Advanced: Handle Deleted Directory**\
    Requirement: Create a directory /tmp/test_dir, navigate to it, and use pwd to confirm the path. In another terminal (or background with &), delete the directory (rm -r /tmp/test_dir). Run pwd again and note any error or output change.\
    *Hint*: Requires mkdir, cd, rm with pwd.
10. **Advanced: Combine with Environment Variable**\
    Requirement: Set an environment variable export MYDIR=/usr/share. Navigate to $MYDIR and use pwd to confirm the path is /usr/share. Redirect the output to mydir.txt and verify the file contents.\
    *Hint*: Requires export, cd, and cat with pwd.