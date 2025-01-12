# popcat_bot
popcat.click auto pop sender with feedback.

# "Features"
This simple script have few "features" compared to other shorter alternatives:
* **Tracks** how many pops you sent
* **Notifies** you if there's issue with sending pops
* **Ban-proof** (rate limited to 800 per 30 seconds)
* Shows which **country** you are contributing to
* Uses little system resources
* Works even if you got banned (yes)

![Screenshot 2021-08-14 195741](https://user-images.githubusercontent.com/14260598/129445599-00568de9-1def-4540-9506-0957ae2c1ea4.png)


# How to do it on Android Chrome browser?
You may run the script by connecting to a PC with Chrome and use the **remote debugging** feature:
https://developer.chrome.com/docs/devtools/remote-debugging/

# Known restrictions
It is known that popcat.click can only accept 800 pops per 30 seconds, and you cannot request API again during the 30 seconds cooldown. 

The website also have a function that checks if you clicked more than 800 times and it will track how many times you hit the threshold. You will need to hit the threshold 10 consecutive times to be marked as a bot. The counter will reset when you miss the threshold.

![Screenshot 2021-08-15 141448](https://user-images.githubusercontent.com/14260598/129469081-6dbda7c2-c5cb-46b1-8c11-0dc1601ae84d.png)

If the variable sequential_max_pops reaches 10 and above, you will be flagged as bot and the cat eyes will light up. 
You may clear the website cookies to unflag yourself.

Please don't try running this on same IP (even with different tab, browser, or devices), it won't work, only 1 request/30 seconds is accepted per IP.

![Screenshot 2021-08-14 184105](https://user-images.githubusercontent.com/14260598/129443727-7e95a17c-06b9-49e7-894b-2d2da5ff8a25.png)


# Solving Error 503
Popcat will sometimes respond with an error "503 - Haven't found your country code yet (try again later)". Despite what the error describing, it is most likely not to do with detecting your country, but rather CloudFlare have flagged you as a bot, and the API call failed. Unfortunately, you might need to wait it out.

AdBlocker is known to cause issue as well, simply disable them and see if it works.

# Malaysia
Go Malaysia go!

![popcat](https://user-images.githubusercontent.com/14260598/129445411-15ce2b1c-5402-4ba4-9322-72512731fe8e.gif)

