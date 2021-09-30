This archive contains the file `userChrome.css` which changes the tabs design in Firefox 89+ (Proton UI) to design similar to the one from Firefox 88. 

Firefox 89+ tabs look (with default Dark Theme, ProtonUI disabled (steps 1-3) and compact mode set (steps 4-5)):
![old](https://user-images.githubusercontent.com/62106309/131740012-6e7a40a5-d755-4fed-b45b-15599a12d206.PNG)

The tabs after using `userChrome.css` from this repo:
![new](https://user-images.githubusercontent.com/62106309/135512812-919d0cb4-e585-4d72-926f-2d09a938ce99.PNG)

Tested on Firefox 91.0.2

### Usage

1. Open Firefox and type `about:config` into the address bar and hit enter
2. In the search box, enter `proton`
3. Set the following settings to `false`:
    ```
    browser.aboutwelcome.protonDesign
    browser.proton.enabled
    browser.proton.places-tooltip.enabled
    ```
4. Find and set the following settings to `true`:
    ```
    browser.compactmode.show
    toolkit.legacyUserProfileCustomizations.stylesheets
    ```
----
5. Click on menu symbol `≡` -> `More tools` -> `Customise toolbar...`
6. At the bottom, click on `Density` and choose `Compact`
---
7. Open new tab, enter `about:support` and hit enter
8. Search for `Profile Folder` and click `Open Folder`
9. In that directory create `chrome` folder 
10. Inside, paste the file `userChrome.css` from this repository and restart Firefox
