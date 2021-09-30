This archive contains the file `userChrome.css` which changes the tabs design in Firefox 89+ (Proton UI) to design similar to the one from Firefox 88. 

Firefox 89+ tabs look (with default Dark Theme, ProtonUI disabled (steps 1-3) and compact mode set (steps 4-6)):
![old](https://user-images.githubusercontent.com/62106309/131740012-6e7a40a5-d755-4fed-b45b-15599a12d206.PNG)

The tabs after using `userChrome.css` from this repo:
![new](https://user-images.githubusercontent.com/62106309/135513090-5cac6846-c9b7-46b3-b546-71e9ac552b53.PNG)

Tested in Firefox 91.0.2 and 92.0.1

### Usage

1. Open Firefox and type `about:config` into the address bar and hit enter
2. In the search box, enter `proton`
3. Set the following settings to `false`:
    ```
    browser.aboutwelcome.protonDesign
    browser.proton.enabled
    browser.proton.places-tooltip.enabled
    ```
---
4. Find and set the following setting to `true`:
    ```
    browser.compactmode.show
    ```
5. Click on menu symbol `≡` -> `More tools` -> `Customise toolbar...`
6. At the bottom, click on `Density` and choose `Compact`
---
7. Find and set the following setting to `true`:
    ```
    toolkit.legacyUserProfileCustomizations.stylesheets
    ```
8. Open new tab, enter `about:support` and hit enter
9. Search for `Profile Folder` and click `Open Folder`
10. In that directory create `chrome` folder 
11. Inside, paste the file `userChrome.css` from this repository and restart Firefox
