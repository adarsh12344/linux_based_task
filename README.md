# **sysopctl**

`sysopctl` is a custom system management utility designed to streamline the administration of Linux systems. With a simple command-line interface, it provides essential tools for managing services, monitoring system health, and performing backup operations.

---

## **Features**

### **General Commands**
- `--help`: Displays a detailed usage guide.
- `--version`: Outputs the version of the `sysopctl` utility.

### **Service Management**
- `service list`: Lists all active services (equivalent to `systemctl list-units --type=service`).
- `service start <service-name>`: Starts the specified service.
- `service stop <service-name>`: Stops the specified service.

### **System Health**
- `system load`: Displays system load averages (equivalent to `uptime`).
- `disk usage`: Shows disk usage statistics for all partitions (equivalent to `df -h`).

### **Advanced Operations**
- `process monitor`: Displays real-time process activity (equivalent to `top`).
- `logs analyze`: Summarizes recent critical log entries (uses `journalctl`).
- `backup <path>`: Creates a backup of the specified directory using `rsync`.

---

## **Installation**

1. Clone the repository:
   ```bash
   git clone <your-private-repo-url>
   cd sysopctl
   ```

2. Make the script executable:
   ```bash
   chmod +x sysopctl.sh
   ```

3. (Optional) Add `sysopctl` to your `PATH`:
   ```bash
   sudo mv sysopctl.sh /usr/local/bin/sysopctl
   ```

4. Verify installation:
   ```bash
   sysopctl --version
   ```

---

## **Usage Examples**

### Help and Version
```bash
sysopctl --help
sysopctl --version
```

### Service Management
```bash
sysopctl service list
sysopctl service start nginx
sysopctl service stop apache2
```

### System Health
```bash
sysopctl system load
sysopctl disk usage
```

### Advanced Operations
```bash
sysopctl process monitor
sysopctl logs analyze
sysopctl backup /home/user/documents
```

---

## **System Requirements**

- Linux operating system.
- Admin privileges (for managing services and logs).
- Tools required:
  - `systemctl`
  - `uptime`
  - `df`
  - `top`
  - `journalctl`
  - `rsync`

---





