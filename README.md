# System-Info-Script

# Bash Script for showing System Information
#!/bin/bash

# Welcome the user
echo "Welcome to System Information Script"
echo "-----------------------------------"
echo

# Show the date and time
echo "Current Date and Time:"
date
echo

# Show uptime and last logins
echo "System Uptime:"
uptime
echo

echo "Last Logins:"
last
echo

# Show disk space
echo "Disk Space:"
df -h
echo

# Show RAM and processor information
echo "RAM and Processor Information:"
free -h
echo

# Show top CPU processes
echo "Top CPU Processes:"
top -b -n 1 | head -n 10
echo

# End of script


# Python Script for Showing System Information
#!/usr/bin/env python3
import os
import platform
import subprocess

def welcome_user():
    print("Welcome to System Information Script")
    print("-----------------------------------")

def show_date_time():
    print("\nCurrent Date and Time:")
    os.system("date")

def show_system_uptime():
    print("\nSystem Uptime:")
    os.system("uptime")

def show_last_logins():
    print("\nLast Logins:")
    os.system("last")

def show_disk_space():
    print("\nDisk Space:")
    os.system("df -h")

def show_ram_processor_info():
    print("\nRAM and Processor Information:")
    os.system("free -h")

def show_top_cpu_processes():
    print("\nTop CPU Processes:")
    os.system("top -b -n 1 | head -n 10")

def main():
    welcome_user()
    show_date_time()
    show_system_uptime()
    show_last_logins()
    show_disk_space()
    show_ram_processor_info()
    show_top_cpu_processes()

if __name__ == "__main__":
    main()
