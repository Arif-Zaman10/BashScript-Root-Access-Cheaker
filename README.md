📌 Overview

This project contains a simple Bash script (check.sh) that checks if the current user has root privileges.
It demonstrates the use of environment variables and conditional statements in Bash.

⚙️ How It Works

The script checks the value of the $UID variable:

    UID = 0 → You are root.

    UID ≠ 0 → You are a normal user.

If the script is run as a non-root user, it will display a warning message.

If run as root, it will allow access.



▶️ Usage

- Make the script executable (only needed once):

chmod +x check.sh


- Run as a normal user:

./check.sh


Output:

You must be root to access this file system


Run as root (using sudo):

sudo ./check.sh


Output:

You have access to this file system



📒 Notes

$UID is a special environment variable in Linux that stores the user’s ID.

    0 = root

    1000+ = normal users

Make sure to run the script with sudo if you want root access.