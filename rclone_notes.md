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
