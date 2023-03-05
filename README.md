# Crontab-Scheduler

The Crontab Scheduler option is the lifeline for every DevOps Engineer out there to automate things on a particular time basis or on any other times needed.

-> Here the DevOps Engineer just needs to write their shell-script or jenkins job or any other job and just instruct the crontab editor to execute that in the particular time.

-> If you want to run a job of checking server uptime, server CPU Utilization at some odd times of a day, you now not need to stay till that time and check by manual process. Everything can be automated with the help of Crontab and you can focus on other particular things.

-> The syntax is too simple and it takes just a few minutes for everyone to understand that.
Syntax: (Minute) (Hour) (Date) (Month) (Day of Week) (Command)

Minute: The minute at which the command is to be executed. It takes a value from 0 to 59.

Hour: The hour at which the command is to be executed. It takes a value from 0 to 23.

Date: Date of the month (1-31)

Month: Month of the year (1-12)

Day of the Week: It takes a value from 0 to 6.
0: Sunday
1: Monday 
2: Tuesday
3: Wednesday etc..

Command: Command to be executed

Example: If we want to run our first script in every Sunday at 1:30 AM in every week of every month (as specified earlier)

Then in your server, type: 'crontab -e'

A prompt will open, then enter the following line: 30 1 * * sun /usr/program_name.sh

The above command will run the job at 1:30 AM in every week of every month.
/usr/program_name.sh is the location of the shell-script where program_name.sh is the name yuou assigned to that job.
Also dont forgot to give the required permissions for that job using chmod or else it will not run.
