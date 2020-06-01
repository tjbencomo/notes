# rclone Notes
Only transfer specified files from current directory using the `--files-from` flag with `rclone copy`
```
rclone copy . --files-from bams.txt remote:lee-lab/collagen11-project . -P
```
Show progress with the `-P` flag
