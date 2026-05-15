# Team Workflow Setup

How to structure your team for efficient, secure multi-account operations using Dolphin {anty}.

## Planning Your Team Structure

Before adding users, define:

1. **Who manages what** — which team members work with which accounts/clients
2. **What each person can do** — permissions per role
3. **How profiles are organized** — folder structure for easy sharing

## Recommended Folder Structure

```
All Profiles
├── Client A
│   ├── Facebook Accounts
│   ├── Google Accounts
│   └── Archived
├── Client B
│   └── ...
├── Internal
│   ├── Testing
│   └── Tools
└── Shared
    └── Warm-up Queue
```

## Step-by-Step Team Setup

### 1. Create the Folder Structure

1. Right-click in the sidebar → **New Folder**
2. Create folders for each client or campaign
3. Move existing profiles into appropriate folders

### 2. Add Team Members

1. Go to **Personal Cabinet → Team**
2. Click **Add User**, enter email
3. Repeat for all team members

### 3. Assign Permissions

For each team member, configure what they can access:

| Role | Typical Permissions |
|------|---------------------|
| Account Manager | View + start/stop + edit profiles in their folders |
| Media Buyer | Start/stop + run scripts, no profile editing |
| Team Lead | Full access to all folders |
| Viewer | View only (for monitoring/reporting) |

### 4. Share Folders

1. Right-click a folder → **Share permissions**
2. Select the team member
3. Set their permission level for this folder
4. Click **Save**

Repeat for each client folder — assign only the relevant people.

### 5. Assign Profiles to Members

For individual profile ownership:
1. Select profile(s)
2. Use **Transfer** to move them to a specific team member
3. Transferred profiles appear in the member's workspace

## Proxy Management in Teams

- Store all team proxies in the **shared proxy library**
- Set proxy visibility per user if needed
- Never give individual team members direct access to proxy credentials — let them use proxies through Dolphin {anty} only

## Communication via Profile Notes

Use profile **Notes** and **Status** fields as lightweight communication:

- **Status**: "Farming" / "Ready to Run" / "Issue" / "Banned"
- **Notes**: Account details, last action, special instructions

## Scaling Your Team

As you grow, consider:

- **Upgrading your plan** to support more profiles and users
- **Creating sub-team leads** who manage their own folder sets
- **Using the API** to automate profile creation and assignment at scale
- **Batch operations** via mass actions for team-wide updates

## Security Best Practices

- Give minimum required permissions — don't make everyone an admin
- Regularly audit which team members have access to which folders
- When a team member leaves, immediately remove their user account
- Use dedicated proxies so individual team members can't access proxy credentials directly
