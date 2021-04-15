# Fiverr - Always Online

I often found that Fiverr would change my status to offline, despite me still having the Fiverr browser tab open. I learnt that it only pings the online API if you're active on the browser tab.

After testing, it seems if it doesn't ping the server within a couple of minutes, it sets your online status to offline.

This script pings the server every 2 minutes, to keep your online status.

You can run this as a background task on your MAC/PC. If using Windows, you can set it up to run when you turn on your PC,

# Setup

To use this script, you need to find your entity_id. To do this, login to Fiverr on Chrome or Firefox, and go to your profile. Open up developer tools, and look out for a post request to "Online". Here you will find your entity_id. Copy that, and inside main.py replace XXXX with your entity_id.

Run the script, and it will now keep your status set to online.