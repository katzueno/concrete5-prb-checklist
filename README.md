# concrete5-prb-checklist

The check list for PRB Reviewers how to review the add-on.
This is how Katz review the add-ons for concrete5

## Common Initial Steps

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
    - Doesn't it use depreciated class, functions and methods or any other legacy stuff
- Does it has clear description of that the add-on/theme has on the marketplace page?
- Images
    - Does it comply any copyright laws?
    - If they use the royalty free license, make sure they purchased the add-on licenses instead of regular ones

## Installation

- Does it run on the minimum required concrete5 version?
- Does it run on the various PHP versions from 5.3.3? (or minimum PHP version indicated otherwise)
- Does it run on PHP 7 and the latest PHP version?

## Upgrade

- Does it upgrade to the new version?

## Uninstallation

- Does it uninstall?
- Does it delete all tables that was made for this package?
- Doesn't it break the site after the uninstallation?

## Add-on

- Can you add the block to the area?
- Can you add the block to global area?
- Can you add the block to stack?
- Does it work within the grid layout?
- Can you ddit a block
- Can you move a block
- Can you delete a block

## Dashboard Page

- Dashboard page (if any)
    - Does it install the single page properly?

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

