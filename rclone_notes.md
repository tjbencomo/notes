# rclone Notes
Only transfer specified files from current directory using the `--files-from` flag with `rclone copy`
```
rclone copy . --files-from bams.txt remote:path/dest . -P
```
Show progress with the `-P` flag

Using `-P` is nice for interactive mode but clogs up the log files when running from the queue.
When submitting the job to Sherlock, it's better to print out the stats every 30 minutes.
```
rclone copy . --files-from files remote:path/dest --stats-one-line --stats 30m
```

## Remote Setup
When creating a new remote, you need to authorize `rclone` account access. The default config setup
will try to open a browser link that will lead you to authorize `rclone` access. This won't work if the computer
doesn't have a monitor/GUI output (ie Sherlock or other SSH scenarios). In this case don't use the default config.
Instead, download `rclone` onto a compute with GUI output (like your laptop) and then follow the instructions to
authorize from the local computer and then paste the key into the remote computer.
