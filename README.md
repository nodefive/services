# System Services Manager

Interactive Bash CLI tool designed to manage systemd services effortlessly on Linux.

## Features
- **Automatic Root Elevation:** Automatically requests `sudo` privileges if not run as root.
- **Two-Column Interactive Menu:** View services in a clean, space-efficient 2-column numbered list.
- **Quick Actions:** Easily start (`s`), stop (`p`), or restart (`r`) any selected service.
- **Filtering:** Use flags to quickly filter and find failed or stopped services.

## Interface Preview

```text
=================================================
               SYSTEM SERVICES                   
=================================================
         For help type: services -h
=================================================

  1) accounts-daemon.service                         2) apache2.service                              
  3) avahi-daemon.service                            4) bluetooth.service                            
  5) colord.service                                  6) containerd.service                           
  7) cron.service                                    8) cups-browsed.service                         
  9) cups.service                                   10) dbus.service                                 
 11) docker.service                                 12) fwupd.service                                
 13) gdm.service                                    14) libvirtd.service                             
 15) ModemManager.service                           16) NetworkManager.service                       
 17) nordvpnd.service                               18) polkit.service                               
 19) power-profiles-daemon.service                  20) rsyslog.service                              
 21) rtkit-daemon.service                           22) smartmontools.service                        
 23) snapd.service                                  24) ssh.service                                  
 25) switcheroo-control.service                     26) systemd-journald.service                     
 27) systemd-logind.service                         28) systemd-machined.service                     
 29) systemd-oomd.service                           30) systemd-resolved.service                     
 31) systemd-timesyncd.service                      32) systemd-udevd.service                        
 33) thermald.service                               34) udisks2.service                              
 35) unattended-upgrades.service                    36) upower.service                               
 37) user@1000.service                              38) virtlockd.service                            
 39) virtlogd.service                               40) wpa_supplicant.service                       
  q) Quit

Select a service: 
```

## Usage
Run the script to launch the interactive menu:
```bash
chmod +x services
services [FLAG]
```

**Available Flags:**
- `no flag` : Show ALL running services (default)
- `-a` : Show ALL services
- `-f` : Show FAILED services
- `-s` : Show STOPPED (inactive) services

## License

MIT License — Copyright (c) 2025 nodefive

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
