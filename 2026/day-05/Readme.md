# Linux Troubleshooting Runbook

**Date:** 13 October 2026  
**Target service:** SSH (`ssh`/`sshd`)  
**Environment:** Ubuntu Linux

## 1. Environment and Filesystem

**Commands:** `uname -a`, `cat /etc/os-release`

**Observation:** Record the kernel version and OS release.

**Filesystem commands:** `mkdir -p /tmp/runbook-demo` and `cp /etc/hosts /tmp/runbook-demo/hosts-copy && ls -l /tmp/runbook-demo`

**Observation:** Confirm that the directory and copied file exist.

```

## 2. Snapshot: CPU and Memory

**Commands:** `ps -eo pid,pcpu,pmem,comm --sort=-pcpu | head` and `free -h`

**Observation:** Record the highest-CPU processes and available memory.


## 3. Snapshot: Disk and I/O

**Commands:** `df -h`, `sudo du -sh /var/log`

**Observation:** Record filesystem usage and the total size of `/var/log`. Note any filesystem with unusually high utilization.

## 4. Snapshot: Network

**Commands:** `sudo ss -tulpn`, `ping -c 4 127.0.0.1 or 8.8.8.8`

**Observation:** Check whether SSH is listening on its expected port and whether local ICMP connectivity succeeds.

## 5. Logs Reviewed

**Commands:** `sudo journalctl -u ssh -n 50 --no-pager`, `sudo tail -n 50 /var/log/auth.log`

**Observation:** Record SSH startup errors, authentication failures, or other relevant messages. Mention if a log file is unavailable.

## 6. Quick Findings

- CPU and memory: [Record findings]
- Disk and I/O: [Record findings]
- Network and SSH listener: [Record findings]
- Logs: [Record errors or state that none were found in the reviewed entries]

## 7. If This Worsens

1. **Validate configuration:** Run `sudo sshd -t` and investigate any reported errors.
2. **Inspect and recover:** Review recent SSH logs, then reload or restart the service only after validating the configuration. Keep an existing SSH session or console access available.
3. **Collect deeper diagnostics:** Check process details and, if necessary, use `strace` on a specific affected process with appropriate permissions.

**Result:** Mark complete after running the commands, recording actual output snippets, and documenting findings.
