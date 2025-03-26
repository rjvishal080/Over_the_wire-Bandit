Over the Wire : Bandit Level 0 - 20 Write up  
# Bandit Write-Up (Levels 0 - 20)

This repository contains my write-up for the Bandit CTF (Capture The Flag) challenge series. Each markdown file covers one level, with explanations, commands, and methods used to solve the challenges.

# Bandit Level 0 -> Level 1

## Challenge

The goal of this level is to log into the Bandit game using SSH. The host to connect to is `bandit.labs.overthewire.org` on port `2220`. The username is `bandit0`, and the password is `bandit0`.

### Steps to Complete

1. **Connect to the Bandit server using SSH**:


   Open your terminal and run the following command to SSH into the server:
   


   ```bash
   ssh bandit0@bandit.labs.overthewire.org -p 2220 Images/Screenshot (2).png
   
Password: bandit0
# Bandit Level 0-1 Solution

## Problem Description:
In this level, your task is to find the password for the **Bandit1** account. The password for the next level is stored in a file called `readme` located in the home directory of **Bandit0**.

## Solution:

1. **SSH into Bandit0**:
   First, log in to the server with the following SSH command:

   ```bash
   ssh bandit0@bandit.labs.overthewire.org -p 2220
   ls
   cat readme
Password : 
## Bandit Level 1-2 Solution

## Problem Description:
In this level, your task is to find the password for **Bandit2**. The password is stored in a file in the home directory, but the file's name starts with a hyphen (`-`).

## Solution:

1. **SSH into Bandit1**:
   First, log in to the **Bandit1** account:

   ```bash
   ssh bandit1@bandit.labs.overthewire.org -p 2220
   ls
   cat -- -file
Password : 
# Bandit Level 2-3 Solution

## Problem Description:
In this level, your task is to find the password for **Bandit3**. The password is stored in a file called `spaces in this filename` in the home directory.

## Solution:

1. **SSH into Bandit2**:
   Log in to **Bandit2** using the password found in **Bandit Level 2**:

   ```bash
   ssh bandit2@bandit.labs.overthewire.org -p 2220
   ls
   cat spaces\ in\ this\ filename
   or
   cat "spaces in this filename"
Password : 
# Bandit Level 3-4 Solution

## Problem Description:
In this level, your task is to find the password for the **Bandit4** account. The password for the next level is stored in a hidden file in the `inhere` directory, which is located in the current working directory.

## Solution:

1. **SSH into Bandit3**:
   First, log in to the server using the password you found in the previous level (Bandit2). Use the following SSH command:

   ```bash
   ssh bandit3@bandit.labs.overthewire.org -p 2220
   cd inhere
   ls -a
   cat .hidden
Bandit Level 4 → Level 5: Identifying a Human-Readable File
Problem Description:
In this level, you are tasked with finding the password for Bandit5. The password is stored in one of the files in the inhere directory, and your goal is to identify the human-readable file among them.

Solution Steps:
Navigate to the inhere directory: Start by changing to the inhere directory where the files are located.

bash
Copy
cd inhere
Identify the Readable File: The file command helps you identify the type of each file in the directory. Use it to check all files:

bash
Copy
file ./*
This will output the type of each file. You are looking for a file that is labeled as ASCII text, as that will be the human-readable file containing the password.

Read the Correct File: Once you have identified the file that is labeled as ASCII text, use the cat command to display its contents:

bash
Copy
cat ./-file07
Replace ./-file07 with the actual filename of the readable file if it's different. The content of the file will contain the password for Bandit5.

Login to Bandit5: After obtaining the password, you can log into Bandit5 with the following command:

bash
Copy
ssh bandit5@bandit.labs.overthewire.org -p 2220
Enter the password you retrieved from the readable file when prompted.
   



   











