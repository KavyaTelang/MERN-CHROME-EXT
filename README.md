# MERN-CHROME-EXT
**COMPANY** : CODTECH IT SOLUTIONS

**NAME** : KAVYA TELANG

**INTERN ID** : CT6WKLY

**DOMAIN** : MERN STACK WEB DEVELOPMENT 

**BATCH DURATION** : January 20th, 2025 to March 5th, 2025

**MENTOR NAME** : Neela Santhosh

##  **Features**  

-  **Automatic Time Tracking** – Logs time spent on each website while browsing.  
-  **Visual Statistics** – Displays time data using an interactive bar chart.  
-  **Persistent Data Storage** – Uses Chrome’s `storage.local` API to save session history.  
-  **User-Friendly Interface** – A clean, minimal popup UI for easy access.  
-  **Real-Time Updates** – Data updates dynamically as the user browses.  
-  **Lightweight & Efficient** – Runs in the background without slowing down the browser.  

##  **Tech Stack**  

- **Frontend:** HTML, CSS, JavaScript  
- **Backend:** Chrome Extension APIs  
- **Libraries:** jQuery, Chart.js  
- **Storage:** Chrome Storage API  

##  **Project Structure**  

```
web-time-tracker/
│── manifest.json        # Chrome extension configuration
│── background.js        # Main tracking logic running in the background
│── popup.html           # UI for the popup display
│── popup.js             # JavaScript logic for displaying stats in the popup
│── custom.css           # Styling for the popup UI
│── Chart.min.js         # Library for visualizing time-tracking data
```

## Working 

- The extension runs a **background script (`background.js`)** that listens for **tab changes** and calculates time spent on each website.  
- The data is **stored locally** using `chrome.storage.local`, allowing persistent time tracking.  
- When users click the extension icon, the **popup (`popup.html` and `popup.js`)** displays the time spent per website.  
- **Chart.js** is used to render time-tracking data in an easy-to-understand bar chart.  


### Implementing Background Tracking (`background.js`)
The **background script** is responsible for continuously monitoring active tabs and logging time spent on websites. It works as follows:

1. **Detecting Tab Changes**: The script listens for tab switches using the `chrome.tabs.onActivated` event.
2. **Tracking Time**: When a user switches to a new tab, the script calculates how long they spent on the previous site and stores this data.
3. **Storing Data**: The extension uses Chrome's storage API (`chrome.storage.local`) to store website visit durations.
4. **Updating Statistics**: The stored data is periodically updated to keep an accurate log.

---

### Designing the Popup UI (`popup.html` & `popup.js`)
The popup interface allows users to view their tracked time in an intuitive format.

- **`popup.html`**: Contains a structured layout with buttons, text sections, and a canvas for displaying charts.
- **`popup.js`**: Fetches stored time-tracking data and dynamically updates the UI.
- **Chart.js Integration**: Uses the `Chart.min.js` library to display time-spent data in visually appealing bar charts.

---

### Styling with Custom CSS (`custom.css`)**
To make the UI more user-friendly, the extension employs:
- **Bootstrap Grid** for responsive design.
- **Custom fonts and colors** for a modern, sleek look.

# OUTPUT - 
![image](https://github.com/user-attachments/assets/7ab10447-f9b0-4788-afad-d9d4fbbd2565)

![image](https://github.com/user-attachments/assets/35779273-d070-4b01-8975-3801ba7e61f0)


