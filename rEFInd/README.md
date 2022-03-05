# My Experience with rEFInd Installation

The documentation of rEFInd only brings you to a point and if the setup you end up with following some tutorials don't work, well good luck. Here are some issues that I encountered and how I fixed them.

- The directories don't match. Whatever FS rEFInd internally uses uses *case sensitive* directories. Each letter must exactly match the case of the actual directory. Otherwise you will bump your head in the wall pondering why rEFInd loops back to main menu when you enter your manual boot entry.
- boot in separate partition. If you read through the Arch Wiki carefully you can notice this but if boot is a separate partition for you, you should write any paths in boot relative to /boot e. g. /vmlinuz-linux instead of `/boot/vmlinuz-linux`

Also as of 4th of March, 2022. I am still dealing with Windows 11 looping back to the main menu. If you can figure out my problem please create an issue or a pull request. Help is really, really appreciated.
