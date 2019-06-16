# Cromwell
## Usage
By default, Cromwell sets the Java temp directory to `$HOME/.tmp`. This memory has much slower read/write speeds than the `$SCRATCH`
directories. This will cause speed problems on any memory intensive programs (I originally encountered this issue with using
`MarkDuplicates` with Cromwell). Setting the Java temp directory to `/tmp` in the cromwell config file with the `temporary-directory`
setting seems to fix the slowdown. See my GATK forums question for more info [here](https://gatkforums.broadinstitute.org/wdl/discussion/23788/cromwell-slow-when-running-markduplicates#latest).

