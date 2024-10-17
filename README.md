# Discord Token Self-XSS

I created this project to show how a Self-XSS vulnerability works in Discord.

## What is Self-XSS?

Self-XSS is when someone tricks you into running a harmful script in your own browser. This script can grab your Discord session token from your browser's storage.

## How I Discovered This

I found that by using a simple script, I could extract my own Discord session token through the Developer Console. This demonstrates how easily someone could be tricked into running a harmful script.

## How to Use

1. Open Discord in your web browser.
2. Open the Developer Console (press F12).
3. Copy and paste the code from `selfxss.js` into the console and press Enter.
4. An alert will show your Discord token.

## Warning

Do not run scripts from unknown sources. This can put your account at risk.
