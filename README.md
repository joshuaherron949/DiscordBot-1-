[README.md](https://github.com/user-attachments/files/23138283/README.md)
# Discord Role Ping Bot

A Discord bot that monitors a specific channel and pings a designated role whenever anyone posts a message.

## Features
- Monitors a specific Discord channel
- Automatically pings a role when messages are posted
- 5-second cooldown to prevent spam
- Robust error handling and auto-reconnection

## Requirements
- Node.js 18 or higher
- Discord bot token
- Channel ID to monitor
- Role ID to ping

## Environment Variables
Set these in your hosting platform:

- `TOKEN` - Your Discord bot token
- `CHANNEL_ID` - The channel ID to monitor (e.g., 1431154474638114961)
- `ROLE_ID` - The role ID to ping (e.g., 1431154632616316968)

## Discord Bot Setup Requirements

### In Discord Developer Portal:
1. Go to https://discord.com/developers/applications
2. Select your bot application
3. Go to the **Bot** section:
   - Enable **Message Content Intent** (required)
   - Disable **Public Bot** (to keep it private)
4. Go to **OAuth2** → **General**:
   - Set **Authorization Method** to "None" (prevents others from inviting)

### In Your Discord Server:
1. Right-click the role you want to ping
2. Edit Role → Enable **Allow anyone to @mention this role**
3. Save changes

## Local Installation
```bash
npm install
node index.js
```

## Deployment on Railway.app (Free 24/7 Hosting)

Railway provides $5 free credits monthly - perfect for this bot!

### Quick Deploy Steps:

1. **Create GitHub Repository** (if you haven't already)
   - Go to GitHub and create a new repository
   - Push this code to GitHub

2. **Deploy to Railway**
   - Go to https://railway.app
   - Click "Start a New Project"
   - Choose "Deploy from GitHub repo"
   - Select your repository
   - Railway will auto-detect Node.js and deploy

3. **Add Environment Variables**
   - In Railway dashboard, go to your project
   - Click "Variables" tab
   - Add these variables:
     - `TOKEN` = your Discord bot token
     - `CHANNEL_ID` = 1431154474638114961
     - `ROLE_ID` = 1431154632616316968

4. **Deploy!**
   - Railway will automatically start your bot
   - Check the logs to confirm it's running
   - Your bot is now live 24/7!

## License
ISC
