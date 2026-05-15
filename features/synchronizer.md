# Synchronizer Tool

The Synchronizer is a powerful feature that mirrors your actions across multiple browser profiles simultaneously. Instead of manually repeating the same steps in each profile, you perform them once and Dolphin {anty} replicates them everywhere.

## What It Does

When the Synchronizer is active, actions you take in one profile window are mirrored to all other profiles in the group:

- Mouse clicks
- Keyboard input
- Navigation (URL changes)
- Scrolling
- Form interactions

## Use Cases

- **Account farming**: Perform warm-up sequences across dozens of accounts at once
- **Bulk form submission**: Fill and submit forms on multiple accounts simultaneously
- **Social media actions**: Like, comment, or follow using multiple profiles in unison
- **Data entry**: Input the same information across multiple accounts
- **Testing**: Verify how different profiles respond to the same interaction

## How to Use

1. Select the profiles you want to synchronize using checkboxes
2. Click **Synchronizer** in the toolbar or mass actions menu
3. A synchronized session opens — all selected profiles appear in a grid view
4. Perform actions in the **primary window** — they are mirrored to all others
5. Stop the synchronizer when done

## Tips

- Test with 2–3 profiles before scaling to large numbers
- Some platforms may detect identical timing across accounts — consider adding small random delays via the Scenario Builder
- The Synchronizer works alongside proxies — each profile still uses its own proxy and fingerprint
