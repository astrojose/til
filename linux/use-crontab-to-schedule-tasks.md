## Use case: use crontab to schedule memory cache and buffer clear
To schedule the task, edit the cron on your linux by using command 
> crotab -e
Then add these lines

>crontab -l

>0 * * *  * sync; echo 3 > /proc/sys/vm/drop_caches
