creating a VHDX backup of windows computers
Source: https://www.youtube.com/watch?v=mzhEV7vAMlo





transferring the file over to the server:
scp /path/to/file.vhdx nameserver@ipaddress:/sharename

note: cannot use tkye samba setup (adding user to non-login shell) for scp
