# Roku Remote Control Example

A lightweight working example written in **Yab** for controlling a Roku TV directly from **Haiku OS** using cURL.

![App Screenshot](https://github.com/GearPlot/remote/blob/main/screenshot.png)

## Requirements

* **Haiku OS**: The operating system environment for running Yab.
* **Yab**: Ensure the Yet Another Basic interpreter is installed on your Haiku system.
* **cURL**: Available in your Haiku command path.
* **Roku TV**: Must be on the same local network as your Haiku machine.

## Setup & Configuration

Because this is a source code example rather than a compiled binary, you must configure your local settings directly inside the Yab script before running it.

1. Open the script file in a text editor (like StyledEdit).
2. Update the `ipAddress$` variable with your Roku TV's local IP address:
```basic
ipAddress$ = "192.168.1.1"

```


3. Configure your shortcut buttons by setting the app name and its corresponding Roku App ID.
To find the App IDs installed on your specific TV, run the following command in Terminal (replace `192.168.1.1` with your actual TV IP address):
```bash
curl "http://192.168.1.1:8060/query/apps"

```


Then update the script variables:
```basic
appOne$ = "Pluto TV"   // Label for your reference
appOneID$ = "74519"    // The target App ID from your TV

```



## Usage

Run the Yab script from Tracker or the Terminal to launch the interface and control your Roku TV.
