# Assignment b4

## Description
The assignment is to enhance the web site you implemented in the previous assignment (b3) with Bootstrap in order to show the web site on small display (e.g., your cell phone).

## Directory Hierarchy:
```
/Library/WebServer/Documents
|--  AwardBio.pdf
|--  index.html             # Main page of the website
|--  index.html.en
|--  scripts
|       |-- main.js         # JavaScript file to manage SPA, History API, and Pagination
|--  sjsu_image.png
|--  styles
|       |-- style.css       # Main CSS file for styling website

3 directories, 6 files
```

## Features
- Single Page Application (SPA): The site behaves like a SPA using the history API and JavaScript to dynamically load content without full page reloads.
- Responsive Design: Bootstrap ensures the website works on mobile devices.
- Pagination: The Web Programming section is split into three pages using a custom pagination system.
- Browser History: Users can navigate back and forth between different sections using the browser’s back/forward buttons.

## Display website on large device (Laptop)
1. Run the Apache
```bash
sudo apachectl -k start
```
2. Open browser and navigate to http://localhost/
5. To end Apache
```bash
sudo apachectl -k stop
```
## Display website on small device (iPhone)
1. Make sure Apache is running.
2. Open brower and navigate to http://localhost/
3. Press 'Cmd + Option + I' on macOS
4. In the Developer Tools window, click on the 'Toggle Device Toolbar' button (it's in the top-left corner of the Developer Tools panel).
5. Feel free to select a predefined mobile device at the top of the page.

## Screenshots
Include screenshots of the page outputs:
  - Laptop version
  - Phone version
