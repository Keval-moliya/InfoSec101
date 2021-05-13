# Bandit Level 8 to 9 Writeup


Author: [Keval Moliya](https://github.com/Keval-moliya)

Problem Page: [bandit14](https://overthewire.org/wargames/bandit/bandit15.html)

## List of Commands Used
```
ls - list files in a directory
sshpass - noninteractive ssh password provider
ssh - OpenSSH remote login client
telnet - The telnet command is used for interactive communication with another host using the TELNET protocol

```

## Walkthrough
 We need to connect to the localhost through port 30000, so we can use telnet to do that and then submitting the password of the current level we get the password for next level.

## Password
`4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e`

## Bash/Python script to automate the process
```
ssh bandit14@bandit.labs.overthewire.org -p 2220
4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e

telnet localhost 30000
4wcYUJFw0k0XLShlDzztnTBHiqxU3b3e
```