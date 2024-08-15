# How to tell what your next punishment will be in the banwave

## Steps

### 1. Open Developer Tools (Inspect Element)
- **Right-click** anywhere on the webpage you want to inspect.
- Select **"Inspect"** from the context menu that appears.
  - Alternatively, you can press **`F12`** or **`Ctrl + Shift + I`** (Windows/Linux) or **`Cmd + Option + I`** (Mac) to open Developer Tools.

### 2. Navigate to the Network Tab
- In the Developer Tools panel, click on the **"Network"** tab.
  - This tab displays all network requests made by the webpage.

### 3. Stop Recording Network Activity
- Look for the **red circle** at the top-left corner of the Network tab.
  - This indicates that network activity recording is currently enabled.
- Click the **red circle** to stop recording.
  - The circle will turn **gray** when recording is stopped.

### 4. Start Recording Network Activity
- To resume recording, click the **gray circle**.
  - The circle will turn **red** to indicate that recording is active.

### 5. Refresh the Page
- **Refresh** the webpage by pressing **`F5`** or clicking the refresh button in your browser.
  - The Network tab will start populating with network requests as the page reloads.

### 6. Search for "punished"
- In the Network tab, use the **search bar** to find specific requests.
  - If you don't see a search bar, press **`Ctrl + F`** (Windows/Linux) or **`Cmd + F`** (Mac) to open it.
- Type **"punished"** into the search bar and press **`Enter`**.
  - The network panel will filter results to show only requests that match "punished".

### 7. Click on the "not-approved" Request
- In the filtered results, find a request that includes **"not-approved"** in its name or status.
- Click on that request to view more details, such as headers, payload, and response data.

## You see something like this:

```json
{
    "punishedUserId": 3954281267,
    "interventionId": "5ed14041-c235-4567-a00f-8a1756607c74",
    "punishmentId": 0,
    "messageToUser": "Roblox does not permit the use of third-party software to modify the client.",
    "punishmentTypeDescription": "Ban 3 Days",
    "beginDate": "2024-08-14T04:03:47.269Z",
    "endDate": "2024-08-17T04:03:47.269Z",
    "badUtterances": [
        {
            "abuseType": "ABUSE_TYPE_CHEAT_AND_EXPLOITS",
            "utteranceText": "ExploitDetected - Place ID : 286090429",
            "imageUrl": null
        }
    ],
    "context": {
        "NEXT_CONSEQUENCE_DURATION": 7,
        "NEXT_CONSEQUENCE_TYPE": "BAN"
    },
    "verificationCategory": "",
    "consequenceTransparencyMessage": "",
    "showAppealsProcessLink": false,
    "isForeshadowingConsequenceEnabled": false
}
```
# What does this mean?
## this tells you what punishment you will get if you are caught in the next banwave
### The only thing that really matters is this part:
```json
{
    "context": {
        "NEXT_CONSEQUENCE_DURATION": 7,
        "NEXT_CONSEQUENCE_TYPE": "BAN"
    },

}
```
### So if you have this:
```json
{
    "context": {
        "NEXT_CONSEQUENCE_DURATION": 1,
        "NEXT_CONSEQUENCE_TYPE": "BAN"
    },

}
```
that means you are going to get banned for a day
### if you have this:
```json
{
    "context": {
        "NEXT_CONSEQUENCE_DURATION": 3,
        "NEXT_CONSEQUENCE_TYPE": "BAN"
    },

}
```
that means you are going to get banned for 3 days
### if you have this:
```json
{
    "context": {
        "NEXT_CONSEQUENCE_DURATION": 7,
        "NEXT_CONSEQUENCE_TYPE": "BAN"
    },

}
```
that means you are going to get banned for 7 days
### The scariest of all if you have this one:
```json
{
    "context": {
        "NEXT_CONSEQUENCE_DURATION": 0,
        "NEXT_CONSEQUENCE_TYPE": "DELETE"
    },

}
```
Your account will be TERMINATED if caught in the next banwave.

# How can I be safe and not get my account banned / terminated in the next banwave with quitting exploiting?
## Basically other then deactivating your account before a banwave (and that is still not 100% safe at all) there is no way to be safe in the banwave when cheating.

# How does the banwave work?
## basically here is how it goes
### 1 day ban (first offense)
### 3 day ban 
### 7 day ban
### Account / IP or HWID Banning
