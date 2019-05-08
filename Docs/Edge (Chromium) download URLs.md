MacOS
--------------
Canary
* `https://officecdn.microsoft.com/pr/C1297A47-86C4-4C1F-97FA-950631F94777/MacAutoupdate/MicrosoftEdgeCanary-76.0.151.0.pkg`


Dev
* `https://officecdn.microsoft.com/pr/C1297A47-86C4-4C1F-97FA-950631F94777/MacAutoupdate/MicrosoftEdgeDev-76.0.151.0.pkg`



Windows
--------------
Canary
* `http://msedge.f.tlu.dl.delivery.mp.microsoft.com/filestreamingservice/files/f4099050-e168-4b0c-9ae3-1ed353ec0486?P1=1555764601&P2=402&P3=2&P4=ZMXei6LNRzOtq0N59ZRnGWSgb1c1vX400i9svGbAQGDbgulUp23%2fGUX7%2bQp3P0IPiRixJQVlq5XGmHG%2bsa1Q9A%3d%3d`


Dev
* `http://msedge.f.tlu.dl.delivery.mp.microsoft.com/filestreamingservice/files/e88bee66-e036-4740-8d67-d9f9042009e8?P1=1557363860&P2=402&P3=2&P4=UYitwtY09unqqGKv0iM%2f66AbYbIJyljmwm3rbQZLo3O1fBM7BBLcWZkwP7a0BmX0nu0vSgIB6j3Zw9%2fSjdOt6g%3d%3d`


Beta
- None (yet)


### Information about the URL scheme

The SHA1 hash and the URL rotates, depending on the version you like to download (yes, MS keeps older versions). The above links are basically only examples.


Sandbox (users)
--------------
Under `C:\Users\WDAGUtilityAccount\AppData\Local\MicrosoftEdge` there is the `Applicationmsedge.exe`.




User Agent switcher (still works but might gets removed)
--------------

```batch
// Facebook
"domain":"facebook.com",
               "applied_policy":"ChromeUA"
```

```batch
// Netflix, HBO etc (for DRM)
"domain":"netflix.com",
               "applied_policy":"EdgeUA"
```

More info about the User-Agent switcher is avbl. [here](https://www.bleepingcomputer.com/news/microsoft/the-new-microsoft-edge-sometimes-impersonates-other-browsers/).


Change default display language
--------------
Close Microsoft Edge (Chromium) and ensure no background task is running! Download the desired language pack from [here](https://chromium.googlesource.com/chromium/reference_builds/chrome_win/+/f4b7e74a777e85405b284a55ce6e3d798bca7159/locales), it is a `.pak` file.


* Canary: `C:\Users\<your-user/pc-name>\AppData\Local\Microsoft\Edge SxS\Application\76.0.152.0\Locales`
* Dev:    `C:\Program Files (x86)\Microsoft\Edge Dev\Application\75.0.139.4\Locales`
* Beta:   `C:\Program Files (x86)\Microsoft\Edge Beta\Application\75.0.139.7\Locales`



Create a new folder and place every other language into it EXCEPT the one you like to switch to so e.g `\Locales\New Folder\` & `\Locales\ru.pak` is then your folder structure. Restart Edge after you're done.


**Warning**
* After you changed the language you might get DPI problems (e.g. the menu is to wide). That's a _known problem_ and depending which DPI you set for your fonts.


Download links
--------------

* https://32767.ga/edge/
* https://chromium.googlesource.com/chromium/reference_builds/chrome_win/+/f4b7e74a777e85405b284a55ce6e3d798bca7159/locales (language packs)
* https://www.microsoftedgeinsider.com/en-us/download/
