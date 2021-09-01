This archive contains the file `userChrome.css` which changes the tabs design in Firefox 89+ (Proton UI) to design similar to the one from Firefox 88. 

Firefox 89+ tabs look (with default Dark Theme, ProtonUI disabled (steps 1-3) and compact mode set (steps 4-5)):
![old](https://user-images.githubusercontent.com/62106309/131740012-6e7a40a5-d755-4fed-b45b-15599a12d206.PNG)

The tabs after using `userChrome.css` from this repo:
![new](https://user-images.githubusercontent.com/62106309/131740024-6bc18533-5cda-4e51-a728-944b29613c23.PNG)

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
----
4. Click on menu symbol `≡` -> `More tools` -> `Customise toolbar...`
5. At the bottom, click on `Density` and choose `Compact`
---
6. Open new tab, enter `about:support` and hit enter
7. Search for `Profile Folder` and click `Open Folder`
8. In that directory create `chrome` folder 
9. Inside, paste the file `userChrome.css` from this repository and restart Firefox
