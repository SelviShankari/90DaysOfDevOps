1.) Checking the health-dashboard for CPU-Memory-Disk

htop :- This command shows the active usage of CPU, Memory, Disk Utilization.

2.) Checking the status of ssh service

sudo systemctl status ssh :- This command returns the stauts of the process whether it is running, stopped etc etc 

3.)Checking the latest logs for that service

cd var/logs/ngninx/ :- This commands navigates us to the destination where the logs gets saved.
 
You may find two files present inside it access.logs and error.log

4.) Viewing the contents of access.logs

cat access.logs :- this command is used to view the content of the access.logs

cat error.logs :- this command is used to view the content of error.logs



