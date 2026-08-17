# System & Maintenance: Setup Instructions

Step-by-step guide to configure your Zorin OS system for system administration and maintenance. *This section may contain technical content.*

## Initial Setup

1. **Install System Tools**
   - Open Terminal
   - Install system monitoring tools: `sudo apt install gnome-system-monitor htop nmon`
   - Install disk utilities: `sudo apt install gparted testdisk`

2. **Enable GNOME Tweaks**
   - If not already installed: `sudo apt install gnome-tweaks`
   - Open GNOME Tweaks and explore customization options

3. **Set Up Terminal**
   - Install preferred shell (zsh, fish): `sudo apt install zsh fish`
   - Install terminal utilities: `sudo apt install tmux tree htop`

## System Customization

### GNOME Tweaks Configuration
- **Appearance**: Change themes, icons, and cursors
- **Extensions**: Enable/disable GNOME Shell extensions
- **Window Management**: Configure window behavior and focus
- **Workspaces**: Set up static or dynamic workspaces
- **Top Bar**: Show/hide date, battery, and other indicators

### Terminal Configuration
- Create custom profiles for different tasks
- Set up keyboard shortcuts for frequently used commands
- Configure tab behavior and appearance
- Install and configure Oh My Zsh for enhanced shell experience

## System Monitoring

### Logs Viewer
- Open Logs application from Activities Overview
- Filter by time period or category
- Monitor systemd journal for errors and warnings
- Set up alerts for critical events

### Mission Center
- Monitor CPU, memory, disk, and network usage
- Set up resource usage alerts
- View process list and manage running applications
- Check system temperature and power consumption

## Storage Management

### Disks Utility
- View and manage disks and partitions
- Create, delete, and resize partitions
- Format drives with different filesystem types
- Set up automatic mount options
- Check SMART status for HDD/SSD health

### Disk Usage Analyzer
- Scan your system for disk usage
- Identify large files and directories
- Clean up unnecessary files
- Set up regular usage scans

## Security Configuration

### Firewall (gufw)
- Open gufw from Activities Overview
- Enable the firewall
- Set default policies (Incoming: Deny, Outgoing: Allow)
- Add rules for specific applications if needed
- Regularly review firewall logs

### Password Management
- **Passwords and Keys (Seahorse)**:
  - Create a login keyring for storing passwords
  - Import existing passwords from other managers
  - Set up SSH keys for remote access
  - Backup your keyring regularly

- **Proton Pass**:
  - Create an account and set up master password
  - Import existing passwords
  - Enable 2FA for added security
  - Set up emergency access for trusted contacts

## Backup Strategy

1. **Pika Backup Setup**
   - Open Pika Backup
   - Create a new backup repository
   - Select folders to back up (Documents, Pictures, etc.)
   - Set up automatic backup schedule (daily/weekly)
   - Choose backup destination (external drive, network location)

2. **Manual Backups**
   - Use File Roller to create archive backups
   - Compress important directories: `tar -czvf backup-$(date +%Y%m%d).tar.gz ~/Documents`
   - Store backups in multiple locations

## Maintenance Tasks

### Regular Maintenance
- Run system updates weekly: `sudo apt update && sudo apt upgrade`
- Clean package cache: `sudo apt clean`
- Remove unused packages: `sudo apt autoremove`
- Check for broken packages: `sudo apt --fix-broken install`

### Performance Optimization
- Use Disk Usage Analyzer to free up space
- Disable unnecessary startup applications
- Use Mission Center to identify resource-heavy processes
- Consider upgrading RAM if system is slow

### Hardware Checks
- Monitor disk health with Disks utility
- Test memory with memtest86+
- Check CPU temperatures with sensors command
- Test webcam with Camera application

## Troubleshooting

- If system is slow: Check Mission Center for resource usage
- If disk is full: Use Disk Usage Analyzer to find large files
- If firewall blocks application: Add exception in gufw
- If password not saved: Check Passwords and Keys (Seahorse) settings
- If terminal commands not found: Check if package is installed and PATH is correct

## Advanced Configuration

- **Custom Scripts**: Create bash scripts for repetitive tasks
- **Cron Jobs**: Set up automated maintenance with `crontab -e`
- **Systemd Services**: Create custom services for background tasks
- **Logging**: Configure rsyslog for advanced logging needs