# Using Proxies Effectively

A guide to choosing, configuring, and managing proxies in Dolphin {anty} for the best results.

## Proxy Types Explained

| Type | Trust Level | Speed | Best For |
|------|-------------|-------|----------|
| Residential | High | Medium | Social media, ad platforms |
| Mobile (4G/5G) | Highest | Varies | Facebook, Instagram, TikTok |
| Datacenter | Low | Fast | Scraping, low-risk tasks |
| ISP (Static Residential) | High | Fast | Long-term accounts |

**Recommendation**: Use residential or mobile proxies for any platforms that actively monitor account behavior (Facebook, Google, Amazon). Datacenter proxies work well for web scraping and less-sensitive tasks.

## One Proxy Per Account

The golden rule: **never share a proxy between two accounts on the same platform**.

If Platform X sees accounts A and B connecting from the same IP at different times, it may link them. If one gets banned, the other is at risk.

## Proxy Format Reference

Dolphin {anty} accepts these formats:

```
# Basic
host:port

# With authentication
host:port:username:password

# With protocol
socks5://host:port
http://host:port

# Full format
socks5://username:password@host:port
```

## Matching Timezone and Language

When a profile uses a US proxy but reports a timezone of "Europe/Moscow", platforms may flag the inconsistency.

Always match:
1. **Proxy country** → **Profile Timezone**
2. **Proxy country** → **Profile Language** (browser language setting)
3. **Proxy country** → **Geolocation** (if using geolocation spoofing)

## Checking Proxy Quality

After adding a proxy, click **Check** in Dolphin {anty} to see:
- IP address
- Location (country, city)
- Connection status

For deeper analysis, launch a profile with the proxy and visit:
- [BrowserLeaks IP Test](https://browserleaks.com/ip)
- [IPInfo](https://ipinfo.io/)

Check for **DNS leaks** and **WebRTC leaks** that might reveal your real IP.

## WebRTC Settings

WebRTC can leak your real IP even when using a proxy. Configure WebRTC in profile fingerprint settings:

- **Disabled** — safest, but some sites require WebRTC
- **Real IP** — uses actual IP (don't use with proxies for sensitive accounts)
- **Fake IP** — spoofs to proxy IP (recommended)

## Bulk Proxy Import

To add many proxies at once:

1. Go to **Proxies → Import**
2. Paste all proxies in one of the accepted formats (one per line)
3. Specify the type if not included in the format
4. Click **Import**

## Proxy Rotation (Advanced)

For scraping or tasks that don't require persistent identity, you can:

1. Create a proxy rotation endpoint (e.g., using a rotating proxy provider)
2. Set the rotating endpoint as the proxy for multiple profiles
3. Each profile request goes through a different IP

Note: Don't use rotating proxies for accounts that need consistent identity (social media, ad platforms).

## Recommended Proxy Providers

Dolphin {anty} works with any proxy provider. Look for providers offering:
- Residential or mobile IPs
- Country/city targeting
- High uptime SLA
- SOCKS5 support
