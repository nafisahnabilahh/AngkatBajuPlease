# AngkatBajuPlease - AngkatBaju Alert Bot (n8n + Telegram)
This is a small automation I built casually using **n8n**.  
As a working wife, there are times when it suddenly rains while I’m still at work  and my husband, who works from home, doesn’t realize it’s raining outside. So I thought… why not automate the reminder? 😄

Now, whenever it rains, he’ll get a Telegram message saying it’s time to *angkat baju* (bring in the laundry)!

## How it works
1. **Schedule Trigger** – runs every hour.  
2. **HTTP Request** – gets the latest weather info from Open-Meteo API.  
3. **IF Node** – checks if `precipitation > 0` (means it's raining).  
4. **Telegram Node** – sends an automated message to my husband’s Telegram.

### Example Flow
