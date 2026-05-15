# Proxy Management

Each browser profile in Dolphin {anty} can be assigned a unique proxy, ensuring that accounts appear to come from different IP addresses and locations.

## Supported Proxy Types

- **HTTP / HTTPS**
- **SOCKS4**
- **SOCKS5**

## Adding a Proxy

### Method 1: From the Proxies Section

1. Go to **Proxies** in the left sidebar
2. Click **New Proxy**
3. Enter proxy details:
   - Type (HTTP/SOCKS4/SOCKS5)
   - Host (IP address or domain)
   - Port
   - Username and password (if required)
4. Click **Check** to verify the proxy works
5. Click **Save**

### Method 2: During Profile Creation

1. When creating or editing a profile, click the **Proxy** field
2. Select **New Proxy** or choose a saved proxy
3. Enter the proxy credentials inline

## Proxy Format

You can paste proxies in bulk using standard formats:

```
# host:port
192.168.1.1:8080

# host:port:user:pass
192.168.1.1:8080:username:password

# type://host:port
socks5://192.168.1.1:1080

# type://user:pass@host:port
socks5://username:password@192.168.1.1:1080
```

## Checking Proxy Status

Click **Check** next to any proxy to verify it is working. Dolphin {anty} will display:
- Connection status (active/failed)
- Detected IP address
- Country and city

## Assigning Proxies to Profiles

Each profile can have one proxy assigned. To assign or change a profile's proxy:

1. Open the profile settings
2. Click the **Proxy** field
3. Select from your saved proxy list or add a new one

## Recommendations

- **Match timezone to proxy location** — your browser timezone should match the proxy's country to avoid detection
- **Use dedicated proxies** — shared proxies increase the risk of IP reputation issues
- **Residential or mobile proxies** have higher trust scores than datacenter proxies on platforms like Facebook

## Sharing Proxies in Teams

On Base plan and above, proxies can be shared with team members. Go to the proxy settings and configure access permissions for each team member.
