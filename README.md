# Discord Token Self-XSS

This shows how a Self-XSS vulnerability works in Discord.

## What is Self-XSS?

Self-XSS is when someone tricks you into running a harmful script in your own browser. This script can grab your Discord session token from your browser's storage.

## How I Discovered This

I found that by using a simple script, I could extract my own Discord session token through the Developer Console. This shows how easily someone could be tricked into running a harmful script.

## Low Impact Vulnerability

This Self-XSS vulnerability is considered low impact for a few reasons:

1. **User Interaction Required**: The user must run the script themselves. An attacker cannot use this without tricking the user.

2. **Limited Scope**: The script only accesses the user's own session token, so it does not affect other users.

3. **Easy to Avoid**: Users can protect themselves by not running scripts from unknown sources.

4. **Small Consequences**: If exploited, the worst outcome is that the user’s own token is shown.

## How to Use

1. Open Discord in your web browser.
2. Open the Developer Console (press F12).
3. Copy and paste the code from `selfxss.js` into the console and press Enter.
4. An alert will show your Discord token.

## Warning

Do not run scripts from unknown sources. This can put your account at risk.
