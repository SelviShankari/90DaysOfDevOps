-------------------------------Process Checks---------------------------------------------

1.) Checking the snapshot of the running processes 

ps --> this command shows the snapshot of the running processes.

2.)Checking the ngnix related processes

ps aux | grep nginx 
  
----------------------------------Service Checks------------------------------------------------

3.) Checking the status of already installed nginx
 sudo systemctl status nginx :- this is the system controller command and is used to check if the service is running or not.

4.)Checking the list of services running in the server
   systemctl list-units --type=service --> This command is used to list out all the running services in the server.

---------------------------------Logs check-------------------------------------------------------

5.)Checking the system logs for nginx
  journalct -u nginx | tail -5 --> this command is used to view system and service logs on systems that use systemd. It shows what happended on the system and what went wrong.