# Home Assistant Starter Kit — Getting Started

Welcome to **Ad Valorem Labs**. This kit turns your Raspberry Pi into a plug‑and‑play Home Assistant hub.

## What's in the box
- Raspberry Pi 4 (8GB) with case + fan
- 32GB microSD (pre‑flashed with Home Assistant OS)
- Official USB‑C 5V/3A power supply
- Micro‑HDMI → HDMI cable
- Quickstart card (this document)

## First boot (5–10 minutes)
1. Insert the microSD and connect Ethernet (recommended for setup).
2. Plug in the HDMI and power.
3. Wait for Home Assistant to finish first‑boot (the green ACT LED will settle).

## Access the UI
- On the same network, open: **http://homeassistant.local:8123/**
- If `.local` doesn't resolve, find the Pi's IP from your router (e.g., `http://192.168.x.x:8123`)

## Initial setup
1. Create your Home Assistant account.
2. Go to **Settings → System → Backups** and create your first snapshot.
3. Optional: enable **SSH & Web Terminal** add‑on from Add‑on Store.

## Wi‑Fi (optional)
If you need Wi‑Fi instead of Ethernet:
1. Power off the Pi, remove the microSD, insert into a computer.
2. Open the **CONFIG** partition → create `my-network` file (see our repo templates).
3. Reinsert and boot. HA will connect after ~2–3 minutes.

## Zigbee/Z-Wave (optional)
- Add a USB coordinator (e.g., Sonoff ZBDongle‑E). Then install Zigbee2MQTT or ZHA via Add‑on Store.

## Troubleshooting
- Stuck at “Preparing Home Assistant”? Power cycle once. If still stuck, re‑flash the SD from our image.
- Can't reach `.local`? Use the IP address instead.

---
**Docs & files:** https://github.com/advaloremlabs/home-assistant  
**Support / FAQ:** https://github.com/advaloremlabs/docs/faq.md
