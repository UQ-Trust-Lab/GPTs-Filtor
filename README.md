# GPTs-Filtor
GPTs-Filtor leverage the unique characteristics of GPTs’ deployment, to conduct in-depth analysis and detection of file knowledge leakage at both user interaction and network transmission levels.

## Environment and equipment requirements
Before running GPTs-Filtor, make sure your system meets the following requirements
### Operating System
macOS **12 Monterey** or later (tested on macOS 13 Ventura & macOS 14 Sonoma)
### Browser Support
Google Chrome Version 120+ (Ensure that Chrome is installed and set as the default browser)
### AppleScript Permissions
- **Full Disk Access** must be granted to Terminal or Script Editor:
  - **System Settings → Privacy & Security → Full Disk Access**  
  - Enable **Terminal** and **Script Editor** 
### Charles Proxy
- **Version 4.76 or later** *(Ensure Charles is installed and running before executing the script.)*
- Download: [Charles Proxy Official Website](https://www.charlesproxy.com/download/latest-release/)
- Allow Charles to intercept SSL traffic (`Help → SSL Proxying → Install Charles Root Certificate`)

### Other required
Don't forget to login your ChatGPT account!😊

## Let's get started with GPTs-Filtor!! 🚀🚀🚀
### Quick Start
```bash
osascript /path/to/gpts_interaction_script.scpt
```
### Step 1: Specify GPT URLs
- Open the `GPTs-Filtor/GPTs.txt` file.
- Add the GPT URLs you wish to test. Each URL should be on a new line.
  *Note: Three example URLs have already been provided in `GPTs.txt`.*

### Step 2: Modify Test Prompts
- Navigate to `GPTs-Filtor/gpts_interaction_script`.
- Locate the `sentenceList` variable.
- Modify the prompts to the ones you want to test.
- The script will randomly pick from these test cases during execution.


### Step 3: Modify Test Prompts
- Run Charles Proxy
- Select `auto save` under the `Tool`.
<img src="https://github.com/UQ-Trust-Lab/GPTs-Filtor/blob/main/assets/tool.png" width="300px">
## Notes
- The script allows for multiple interactions per experiment.
- If changes are needed, only update the values of each `keystroke`.
- Ensure stable network connectivity for smooth interaction with GPTs.
