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
   ssh bandit0@bandit.labs.overthewire.org -p 2220
