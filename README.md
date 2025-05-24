# Linux Commands by Category

1. **File Storage Locations**
   1. [cd](/docs/1_File_Storage_Locations/cd.md): Change directory, most fundamental navigation command.
   2. [ls](/docs/1_File_Storage_Locations/ls.md): List directory contents, widely used for exploration.
   3. [pwd](/docs/1_File_Storage_Locations/pwd.md): Print working directory, simple and essential.
   4. [mkdir](/docs/1_File_Storage_Locations/mkdir.md): Create directories, basic file system modification.
   5. rmdir: Remove empty directories, slightly more specific.
   6. find: Search for files/directories, more complex with options.
   7. locate: Faster search using a database, requires understanding of updatedb.
   8. tree: Display directory structure, less common but visually informative.

2. **Text Manipulation**
   1. grep: Search for patterns, widely used and straightforward.
   2. fgrep: Fixed-string search, simpler than regex-based grep.
   3. sort: Sort lines, simple and common.
   4. uniq: Remove duplicate lines, often used with sort.
   5. wc: Count lines/words/characters, basic text analysis.
   6. cut: Extract fields/columns, straightforward text slicing.
   7. tr: Translate or delete characters, simple transformations.
   8. paste: Merge lines from files, less common but intuitive.
   9. nl: Number lines, specific but easy to use.
   10. strings: Extract printable strings from files, niche but simple.
   11. expand: Convert tabs to spaces, specific text formatting.
   12. unexpand: Convert spaces to tabs, counterpart to expand.
   13. fold: Fold lines into columns, specialized formatting.
   14. fmt: Simple text formatter, less common but straightforward.
   15. comm: Compare sorted files, requires sorted input.
   16. sed: Stream editor for complex text manipulation.
   17. awk: Powerful text processing with scripting, more complex.
   18. csplit: Split files by context, advanced file manipulation.
   19. bc: Arbitrary-precision calculator, requires understanding of math expressions.
   20. printf: Formatted output, advanced formatting control.

3. **Finding and Grep**
   1. grep: Basic pattern search in files.
   2. fgrep: Fixed-string search, simpler than regex.
   3. zgrep: Grep for compressed files, builds on grep.
   4. find: Advanced file search with multiple criteria.

4. **Permissions**
   1. chmod: Change file permissions, core and widely used.
   2. chown: Change file ownership, common admin task.
   3. chgrp: Change group ownership, similar to chown.
   4. umask: Set default permissions for new files, less frequent.
   5. getfacl: View access control lists, requires ACL knowledge.
   6. setfacl: Set access control lists, more complex.
   7. lsattr: List file attributes, niche and system-specific.
   8. chattr: Change file attributes, advanced and less common.

5. **User Management**
   1. whoami: Display current user, simplest identity check.
   2. who: List logged-in users, straightforward.
   3. id: Display user/group IDs, slightly more detailed.
   4. groups: List user’s groups, simple group check.
   5. passwd: Change user password, common task.
   6. su: Switch user, basic privilege escalation.
   7. sudo: Execute commands as another user, widely used.
   8. useradd: Create a new user, core admin task.
   9. groupadd: Create a new group, similar to useradd.
   10. adduser: Interactive user creation, user-friendly wrapper.
   11. usermod: Modify user attributes, more complex.
   12. gpasswd: Manage group passwords, specific group admin task.
   13. userdel: Delete a user, potentially destructive.
   14. groupdel: Delete a group, similar to userdel.
   15. chage: Manage password aging, advanced user policy.

6. **Compression and Archiving**
   1. zip: Create compressed archives, simple and cross-platform.
   2. unzip: Extract zip archives, counterpart to zip.
   3. tar: Create/extract archives, versatile and common.
   4. gzip: Compress files, widely used with tar.
   5. gunzip: Decompress gzip files, counterpart to gzip.
   6. bzip2: Compress with better ratio, less common but similar to gzip.

7. **Process Management**
   1. ps: List processes, basic process inspection.
   2. top: Real-time process monitoring, interactive and common.
   3. htop: Enhanced top, user-friendly but requires installation.
   4. jobs: List background jobs, simple job control.
   5. fg: Bring job to foreground, basic job management.
   6. bg: Run job in background, counterpart to fg.
   7. kill: Terminate process by PID, core process control.
   8. pkill: Kill processes by name, builds on kill.
   9. killall: Kill all processes by name, similar to pkill.
   10. pgrep: Find process IDs by name, useful for scripting.
   11. pidof: Find PIDs of a program, similar to pgrep.
   12. nice: Set process priority, affects scheduling.
   13. renice: Change priority of running process, builds on nice.
   14. nohup: Run process immune to hangups, for persistent tasks.
   15. wait: Wait for background processes, scripting utility.
   16. pstree: Display process tree, visual process hierarchy.
   17. pmap: Display process memory map, advanced diagnostics.

8. **Monitoring and Logging**
   1. uptime: Display system uptime, simple system status.
   2. free: Show memory usage, basic resource check.
   3. top: Real-time system monitoring, widely used.
   4. htop: Enhanced top, more user-friendly.
   5. w: Show who is logged in, simple user activity.
   6. last: List last logged-in users, straightforward.
   7. nproc: Show number of CPU cores, basic hardware info.
   8. lscpu: Display CPU details, detailed but accessible.
   9. lsblk: List block devices, clear storage overview.
   10. lspci: List PCI devices, hardware diagnostics.
   11. lsusb: List USB devices, similar to lspci.
   12. lshw: List hardware details, comprehensive hardware info.
   13. dmidecode: Display system BIOS info, advanced hardware.
   14. tail: Show end of files/logs, common for logs.
   15. dmesg: Display kernel messages, system diagnostics.
   16. journalctl: View systemd logs, modern log management.
   17. watch: Run command repeatedly, simple monitoring.
   18. vmstat: Virtual memory stats, system performance.
   19. iostat: I/O statistics, disk performance.
   20. mpstat: CPU statistics, detailed processor info.
   21. pidstat: Process statistics, granular process monitoring.
   22. sar: System activity reporting, historical data.
   23. lsof: List open files, advanced resource tracking.
   24. iftop: Network traffic monitoring, network-specific.
   25. nload: Network bandwidth monitoring, similar to iftop.
   26. inxi: System information tool, comprehensive but niche.
   27. hdparm: Disk performance and settings, storage-specific.
   28. iw: Wireless device management, network-specific.
   29. iwconfig: Configure wireless interfaces, builds on iw.
   30. iwlist: List wireless networks, wireless diagnostics.
   31. acpi: Display power/battery info, power management.
   32. nmon: Advanced performance monitor, requires installation.
   33. sysstat: Collection of performance tools, advanced suite.

9. **Networking**
   1. ping: Test network connectivity, simplest diagnostic.
   2. whois: Query domain info, straightforward lookup.
   3. nslookup: DNS lookup, basic DNS query.
   4. dig: Advanced DNS lookup, more detailed than nslookup.
   5. curl: Transfer data via URLs, common for APIs.
   6. wget: Download files, simpler than curl for downloads.
   7. ifconfig: Display network interfaces, legacy but common.
   8. ip: Modern network configuration, replaces ifconfig.
   9. nmcli: Manage NetworkManager, user-friendly network control.
   10. netstat: Display network stats, versatile but legacy.
   11. ss: Modern replacement for netstat, more efficient.
   12. arp: Display ARP table, network troubleshooting.
   13. route: Display routing table, network routing.
   14. traceroute: Trace network path, diagnostic tool.
   15. mtr: Combine ping and traceroute, enhanced diagnostics.
   16. ethtool: Display NIC settings, hardware-specific.
   17. ifstat: Network interface stats, traffic monitoring.
   18. iftop: Real-time network traffic, advanced monitoring.
   19. netcat: Network utility for connections, versatile.
   20. telnet: Test connectivity to ports, legacy but simple.
   21. tcpdump: Capture network packets, advanced analysis.
   22. nmap: Network scanning, security and diagnostics.
   23. iptables: Configure firewall rules, security-focused.
   24. systemd-resolve: DNS resolution, modern resolver.

10. **Disk and Filesystem Management**
    1. df: Display disk usage, basic storage check.
    2. du: Estimate file space usage, complements df.
    3. mount: Mount filesystems, common admin task.
    4. umount: Unmount filesystems, counterpart to mount.
    5. fdisk: Partition disks, core disk management.
    6. fsck: Check/repair filesystems, filesystem maintenance.
    7. mkfs: Create filesystems, builds on partitioning.
    8. mkswap: Create swap space, specific to memory.
    9. swapon: Enable swap space, activates mkswap.
    10. smartctl: Monitor disk health, advanced diagnostics.
    11. resize2fs: Resize ext filesystems, filesystem tuning.
    12. lvcreate: Create logical volumes, LVM-specific.
    13. mdadm: Manage RAID arrays, advanced storage.

11. **Systemd**
    1. systemctl: Manage services, core systemd command.
    2. journalctl: View system logs, log management.
    3. systemd-analyze: Analyze boot performance, advanced diagnostics.

12. **Proc File System**
    1. cat: Display /proc file contents, only command.

13. **SSH**
    1. ssh: Remote login, core SSH command.
    2. scp: Secure file transfer, builds on ssh.
    3. sftp: Secure FTP, interactive file transfer.
    4. ssh-keygen: Generate SSH keys, key management.
    5. sshd_config: Configure SSH daemon, server-side setup.

14. **Automation and Scheduling**
    1. crontab: Schedule recurring tasks, simplest automation.
    2. at: Schedule one-time tasks, complements crontab.
    3. ansible: Configuration management, complex automation.
    4. puppet: Infrastructure automation, similar to ansible.
    5. chef: Configuration management, advanced orchestration.

15. **Security**
    1. iptables: Configure firewall rules, core security.
    2. firewall-cmd: Manage firewalld, modern firewall tool.
    3. firewall-config: GUI for firewall settings, user-friendly.
    4. sestatus: Check SELinux status, simple SELinux query.
    5. ssh-keygen: Generate SSH keys, secure authentication.
    6. sshd_config: Configure SSH server, server security.
    7. visudo: Edit sudoers file, privilege management.
    8. google-authenticator: Set up 2FA, enhances security.
    9. setenforce: Toggle SELinux mode, SELinux control.
    10. setsebool: Set SELinux booleans, fine-grained SELinux.
    11. semanage: Manage SELinux policies, advanced SELinux.
    12. restorecon: Restore SELinux context, SELinux maintenance.
    13. cryptsetup: Manage encrypted filesystems, advanced.

16. **Certificates**
    1. openssl: Manage SSL/TLS certificates, core crypto tool.
    2. certbot: Automate certificate issuance, builds on openssl.

17. **Kernel and System**
    1. date: Display/set system date, simple system command.
    2. cal: Display calendar, straightforward utility.
    3. uname: Display system info, basic system query.
    4. hostname: Display hostname, simple system info.
    5. hostnamectl: Manage hostname, modern control.
    6. ntp: Synchronize time, network-based.
    7. sysctl: Configure kernel parameters, system tuning.
    8. lsmod: List kernel modules, kernel diagnostics.
    9. modprobe: Load/unload kernel modules, kernel management.
    10. kexec: Boot new kernel, advanced system control.
    11. livepatch: Apply kernel patches live, cutting-edge.
    12. init: Manage runlevels, legacy system control.
    13. halt: Stop system, destructive system command.

18. **Resource Management**
    1. ulimit: Set/report resource limits, only command.

19. **Other Tools**
    1. echo: Print text, simplest output command.
    2. cat: Display file contents, basic file viewing.
    3. head: Show start of file, complements cat.
    4. tail: Show end of file, common for logs.
    5. less: View files page-wise, improved file browsing.
    6. more: View files page-wise, older than less.
    7. touch: Create/update files, basic file management.
    8. cp: Copy files, core file operation.
    9. mv: Move/rename files, similar to cp.
    10. rm: Remove files, potentially destructive.
    11. ln: Create links, slightly more complex.
    12. nano: Simple text editor, user-friendly.
    13. file: Determine file type, basic file inspection.
    14. man: Display command manuals, essential help.
    15. help: Display command help, simpler than man.
    16. type: Show command type, command introspection.
    17. apropos: Search man pages, advanced help.
    18. history: List command history, shell utility.
    19. alias: Create command shortcuts, shell customization.
    20. unalias: Remove aliases, counterpart to alias.
    21. env: Display environment variables, basic env management.
    22. printenv: Print specific env variables, similar to env.
    23. export: Export variables to child processes, env control.
    24. chsh: Change user shell, user customization.
    25. passwd: Change passwords, user task.
    26. chpasswd: Bulk password changes, advanced user management.
    27. sleep: Pause execution, simple scripting utility.
    28. tee: Redirect output to file and stdout, scripting tool.
    29. xargs: Build commands from input, scripting utility.
    30. test: Evaluate conditions, core scripting command.
    31. source: Execute script in current shell, scripting utility.
    32. logger: Log messages to syslog, system logging.
    33. getopt: Parse command-line options, scripting complexity.
    34. getopts: Parse command-line options, simpler than getopt.
    35. mail: Send emails, basic communication.
    36. shred: Securely delete files, security-focused.
    37. dd: Low-level data copy, advanced file operation.
    38. od: Dump files in octal, low-level file inspection.
    39. time: Measure command execution, performance analysis.
    40. tput: Terminal formatting, advanced terminal control.
    41. apt: Debian package manager, common package tool.
    42. dpkg: Low-level Debian package tool, complements apt.
    43. yum: Red Hat package manager, similar to apt.
    44. dnf: Modern Red Hat package manager, replaces yum.
    45. pacman: Arch Linux package manager, distro-specific.
    46. portage: Gentoo package manager, advanced package system.
    47. lsb_release: Display Linux Standard Base info, system query.
    48. software-properties-common: Manage software sources, package config.
    49. git: Version control, development tool.
    50. pip: Python package manager, development utility.
    51. virtualenv: Python virtual environments, development setup.
    52. mysqldump: Backup MySQL databases, database admin.
    53. gpg: Encryption and signing, security tool.
    54. docker: Container management, modern DevOps.
    55. kubeadm: Kubernetes cluster setup, advanced orchestration.
    56. aws: AWS CLI, cloud management.
    57. terraform: Infrastructure as code, advanced DevOps.
    58. rsnapshot: Backup tool, advanced backup management.
    59. inotifywait: Monitor filesystem events, advanced scripting.
    60. ab: Apache benchmarking, web performance testing.
    61. jstack: Java thread dump, Java diagnostics.
    62. jmap: Java memory map, advanced Java diagnostics.
