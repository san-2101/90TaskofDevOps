# Day 04 – Linux Practice: Processes and Services

## 1. Process Checks

### Command 1: `ps aux | head -10`
- **Purpose:** Display running processes.
- **Observation:** Checked process IDs, CPU usage, and memory usage.
- **Output:** Recorded from my terminal.

### Command 2: `top -b -n 1 | head -15`
- **Purpose:** Check process and system resource usage.
- **Observation:** Reviewed CPU and memory information.
- **Output:** Recorded from my terminal.

## 2. Service Checks

### Command 3: `systemctl status ssh --no-pager`
- **Purpose:** Inspect the SSH service.
- **Observation:** Recorded the service state and any reported errors.
- **Output:** Recorded from my terminal.

### Command 4: `systemctl is-enabled ssh`
- **Purpose:** Check whether SSH starts automatically at boot.
- **Observation:** Recorded the enabled, disabled, or other returned state.
- **Output:** Recorded from my terminal.

## 3. Log Checks

### Command 5: `sudo journalctl -u ssh -n 20 --no-pager`
- **Purpose:** Inspect recent SSH service logs.
- **Observation:** Checked for startup messages and errors.
- **Output:** Recorded from my terminal.

### Command 6: `sudo journalctl -p warning -n 20 --no-pager`
- **Purpose:** Inspect recent system warnings and more severe messages.
- **Observation:** Reviewed the returned entries for possible issues.
- **Output:** Recorded from my terminal.

## 4. Mini Troubleshooting Steps

1. Check the SSH service status.
2. Inspect service logs if the service is inactive or failing.
3. Identify the reported error before making changes.
4. Apply an appropriate fix only after identifying the cause.
5. Recheck the service status and logs.

## 5. Learning Summary

- Practiced two process-monitoring commands.
- Inspected the SSH service using systemd.
- Reviewed service-specific and system-wide logs.
- Practiced a basic troubleshooting workflow.

**Result:** Complete after running all six commands and recording their actual outputs.
