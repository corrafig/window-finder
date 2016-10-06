# window-finder
Find rapidly any open window and switch to that.
## The problem
My problem was 10 workspaces and too many open windows. Some windows were shaded, some minimized and some just below other windows. It always took a while to find one particular window, even with help of XFCE4 window listing.
## The solution
I wrote `window-finder` and binded it to `meta` + `w` keyboard shortcut. It lists all open windows with additional information and allows filter list by string. 

The window list contains following filterable data:
* workspace
* process name
* window title

When window is selected from the list:
* workspace is changed to same workspace of selected window
* selectedw indow is unshaded
* focus is moved to selected window

# Screenshots
## Window list without filter
![](https://mononen.eu/u/data/window-finder/window-finder0.png)
## Window can be selected from the list
![](https://mononen.eu/u/data/window-finder/window-finder1.png)
## List can be filtered for example by window title
![](https://mononen.eu/u/data/window-finder/window-finder2.png)

# Requirements
* python
* dmenu
* wmctrl
