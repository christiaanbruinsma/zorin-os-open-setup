# Setting Up Appearance Tweaks

This guide explains how to install and apply appearance customizations on Zorin OS.

---

## Installing Fluent Icon Theme

### Step 1: Download the Theme
Download the latest release from the GitHub repository:
[Fluent Icon Theme on GitHub](https://github.com/vinceliuice/Fluent-icon-theme)

### Step 2: Extract the Files
Extract the downloaded archive to your home folder.

### Step 3: Install the Theme
Open a terminal and run:

```
mkdir -p ~/.icons
cp -r Fluent* ~/.icons/
```

### Step 4: Apply the Theme
1. Open **Zorin Appearance** application
2. Go to the **Icons** tab
3. Select **Fluent** from the list
4. The theme will be applied immediately

### Optional: Set as Default
To make Fluent the default icon theme for all users:

```
sudo cp -r ~/.icons/Fluent* /usr/share/icons/
```

---
*Created: 17-08-2026*
*Last updated: 17-08-2026*
