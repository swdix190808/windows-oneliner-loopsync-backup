# windows-oneliner-loopsync-backup
This is a simple loop backup method that allows robocopy (installed on Windows by default) to recursively copy data.
Easily send results to your encrypted containers using Windows alias methods.  No subscriptions or fees. Backup as often as you need, every minute, ten minutes, or once a day (enter number of seconds). Database users may have to have a copy of the database closed due to multi user locking issues and this will not backup your operating system or programs running in memory, only saved data from one location to another, without a need for any network shares (unless you want to).

cmd /C "FOR /L %N IN DO robocopy x:\ y:\ /e >> z:\mybackup_log.txt & timeout 600"
