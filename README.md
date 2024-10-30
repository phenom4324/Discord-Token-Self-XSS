# Discord Token Self-XSS

This shows how a Self-XSS vulnerability works in Discord.

## What is Self-XSS?

Self-XSS is when someone tricks you into running harmful code in your own browser. This code can steal your Discord session token from your browser. If an attacker gets you to copy and paste their code, they can take over your account.

Be careful when screen sharing. If someone trying to steal your token is recording while you’re sharing your screen, and you accidentally show your token, they can capture it right then. This means your token could be stolen without you knowing, just from a video you shared.

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
