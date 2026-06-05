<p align="center">
Windows 11 Settings App condsensed visual style customizations
<br>
(via Windhawk customization engine)
</p>

#### Densy

A condensed style:
  - Removed a lot of extra whitespace
    - Before: ![Settings_1Before](./img/Settings_1Before.png)
    - After: ![Settings_2After](./img/Settings_2After.png)
  - …and a few helpful ads
    - ![Settings_remove_msg](./img/remove_msg.png)
  - Cleaner lists without border separators, e.g., installed app list:
    - ![App_List_0Before](./img/App_List_0Before.png)
    - ![App_List_1After](./img/App_List_1After.png)

## Known issues
  - descriptions in 1-line items are not vertically aligned ![v-misalignment](./img/Settings_issue_vertical_misalignment.png), not sure whether it's possible to fix using XAML styling alone and these 2 grid child lines (name/description) have to be aware of the size of it's cousins, so would likely need a change in the whole grandparent structure (a table)
  - not all lines (especially those in sub-menus) have been restyled
  - some views (like "Apps > Installed apps") crash the Settings app if their orientation is changed to collapse 2 rows into 1 row of 2 columns, so they're left as is
  - a few lines have 3 rows that don't fit into the current height constraints; or 2 lines might have the subtitle line slightly cut off

## Credits
  - [Windhawk](https://windhawk.net) mod engine
  - [Windows 11 Start Menu Styler](https://windhawk.net/mods/windows-11-start-menu-styler), which this one is based upon
