# Multi-Account Setup for Facebook Ads

This guide walks through setting up multiple Facebook advertising accounts using Dolphin {anty}.

## Prerequisites

- Dolphin {anty} installed and account created
- Residential or mobile proxies (one per Facebook account)
- Valid Facebook accounts or access to account creation workflow

## Why Proxies Matter for Facebook

Facebook's fraud detection correlates IP addresses across accounts. If two accounts share an IP, Facebook may link and ban them. Use **dedicated residential or mobile proxies** — one unique IP per account.

## Step 1: Add Your Proxies

1. Go to **Proxies** in the sidebar
2. Add each proxy with its credentials
3. Click **Check** to verify each one is working
4. Note the country/city for timezone matching

## Step 2: Create Browser Profiles

For each Facebook account, create a separate browser profile:

1. Click **Create Profile**
2. Name it clearly (e.g., "FB - John Smith - US")
3. Select the proxy for this account
4. **Timezone**: set to match the proxy's country
5. **Language**: set to match the proxy's country
6. Leave fingerprint settings at default
7. Click **Save**

## Step 3: Warm Up New Accounts

Before running ads, warm up new accounts to build a natural browsing history:

1. Launch the profile
2. Browse normally: news sites, YouTube, Google searches
3. Log in to Facebook and perform normal social activity (likes, comments, friend requests)
4. Do this for 3–7 days before adding payment methods or running ads
5. Use the **Scenario Builder** or **Synchronizer** to automate warm-up across multiple profiles

## Step 4: Configure Facebook Business Manager

Once warmed up:

1. Log into Facebook from the profile
2. Navigate to Business Manager
3. Add your ad account, payment method, and pixel
4. Keep all Business Manager activity within the same profile

## Step 5: Organize Profiles

Keep your profiles organized as you scale:

- Create folders per **campaign**, **client**, or **geo**
- Use **tags** to mark account health (e.g., "Active", "Banned", "Warming")
- Use **status** labels to show current state to teammates
- Use **notes** to record account details (BM ID, ad spend limits, etc.)

## Running Multiple Accounts with a Team

1. Create a team in **Personal Cabinet → Team**
2. Assign profiles to specific team members
3. Use the **Synchronizer** for bulk warm-up tasks
4. Set permissions so media buyers only see their assigned profiles

## Troubleshooting

**Account getting checkpointed immediately**
- Check proxy quality — use residential, not datacenter
- Ensure timezone matches proxy location
- Increase warm-up time before ad activity

**Profiles linking each other**
- Verify each profile has a unique, dedicated proxy
- Check WebRTC settings — disable or set to proxy IP
- Don't import cookies from one profile into another

**Low ad account limits**
- Spend time warming up the Facebook profile before ads
- Build social proof: profile photo, friends, activity history
