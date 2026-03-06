# Day 06 – Fixing Touchpad using xinput

Today I learned how to troubleshoot and manage input devices in Linux using the `xinput` command.  
This helped me identify and fix my touchpad issue after installing Linux.

## Listing Input Devices

xinput list

This command lists all connected input devices such as:
- keyboard
- mouse
- touchpad
- stylus

Each device will have a **device ID**.

Example devices:
- AT Translated Set 2 keyboard
- USB Optical Mouse
- ELAN Touchpad / Synaptics Touchpad

## Finding the Touchpad

From the list, identify the **touchpad name and ID**.

Example:

ELAN Touchpad id=12

## Enabling the Touchpad

xinput enable 12

This command enables the device using its ID.

## Disabling the Touchpad

xinput disable 12

This disables the touchpad.

Useful when:
- using an external mouse
- troubleshooting touchpad issues

## Viewing Device Properties

xinput list-props 12

Displays detailed properties of the device such as:
- tapping
- scrolling
- sensitivity

## Checking Hardware Devices

lsusb

Lists all USB devices connected to the system.

## Checking Input Devices from System

cat /proc/bus/input/devices

Displays detailed information about all input hardware.

## Checking Kernel Messages

dmesg | grep -i touchpad

Shows system messages related to the touchpad.

## Summary

Today I learned how to:
- list input devices using `xinput`
- identify device IDs
- enable or disable devices
- inspect device properties
- check hardware and system messages

These commands helped me troubleshoot and fix my touchpad issue.
