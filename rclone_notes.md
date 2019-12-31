# rclone Notes
Only transfer files from list using the `--from-files` flag with `rclone copy`
```
rclone copy --files-from bams.txt remote:lee-lab/collagen11-project . -P
```
Show progress with the `-P` flag
