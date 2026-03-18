=====================================================
ISP OS LICENSE SYSTEM - QUICK GUIDE
=====================================================

SECRET KEY (DO NOT SHARE!):
ac794b1ccc6e9664e01e7a973f007ad23f07c7f0fd3b60e0ba3f978af3f748d3

This key is in:
- services/licenseService.js (device side)
- tools/license-generator.html (vendor side)

=====================================================
HOW TO GENERATE LICENSE FOR CUSTOMER:
=====================================================

1. Customer sends you their HARDWARE ID
   (They copy it from: http://device-ip/license page)

2. Open license-generator.html in your browser
   - Just double-click the file, opens in Chrome/Firefox
   - OR host on GitHub Pages for access anywhere

3. Enter:
   - Hardware ID (paste what customer sent)
   - Customer Name (e.g., "Juan's Cafe")
   - Tier (Enterprise/Pro/Basic)

4. Click GENERATE

5. Copy the code and send to customer
   (via SMS, Messenger, email, etc.)

6. Customer pastes code in ISP OS license page
   → ACTIVATES INSTANTLY (no internet needed!)

=====================================================
ONLINE VALIDATION (OPTIONAL):
=====================================================

When device goes online, it checks GitHub for:
- Revoked licenses (you can block bad customers)
- Duplicate usage (same license on 2 devices)

To enable online validation:
1. Create licenses.json in your GitHub repo
2. Set GitHub token on device

But OFFLINE activation works without this!

=====================================================
FILES:
=====================================================

license-generator.html  - Open this to generate codes
LICENSE-README.txt      - This file

=====================================================
