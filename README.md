# PITCH TALK BOT

**AIRDROP** : PitchTalk Support By Near

**Reward** : PITCH

**Register** : [Here](https://t.me/pitchtalk_bot/app?startapp=334a84)
- Complete Task
- Farm Daily
- Done

**Listed On Q1 & Not Tap Tap Project!**

## PREREQUISITE

- Git
- Node JS
- TELEGRAM_APP_ID & TELEGRAM_APP_HASH Get it from [Here](https://my.telegram.org/auth?to=apps) (REQUIRED IF YOU WANT USE SESSIONS).

## BOT FEATURE

- Multi Account With Proxy Support
- Support Telegram Sessions and Telegram Query (Query May Expired)
- Auto Complete Some Misisons
- Auto Start Farming
- Auto Claim Farming
- Auto Claim Referal Reward

## SETUP & CONFIGURE BOT

### LINUX & MAC OS

1. Clone project repository
   ```
   git clone https://github.com/Rambeboy/pitch-talk-bot.git && cd pitch-talk-bot
   ```
2. Install dependencies
   ```
   npm install && npm i telegram@2.22.2
   ```
4. Make new accounts folder
   ```
   mkdir -p accounts
   ```
5. Configure all folder
   ```
   cp config/config_tmp.js config/config.js && cp config/proxy_list_tmp.js config/proxy_list.js
   ```
6. (If You Use Telegram Sessions) To configure the app, run
   ```
   nano config/config.js
   ```
   and add your telegram app id and hash there.
7. (If You Use Proxy) To configure the app, run
   ```
   nano config/proxy_list.js
   ```
   and add your proxy list there, use http proxy
8. To start the app run
   ```
   npm run start
   ```
9. if any error regarding `config.js` not found, or `proxy_list.js` not found, try to copy `config` folder to `app` folder. make sure you have those file inside `config` folder.

### WINDOWS

1. Open your `Command Prompt` or `Power Shell`.

2. Clone project repository
   ```
   git clone https://github.com/Rambeboy/pitch-talk-bot.git && cd pitch-talk-bot
   ```
3. Install dependencies
   ```
   npm install && npm i telegram@2.22.2
   ```

5. Navigate to `pitch-talk-bot` directory.

6. Make new folder named `accounts`.

7. Navigate to `config` folder and rename `config_tmp.js` to `config.js` also `proxy_list_tmp.js` to `proxy_list.js`.

8. Now Open and configure `config.js`.
9. Now back to the `pitch-talk-bot` folder
10. To start the app open your `Command Prompt` or `Power Shell` again and run
    ```
    npm run start
    ```
11. If Any error happen contains config or proxy, Copy `config` folder to `app` folder
12. Finally run with
    ```
    node app/index.js
    ```

## UPDATE BOT

To update bot follow this step :

1. Run
   ```
   git pull
   ```
   or
   ```
   git pull --rebase
   ```
   if error run
   ```
   git stash && git pull
   ```
2. Run
   ```
   npm update
   ```
3. Start the bot.

## SETUP ACCOUNTS

1. Run bot `npm run start`.
2. Choose option `1` to create account
3. Choose account type `Query` or `Sessions`.
4. `Session` Type.
- Enter Account Name.
- Enter your phone number starting. with countrycode ex : `+628xxxxxxxx`
- You will be asked for verification code and password (if any).
- Start The bot Again after account creation complete.
5. `Query` Type.
- Enter Account Name.
- Enter Telegram Query (you can get query by opening bot app on browser > inspect element > storage / application > session storage > telegram init params > copy tg web app data value).
- Start The bot Again after account creation complete.
6. After bot started choose option `3` start bot.

## SESSION TROUBLESHOOT

If you asked to enter phone number again after sessions creation, it mean session not initialized correctly, try to delete the created sessions.

Example Case

- example you already have 1 session (sessionA) and all good when you run bot. After that you create another session, but when you run bot, the bot asked to enter phone number again, so the problem is on (sessionB), to fix it just remove the `accounts/sessionB` folder and re create it or just delete all folder inside `accounts` directory with prefix `sessions-`.

## QUERY TROUBLESHOOT

if your bot get eror, with some error code `401` it mean your query expired, go get new query and run bot again and choose option `4` for query modification.

## NOTE

Don't use bot with `session` type if you using telegram account that bought from someone because it can make your telegram account deleted. instead of using `session` type, use `query` type.

This bot can use Telegram Query and Telegram Sessions. if you want to use sessions, and ever use one of my bot that use telegram sessions, you can just copy the `accounts` folder to this bot. Also for the telegram APP ID and Hash you can use it from another bot. If you want to use Telegram Query, get your query manually.

if you got error `Invalid ConstructorId` try to run this `npm i telegram@2.22.2`.

## LICENSE

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
