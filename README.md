#### Hardens Chromium and it's settings in the name of security

The goal of this project is to provide information (and an extension maybe?) to setup Chromium for maximum application security (which doesn#t mean you're more secure in terms of that the browser/data aren't attackable). 

[![Twitter URL](https://img.shields.io/twitter/url/https/twitter.com/fold_left.svg?style=social&label=Follow%20%40CHEF-KOCH)](https://twitter.com/CKsTechNews)
[![Say Thanks!](https://img.shields.io/badge/Say%20Thanks-!-1EAEDB.svg)](https://saythanks.io/to/CHEF-KOCH)
[![Discord](https://discordapp.com/api/guilds/418256415874875402/widget.png)](https://discord.me/CHEF-KOCH)

### Chromium vs. Mozilla Firefox Quantum (**still needs to be updated!**)


## Differences between Chrome and Chromium

Chromium was not made by Google, it's a web browser 'developed' (based on parts of the original source code from Chrome) by volunteers and released under FLOSS. There exist bunch of alternative forks of it with additional features in it.

Most core developers are Google employees, you can easily see this in their bug reports (eMail/name) etc, that they work for the Chromium project as 'volunteers' and release the source code but in reality they work for the mother Google, that said not all of them.

A fork means that Google takes the original source code of Chromium and they adding some bits of code and tools (like for example Flash Player (now removed), RLZ etc) Google Chrome itself is either open-source nor proprietary, it's freeware under [Google Chrome's Terms of Service](https://www.google.com/intl/en/chrome/browser/privacy/eula_text.html). Googles Privacy policy can be reviewed [here](https://policies.google.com/privacy?hl=en).



## Performance (Overall)

| Feature        | Chrome           | Firefox Quantum  | Description | 
| ------------- |:-------------:| :-------------:| -------:|
| Startup Memory | Chromium consumes overall more memory than Firefox, but starts up faster - Chromes kernel requires more resources | Firefox loads less fast and on the initial startup it consumes for a short amount of time lots of RAM |  // |
| Multi-core system integration   | Chrome ones is older and more reliable because it's longer tested  |  Firefox isolation feature is (by default) limited | Both perform equal, depending on the used API |
| JavaScript performance | //  |  // | Equal? (depending) |
| _Synthetic Octane benchmark_ | 45169 Points | 43246 Points |
| ARES-6 Browser Benchmark | ~ 21 sec | ~ 50 sec | [Test link](https://browserbench.org/ARES-6/about.html) |
| WebXPRT Test | ~ 275 | ~ 300 | Several API tests |
| Basemark | ~ 1420 | ~ 810 Points | Lots of different tests (encryption etc) |


### Independent performance tests
* [A Quick Look At The Firefox 66.0 vs. Chrome 73.0 Performance Benchmarks (phoronix.com)](https://www.phoronix.com/scan.php?page=news_item&px=Firefox-66-Chrome-73-Benchmarks)


## Privacy & Security Scandals

Firefox
========

* [Firefox browser trusts DarkMatter CA certificate to cause security industry controversy](https://bugzilla.mozilla.org/show_bug.cgi?id=1427262) (see [here](https://www.reuters.com/investigates/special-report/usa-spying-raven/) how it could be abused) _However, this one is questionable and controversial because there is no audit or sign that this was abused_
* [Firefox Users Cry Foul Over 'Mr. Robot' Ad Installed As Research Program](http://fortune.com/2017/12/17/firefox-mr-robot-looking-glass/) [2017]
* [Firefox Shield Studies](https://wiki.mozilla.org/Firefox/Shield/Shield_Studies) - these studies are separate from the normal telemetry
* [Cliqz](https://gist.github.com/solso/423a1104a9e3c1e3b8d7c9ca14e885e5) acquired by Mozilla 
* [Firefox tracks users with Google Analytics in the add-on settings](https://github.com/mozilla/addons-frontend/issues/2785) [2017]
* Most concerns can be destroyed using about:config.
* Firefox has forks in order to (by default) opt-out (without any need of altering about:config). E.g. Waterfox.
* [Mozilla responds to Booking.com Snippet Concerns; “It was not a paid placement or advertisement. We are continually looking for more ways to say thanks for using Firefox."](https://old.reddit.com/r/privacytoolsIO/comments/abfgj5/mozilla_responds_to_bookingcom_snippet_concerns/)


Isn't it funny that [Firefox Wikipedia page](https://gist.github.com/solso/423a1104a9e3c1e3b8d7c9ca14e885e5) has not any section related to Mr. Robot and safebrowsing privacy concerns while Chrome has this mentioned?! Remember Firefox (by default) has also in fact more studies and telemetry integrated in his browser! They even call telemetry in the article as [security](https://en.wikipedia.org/wiki/Firefox#Security) feature. Is this objective written - _I very much doubt it._  


Chrome
========

* ZERO no additional studies or additional telemetry. The stuff which is send back is exactly the same like Mozilla does. Safebrowsing, Malware (Phishing filter updates etc).
* Google sells (officially) only ads. 
* Most concerns can be destroyed using about:flags.
* Chrome has forks (Chromium) in order to (by default) opt-out (without any need of altering about:flags). E.g. Cent Browser.


## Features
* Chromium generally supports the latest HTML features sooner
* Firefox generally supports the latest Javascript features sooner
* Both have mobile versions
* Both manage bookmarks
* Both have a useful dashboard startpage
* Firefox is more extensible
* There are countless themes and extensions, and there's an advanced Customize mode to change the placement of anything on the screen.
* Firefox has an advanced user profile system that's easy to backup
* Both support syncing browser data and preferences between multiple installations, including on mobile
* Firefox allows non-tabbed mode, Chromium does not
* Firefox allows traditional style menus, Chromium does not
* Chrome was the first browser which by default introduced adblocking without any extension ([Android Chrome version got it first](https://www.ghacks.net/2017/07/31/google-launches-adblocker-in-chrome-dev-and-canary-for-android/))

## Extension coverage
* Some extensions like e.g. Ghostery lacks features compared to the Mozilla version
* Chromium has a Downloadbar and limited support for Greasemonkey, Tapermonkey Userscripts by default
* The Firefox extension API is far more powerful than Chromium's; every part of the browser can be customized
* Mozilla adopted WebExtension API which technically can run Chrome/Firefox extensions but it's messy (atm)
* Both extension/theme/plugin stores getting daily scans to avoid malware
* WebKit/WebExtension seems the today's default

## Data privacy with default settings
* Firefox uses Yahoo as its default search engine in North America, and other search engines in other regions
* Chromium uses 'Google' as its default search engine
* Firefox Sync can be hosted on your own server, and uses a zero-knowledge architecture. Chrome Sync only syncs to Google servers but's encrypted.
* Both support private sessions where there is no history saved (private/incognito modes)
* Chromium natively supports WebRTC, just like Edge and Firefox do as well. WebRTC basically can return your IP info if queried, but your browser's usual HTTP headers return IP info and a wealth of other metadata anyway. The potential privacy concern is WebRTC providing IP info if located behind e.g. a VPN or anonymous proxy, so if either apply, block the WebRTC query (among other things) with an extension. If neither apply, then it is pretty much no point of talking about security (no matter which browser).

## Data privacy after user configuration
* Both Firefox and Chromium extensions may send private/usage data to somewhere (with prior warning)
* You can change the default search engines of both to services like DuckDuckGo
* Users can easily disable features of Chromium that remotely use Google-services
* You can selectively enable Chromium's extensions for private sessions
* You can use NoScript in Firefox and µMatrix (formerly HTTP Switchboard) in Firefox and Chromium to greatly enhance your privacy
* Both support the HTTPS Everywhere extension from the Electronic Frontier Foundation
* Both can be configured to use TOR, but the TOR project recommends configuring Firefox or using the Firefox-based Tor browser
* Firefox allows extensive control over which elements of the browser run and transmit data. These can be changed in the about:config page
* Newer versions of Chromium require you download extensions from the Chrome web store or manually install from a local file
* None browser is perfect this is due -> we still using outdated protocols and usability


## Preferences file

See this [documentation](https://chromium.googlesource.com/chromium/src/+/master/docs/user_data_dir.md) for more details regarding to the default profiles.

Windows: C:\Users\<username>\AppData\Local\Google\Chrome\User Data\
MacOS X: ~/Library/Application Support/Google/Chrome/
Linux: ~/.config/google-chrome/


## Media Engagement Index (MEI) (Chrome 66+)

The MEI is determined by a ratio of visits to significant media playback events per origin, determined by these four factors:

* Consumption of the media (audio/video) must be greater than 7 seconds.
* Audio must be present and unmuted.
* Tab with video is active.
* Size of the video (in px) must be greater than 200×140.


## Chrome's integrated Ads-blocker

[Google](https://blog.chromium.org/2018/02/how-chromes-ad-filtering-works.html) is evaluating sites based on the [Better Ads standards](https://www.betterads.org/standards) and then rating them as a pass, warning, or failing. Site owners can access these evaluations using an API, and sites can be re-reviewed after bad ads have been addressed.


## Privacy Concerns

I'll explain in short the privacy concerns and if it's true or already outdated or already fixed. 

<p align="center"> 
<img src="https://raw.githubusercontent.com/CHEF-KOCH/Chromium-hardening/master/Wikipedia/Privacy%20concerns.png">
</p>

The official Wikipedia privacy concerns (User tracking concerns) is outdated.

<p align="center"> 
<img src="https://raw.githubusercontent.com/CHEF-KOCH/Chromium-hardening/master/Wikipedia/Botnet.png">
</p>


| Privacy concern        | Explanation           | 
| ------------- |:-------------:| 
Chrome sends details about its users and their activities to Google through both optional and non-optional user tracking mechanisms. | Google already explained this right from the beginning since 2008 with a [Blog post](https://blog.chromium.org/2008/10/google-chrome-chromium-and-google.html). The privacy settings can also be manually controlled as explained over [here](https://support.google.com/chrome/answer/114836?visit_id=0-636611054822963698-3982001039&rd=1). This is in the meantime an common technique in all current Browser starting from Firefox over Opera and even Edge has some kind of safebrowsing mechanism, safebrowsing itself doesn't contain any personal information which can expose you or your browser habits. The only critical thing someone can find here is that these data are stored locally into your Browser Data folder. |
Every URL you even begin to type in the address bar is sent to Google, in whole or in fragments, for auto-completion purposes. | It's called Omnisearch and can be disabled since many years in Chrome via about:flags. [Google explained how you disable it](https://productforums.google.com/forum/#!topic/chrome/PLaFaRnd1Hw). The Google URL Search prediction (or link prefetching) can be disabled, after that and clearing the Browser Cache it will only show results based on your **Offline** Browser History.  |
Connects to Google every 30 minutes to download a list of malicious URLs, so the fact that you even have Chrome open is transmitted to Google. |  This is a protection mechanism in order to protect you from malware. You can disable it in the options since many years. |
Asks you to login to your Google account, so your browsing tabs, history, etc. is stored on Google servers. | Login is optional since forever and always will be. Every Browser nowadays have a login function. | 
Connects to websites in the background before you are even finished typing them in, without your explicit instruction. | This is a prefetch option to predict stuff to load content more quickly. This doesn't expose you and is not relevant to any privacy aspect. If you don't like it disable it via about:flags. | 
Contains an RLZ identifier, an encoded string sent together with all queries to Google. | RLZ source code was released exactly one week after it got integrated. RLZ will never be send when you install Chrome from official sources. It's however true that on Android it's more problematically but you can use a Chromium based Browser (fork) which doesn't include the RLZ source code. | 
[clientID](http://blogoscoped.com/archive/2008-09-09-n68.html) | The clientID (unique one) was removed already since Aug. 2009 due privacy concerns but no one ever add any proof that this exposes you or fingerprint/track you. |
Page not found | This is not even a tracking method, it's a 404 which are displayed in order to inform the user that the URL/Domain is not reachable. You however can change this behavior with a cached version since Chrome 55. | 
Google Update | This is also not a privacy concern, every Browser has an integrated update mechanism. Using the latest versions which contains security bugfixes is important and the opposite of an privacy concern. Since Android P Google even started to force OEMs to push more frequently security updates for normal users which should help to get less vulnerable. | 
Other features like Do not Track & Co. | Can all be controlled (disabled/enabled) within settings. | 


Privacy related issue tickets can be found [here](https://bugs.chromium.org/p/chromium/issues/list?q=component:Privacy).


**About Ungoogled-Chromium**


[Ungoogled-Chromium](https://github.com/Eloston/ungoogled-chromium) project has major weaknesses too so before you recommend this browser as _alternative_ think about the following: 


```bash
Update as of September 2016: 
I, Eloston, am in a period of time where I do not have as much time as I had before to work on this project...


~~~

Update 9/29: 

Our favorite infosec expert (whom we’ve cited before on a few matters) SwiftOnSecurity, let us know today that Ungoogled Chromium is a student project and doesn’t have the ability to update itself (and likely hasn’t been updated.) In that regard, we can’t recommend it...

```

In other words it has [no auto-updater mechanism integrated](https://lifehacker.com/ungoogled-chromium-strips-away-the-privacy-invading-fea-1787139870), this is for advance users no problem they can use some tools/scripts or manually download and install it but the normal user will never do this. However, in the meantime some things has changed, it more often gets updates now which is a good sign but this is no guarantee for code quality which applies to every Browser or Fork. The release page by itself mostly only provides the source code until the project manager decide to release a new version which is then always behind other forks because it needs to be reviewed over a long(er) time period.  


Using scripts and updater tools can be dangerous when they suddenly starting to download official Google builds, as shown [here](https://github.com/Eloston/ungoogled-chromium/issues/415) which the user is only aware of after everything happened. and Windows Users now need such an updater/downloader in order to get the binaries, read [here](https://github.com/henrypp/chrlauncher/issues/33#issuecomment-279736691) basically this means you must trust someone else because most users will blindly install it and not compile it themselves.I see this critical.


** Conclusion**

Chrome is not more or less tracking anyone then all other Browsers on the market. Other Browser in fact imitates Google and their features such as [Chromecast](https://en.wikipedia.org/wiki/Chromecast) detection which is often misleading called as _background spying_ because it sends every 2 minutes requests in order to check if the service is available or not among other features such as [Captive portal](https://en.wikipedia.org/wiki/Captive_portal) checks. 

Browser Forks mostly only removing integrated functions which is maybe the best way, preventing or giving people a opt-out for certain integrated features is definitely the better method, you can read about how you do this (with examples) [here](https://github.com/CHEF-KOCH/Chromium-hardening/blob/master/Configure%20Google%20Chrome%20via%20Group%20Policies.md).




## Acknowledgments and References
* [Official Google Chrome Group Policy Templates](https://dl.google.com/dl/edgedl/chrome/policy/policy_templates.zip)
* [Chrome Profiles](https://support.google.com/chrome/answer/2364824)
* [Chrome removed the enable_webrtc=false flag (which means no more No-WebRTC builds)](https://chromium.googlesource.com/chromium/src/+/d98b020fe1f0cb85de21de5313261a66ad9c9fe4)
* [Official System Hardening Guide](https://sites.google.com/a/chromium.org/dev/chromium-os/chromiumos-design-docs/system-hardening)
* [Official Chromium Security tracker](https://bugs.chromium.org/p/chromium/issues/list?q=Type%3DBug-Security)
* [Transitioning from SPDY to HTTP/2](https://blog.chromium.org/2016/02/transitioning-from-spdy-to-http2.html)
* [Chrome Vs. Chromium](http://www.linuxinsider.com/story/79510.html)
* [The Private Life of Chromium Browsers](https://thesimplecomputer.info/the-private-life-of-chromium-browsers)
* [How Chromium works](https://medium.com/@aboodman/in-march-2011-i-drafted-an-article-explaining-how-the-team-responsible-for-google-chrome-ships-c479ba623a1b#.is7blrj34)
* [BetterFirefox](https://github.com/CHEF-KOCH/BetterFirefox)
* [Chromium WPAD detection](https://sunweavers.net/blog/node/37)
* [Baselines of Web Browsers](https://thesimplecomputer.info/baselines-web-browsers)
* [Custom DNS names in Chromium](http://michaelkc.tumblr.com/post/98129633274/working-with-custom-dns-names-in-chromium)
* [Compile Chrome on Windows](https://github.com/henrypp/chromium)
* [POTARC](https://github.com/CHEF-KOCH/Online-Privacy-Test-Resource-List)
* [NoScript whitelist](https://github.com/CHEF-KOCH/NoScript-Whitelist)
* [Why isn't passive browser fingerprinting (including passive cookies) in Chrome's threat model?](https://dev.chromium.org/Home/chromium-security/security-faq#TOC-Why-isn-t-passive-browser-fingerprinting-including-passive-cookies-in-Chrome-s-threat-model-) *[ref](https://dev.chromium.org/Home/chromium-security/client-identification-mechanisms)
* [Browser Sec Whitepaper](https://github.com/cure53/browser-sec-whitepaper)
* [Chromium Updater Script by mkorthof](https://github.com/mkorthof/chrupd)
* [Cent Browser](https://www.centbrowser.com/)
* [Privacy disrespected (by default)](https://bugs.chromium.org/p/chromium/issues/detail?id=795526)
* [https://bugs.chromium.org/p/chromium/issues/detail?id=795526](https://bugs.chromium.org/p/chromium/issues/detail?id=661792)
* [DNS caches can be used as cross-domain persistent cookies](https://bugs.chromium.org/p/chromium/issues/detail?id=546733)
* [Chrome Security FAQ](https://chromium.googlesource.com/chromium/src/+/lkcr/docs/security/faq.md)
* [Chrome Browser for enterprise](https://enterprise.google.com/chrome/chrome-browser/)
* [The story of why Chrome and Firefox will soon block sites with certain SSL certificates](https://www.templarbit.com/blog/2018/09/07/the-story-of-why-chrome-and-firefox-will-soon-block-sites-with-certain-ssl-certificates/)
* [Opt-out/opt-in selective on every Google Service](https://takeout.google.com)
* [Microsoft Edge Insider Channels](https://www.microsoftedgeinsider.com/en-us/download/)

## External scripts & tools
* [PowerShell script to get the latest build of Chromium directly from the Chromium Project](https://github.com/RealDrGordonFreeman/Chromigen)


## Papers
* [Web Developer's Guide to Prerendering in Chrome](https://web.archive.org/web/20120309113126/http://code.google.com/chrome/whitepapers/prerender.html)
* [Google Chrome Privacy Whitepaper](https://www.google.com/chrome/privacy/whitepaper.html) **updated frequently by me and other people**
