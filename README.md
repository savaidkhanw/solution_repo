# solution_repo
solutions for roadmap.sh
Server Stats Script

This script, server-stats.sh, provides basic server performance statistics and additional information about the system. It is designed to run on any Linux server and outputs the following stats:

Features

Basic Stats

Total CPU Usage

Total Memory Usage: Includes free and used memory with percentages.

Total Disk Usage: Includes free and used disk space with percentages.

Top 5 Processes by CPU Usage

Top 5 Processes by Memory Usage

Additional Stats (Stretch Goals)

Operating System Version

Uptime and Load Average

Logged-in Users

Failed Login Attempts

Prerequisites

A Linux server with the following commands installed:

awk

free

df

ps

lsb_release (optional for OS version)

grep (optional for failed logins)

Root or appropriate user permissions to read logs (for failed login attempts).

Installation

Clone this repository or download the server-stats.sh file.

Make the script executable:

chmod +x server-stats.sh

Usage

Run the script directly from the terminal:

./server-stats.sh

The script will output the server stats in a clean, readable format.

Example Output

----- Server Performance Stats -----

Total CPU Usage:
15.32%

Total Memory Usage:
Used: 2048MB (50.00%), Free: 2048MB (50.00%)

Total Disk Usage:
Used: 50G (25%), Free: 150G

Top 5 Processes by CPU Usage:
PID   PPID CMD       %MEM  %CPU
1234  1    process1  1.2   30.0
...

Top 5 Processes by Memory Usage:
PID   PPID CMD       %MEM  %CPU
2345  1    process2  15.0  10.0
...

----- Additional Server Information -----

Operating System Version:
Ubuntu 20.04.3 LTS

Uptime and Load Average:
 12:34:56 up  1 day,  3:21,  2 users,  load average: 0.15, 0.10, 0.05

Logged-in Users:
user1   pts/0   2024-12-25 12:00 (192.168.0.1)

Failed Login Attempts:
42
Total CPU Usage:
15.32%

Total Memory Usage:
Used: 2048MB (50.00%), Free: 2048MB (50.00%)

Total Disk Usage:
Used: 50G (25%), Free: 150G

Top 5 Processes by CPU Usage:
PID   PPID CMD       %MEM  %CPU
1234  1    process1  1.2   30.0
...

Top 5 Processes by Memory Usage:
PID   PPID CMD       %MEM  %CPU
2345  1    process2  15.0  10.0
...

----- Additional Server Information -----

Operating System Version:
Ubuntu 20.04.3 LTS

Uptime and Load Average:
 12:34:56 up  1 day,  3:21,  2 users,  load average: 0.15, 0.10, 0.05

Logged-in Users:
user1   pts/0   2024-12-25 12:00 (192.168.0.1)

Failed Login Attempts:
42

Customization

Feel free to modify the script to include more stats or adjust the format according to your needs. For example:

Add network usage stats.

Monitor specific services or processes.

Troubleshooting

Permission Denied: Ensure the script is executable:

chmod +x server-stats.sh

Command Not Found: Make sure all required commands are installed on the server.

License

This project is licensed under the MIT License. Feel free to use, modify, and distribute it as needed.

