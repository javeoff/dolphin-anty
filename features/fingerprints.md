# Fingerprint Management

A browser fingerprint is a collection of technical attributes websites use to identify and track users. Dolphin {anty} lets you customize these attributes per profile so each profile looks like a unique, real device.

## What is a Browser Fingerprint?

When you visit a website, your browser reveals information like:
- Operating system and version
- Screen resolution and color depth
- Installed fonts and plugins
- Canvas and WebGL rendering signatures
- Time zone and language settings
- Hardware concurrency (CPU threads)
- Memory (device RAM)
- WebRTC IP addresses

Antidetect browsers replace these values with controlled, realistic alternatives.

## Default Fingerprints

When creating a new profile, Dolphin {anty} automatically assigns a fingerprint based on real device data. **The default settings are optimal** — they are selected by the development team to maximize authenticity.

> Recommendation: Use default fingerprint settings unless you have a specific reason to customize.

## Customizable Parameters

Dolphin {anty} allows you to customize 20+ fingerprint parameters:

### Browser & OS
- **User Agent** — browser type, version, and OS string
- **Platform** — reported operating system
- **Screen Resolution** — width × height
- **Color Depth** — typically 24-bit
- **Device Pixel Ratio** — for HiDPI display simulation

### Graphics
- **WebGL Vendor & Renderer** — GPU identification string
- **WebGPU** — newer graphics API fingerprint
- **Canvas** — 2D canvas rendering noise

### Hardware
- **CPU Cores** — reported `navigator.hardwareConcurrency`
- **RAM** — reported `navigator.deviceMemory`

### Media & Devices
- **Webcam Spoofing** — replace real camera data with spoofed identifiers
- **Microphone** — audio device identifiers
- **Audio Context** — audio processing fingerprint

### Network
- **WebRTC** — control IP leakage through WebRTC (disable, use real IP, or spoof)
- **Timezone** — match to your proxy location
- **Language** — browser language setting
- **Geolocation** — GPS coordinates (can be spoofed or disabled)

### Fonts & Plugins
- **Font List** — which fonts are reported as installed
- **Plugins** — browser plugin list

## Fingerprint Authenticity

Dolphin {anty} uses fingerprints extracted from real devices. Each profile gets a fingerprint configuration that browsers and anti-fraud systems recognize as a genuine user device.

## ClientHints

Dolphin {anty} supports modern **User-Agent Client Hints** (UA-CH), the newer fingerprinting method used by Chromium-based browsers. These are automatically handled to stay consistent with the User Agent string.

## Checking Your Fingerprint

You can verify your profile's fingerprint integrity using services like:
- [BrowserScan](https://browserscan.net/)
- [CreepJS](https://abrahamjuliot.github.io/creepjs/)
- [Browserleaks](https://browserleaks.com/)
- [Pixelscan](https://pixelscan.net/)
