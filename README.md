# M5Paper Clock - PlatformIO Version v2.1

## Quick Start

1. **Install PlatformIO**:
   - Install VS Code
   - Install PlatformIO IDE extension

2. **Open Project**:
   - Open this folder in VS Code
   - PlatformIO will auto-detect `platformio.ini`

3. **Prepare SD Card**:
   - Format microSD card as FAT32
   - Copy `settings.txt` to SD card root
   - Edit `settings.txt` with your WiFi credentials and timezone

4. **Upload**:
   - Connect M5Paper via USB
   - Click "Upload" button in PlatformIO toolbar
   - Or run: `pio run -t upload`

5. **Monitor**:
   - Open Serial Monitor at 115200 baud
   - Verify settings loaded successfully

## Settings File Format

Edit `settings.txt` on SD card:

```
TIMEZONE=-7
WIFI_SSID=YourNetworkName
WIFI_PASSWORD=YourPassword
NTP_SERVER=time.cloudflare.com
```

## Requirements

- PlatformIO Core
- M5Paper hardware
- MicroSD card (FAT32)
- 2.4GHz WiFi network

## Build

```bash
pio run
```

## Upload

```bash
pio run -t upload
```

## Serial Monitor

```bash
pio device monitor
```

See main README.md for detailed documentation.
