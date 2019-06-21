# rr
Remote Run - a tool to synchronize and run on HPC/Remote servers from your local machine


## Road Map

- Implement `send_to`, which rsyncs the current directory with a remote directory
  - Implement open paramiko through reboots
  - Implement `.rr` config files
  - Implement safe directories that we don't sync
- Implement `run_on`, which runs a command through sbatch or just command line on the remote directory after `send_to`
  - Implement remote and local paths
- Implement `get_from`, which retrieves files after running using rsync from the foreign directory
- Implement `check_progress`, which incrementally checks progress from the remote server
