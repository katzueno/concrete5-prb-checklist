# concrete5-prb-checklist

The check list for PRB Reviewers how to review the add-on.
This is how Katz review the add-ons for concrete5

## Common Initial Steps

- Add-on Itself
    - Does the Title of the Add-on/Theme represent what it is about?
    - Does the title violate trademark and copyright or misrepresent the add-on author is the actual service providers? (If they are official service provider, they can claim add-on/theme to be official one.)
    - Doesn't it use depreciated class, functions and methods or any other legacy stuff
- Marketplace and Documentation
    - If the page has proper screenshot.
    - If the page has proper description of the add-on
    - If the page properly describe how to install, set-up, use and uninstall (if special care needed)
    - If the add-on/theme front page is not too long and too complicated (that they should create additional page such as Documentation).
    - If the marketplace page represent the add-on/theme properly and fairly explain what is this add-on/theme is all about.
    - The marketplace place could contain other language rather than English. But English is primary language for the marketplace.
- Unzip and see if it contains any extra files
- Upload onto your concrete5 testing site
- Check to see if it installs
- Check if the license.txt is properly mentioned
- Open all files and check the followings
    - If the add-on includes third-party library, make sure if it doesn't violate its license
    - Check to see if the strings are properly wrapped with t()
- Check to see if the add-on is properly made against any security threat
    - Does it properly escape, validate against XSS
    - Does it properly handled against SQL Injection
- Does it has clear description of that the add-on/theme has on the marketplace page?
- Images
    - Does it comply any copyright laws?
    - If they use the royalty free license, make sure they purchased the add-on licenses instead of regular ones

## Installation

- Does it run on the minimum required concrete5 version?
- Does it run on the various PHP versions? (or minimum PHP version indicated otherwise)
    - For 5.6.x, PHP 5.2.4 and above
    - For 5.7.x, PHP 5.3.3 and above
    - For 8.x, PHP 5.5.9 and above
- Does it run on PHP 7 (7.2) and the latest PHP version?

## Upgrade

- Does it upgrade to the new version?

## Uninstallation

- Does it uninstall?
- Does it delete all tables that was made for this package?
- Doesn't it break the site after the uninstallation?

## Add-on

- Can you add the block to an area?
- Can you add the block to a global area?
- Can you add the block to a stack?
- Does it work within the grid layout?
- Can you edit a block
- Can you move a block
- Can you delete a block
- Can you have multiple uses of a block on the same page?
- Can you copy/paste a block on the same page?
- Are the block database tables and columns (db.xml or other) appropriate to the purpose?
- If a block is saved with empty or un-edited data, does it cause errors?
- If a block is saved with typos or other mistakes in the data, does it cause errors?
- Are all inputs appropriately validated?

## Dashboard Page

- Dashboard page (if any)
    - Does it install the single page properly?
    - If a dashboard page is saved with empty or un-edited data, does it cause errors?
    - If a dashboard page is saved with typos or other mistakes in the data, does it cause errors?
    - Are all inputs appropriately validated?

- Are the package database tables and columns (db.xml or other) appropriate to the purpose?


## Job

- Does it install
- Does it run?

## Themes

- If contents swap, does it swap properly?
    - Theme
    - Custom Templates (if any)
    - Custom Block (if any)
- Does the custom template works as it says?
- Doesn't it override the default cocnrete5 UI?
- If the theme provides blocks or dashboard pages, all the checks for add-on blocks and dashboard pages also apply to the theme.

