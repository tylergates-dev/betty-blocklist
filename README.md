# betty-blocklist

A custom uBlock Origin filter list that blocks US home buying, real estate listing, and mortgage websites. Network-independent — enforced at the browser level regardless of what Wi-Fi or network the device is on.

## Covered Categories

- Real estate listing platforms (Zillow, Redfin, Realtor.com, Trulia, etc.)
- National real estate brokerages (Coldwell Banker, RE/MAX, Keller Williams, Compass, etc.)
- New construction and foreclosure sites
- Mortgage lenders and rate comparison tools

## Installation

1. Open your browser and click the uBlock Origin icon
2. Go to the **Dashboard** (the sliders icon)
3. Click the **Filter lists** tab
4. Scroll to the bottom and click **Import...**
5. Paste the following URL:

```
https://raw.githubusercontent.com/tylergates-dev/betty-blocklist/main/homebuying-blocklist.txt
```

6. Click **Apply changes**

uBlock Origin will now block all sites on the list and will automatically check for updates approximately every 5 days. To force an immediate update, return to Filter lists and click the refresh icon next to the list name.

## Updating the List

To add or remove a domain, edit `homebuying-blocklist.txt` directly on GitHub and increment the `! Version:` number in the file header. uBlock Origin will pick up the change on its next scheduled refresh or on a manual refresh.

## Pi-hole Integration

The domains in this list can also be added to a Pi-hole instance for network-level blocking independent of the browser. This covers all browsers, apps, and devices on the network simultaneously. See Pi-hole documentation for importing a custom blocklist via the Group Management interface.
