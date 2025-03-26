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





