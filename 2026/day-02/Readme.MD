# Day 02 or Task-02 — Linux Architecture, Processes, and systemd

## 1. Core Components
- **Kernel:** The core of Linux. It manages CPU, memory, devices, filesystems, and networking, and provides services to programs.
- **User space:** Where shells, commands, libraries, and applications run. Most applications request kernel services through system calls.
- **PID 1 / systemd:** On most modern Linux distributions, `systemd` is the first userspace process (PID 1). It starts and supervises system services and helps bring the system to its configured state.

## 2. How Processes Work
- A **process** is a running instance of a program. Each process has a process ID (**PID**) and may have a parent process (**PPID**).
- A process can be created by an existing process using mechanisms such as `fork()` and then run a program with `exec()`.
- The kernel schedules processes and shares CPU time between runnable tasks. Processes can also request memory, open files, and communicate with other processes.

## 3. Common Process States
- **Running / runnable (`R`):** Executing on a CPU or ready to run.
- **Sleeping (`S` / `D`):** Waiting for an event. `S` is interruptible sleep; `D` is uninterruptible sleep, often while waiting for I/O.
- **Stopped (`T`):** Suspended, for example by a job-control signal.
- **Zombie (`Z`):** The process has exited, but its parent has not yet collected its exit status. A zombie is not actively running; investigate the parent if it persists.

## 4. What systemd Does
- Starts services and other units during boot, manages dependencies, and can restart services according to their configuration.
- Provides `systemctl` to inspect and control services, and commonly works with `journalctl` to read service and system logs.
- Useful checks:
  - `systemctl status nginx` — inspect a service.
  - `systemctl restart nginx` — restart it after checking the impact.
  - `journalctl -u nginx --since today` — view recent service logs.

## 5. Five Commands I Can Use Daily
1. `ps aux` — list processes and inspect CPU/memory usage.
2. `top` — monitor live process and system resource usage.
3. `free -h` — check memory and swap usage.
4. `systemctl status <service>` — check whether a service is healthy.
5. `journalctl -u <service> -n 100 --no-pager` — inspect the latest 100 log lines for a service.

**My troubleshooting habit:** Check service status, read its logs, inspect the process and resource usage, then make a change and verify the result.

