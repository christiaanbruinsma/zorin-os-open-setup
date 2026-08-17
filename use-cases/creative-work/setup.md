# Creative Work: Setup Instructions

Step-by-step guide to configure your Zorin OS system for creative work.

## Initial Setup

1. **Install Graphics Drivers**
   - For NVIDIA: `sudo ubuntu-drivers autoinstall` then reboot
   - For AMD: Open-source drivers are included by default
   - For Intel: Open-source drivers are included by default

2. **Install Core Creative Applications**
   - Install GIMP for image editing
   - Install Inkscape for vector graphics
   - Install Krita for digital painting
   - Install Kdenlive for video editing
   - Install Audacity for audio production

3. **Set Up Storage**
   - Create dedicated directories for projects: `mkdir ~/Projects/{Graphics,Video,Audio,Ebooks}`
   - Consider using a separate partition for large media files

## Graphic Design & Illustration

### GIMP Configuration
- Set up custom brushes and tool presets
- Configure color management for your monitor profile
- Enable single-window mode for better workflow
- Install plugins: GIMP Plugin Registry (gimp-plugin-registry)

### Inkscape Configuration
- Set default document size to your preferred canvas
- Configure grid and guide settings
- Install additional fonts for design work
- Enable SVG export options

### Krita Configuration
- Import brush packs from Krita Artists community
- Set up custom workspaces for different tasks (painting, illustration, animation)
- Configure tablet/pen pressure sensitivity
- Set up color profiles for print and web

## Video Editing & Production

### Kdenlive Configuration
- Set up project profiles for different resolutions (1080p, 4K, etc.)
- Configure proxy settings for smoother editing with high-res footage
- Import and organize your media library
- Set up keyboard shortcuts for your workflow

### HandBrake Configuration
- Create custom presets for your most-used output formats
- Configure quality settings (RF value for H.264/HEVC)
- Set default output directory
- Enable hardware acceleration if available

## Audio Production

### Audacity Configuration
- Set up your audio device in Preferences
- Configure quality settings (44100Hz, 16-bit for CD quality)
- Install effects plugins (if needed)
- Set up keyboard shortcuts for common actions

## E-Book Reading

### Foliate Configuration
- Set default font and font size for reading comfort
- Configure dark mode for night reading
- Set up library directories
- Enable text-to-speech if needed

## Optimization Tips

- **Graphics Performance**: Enable hardware acceleration in your applications
- **Color Management**: Calibrate your monitor for accurate colors
- **Tablet Support**: Configure pressure sensitivity for drawing tablets
- **Backup**: Regularly back up your creative projects (use Pika Backup)
- **Updates**: Keep all creative applications updated for new features

## Workflow Tips

- **File Organization**: Use a consistent naming scheme for project files
- **Version Control**: Use Git for design files (GIMP, Inkscape have .xcf/.svg formats that work with Git)
- **Cloud Storage**: Sync important files with Nextcloud or similar services
- **Keyboard Shortcuts**: Learn and customize shortcuts for your most-used tools

## Troubleshooting

- If graphics performance is slow: Check if hardware acceleration is enabled
- If tablet isn't working: Install proper drivers and check pressure sensitivity settings
- If colors look wrong: Calibrate your monitor or check color profile settings
- If video playback is choppy: Enable proxy editing in Kdenlive or reduce preview quality

## Hardware Recommendations

- **Graphics Tablet**: Wacom, Huion, or XP-Pen for digital painting
- **Monitor**: Color-accurate display with at least 95% sRGB coverage
- **Storage**: Fast SSD for active projects, HDD for archive
- **Memory**: 16GB+ RAM for video editing and large graphic files