# deMe - eMed Selenium Web Scraper

## Requirements

- Python 3
- Pip 22.2.2+

You will need to install these in your computer before starting the setup

## Setup

1. Download required packages by running command

   ```
   pip install -r requirements.txt
   ```

   --- or ---

   ```
   pip3 install -r requirements.txt
   ```

2. Create a `config.ini`
   > **_Note:_** Use example file `config.ini.example` as a starting point
3. Get the `service_account.json` file from 1Password and put it in the root directory of this project
   > Ask vahid@niuhealth.com on how to get access to this file
4. Run the following command
   ```
   python run_niu.py
   ```
   --- or ---
   ```
   python3 run_niu.py
   ```

---

## Config INI Data Dictionary

| Key        | Description                                                                                                          | Type      |
| ---------- | -------------------------------------------------------------------------------------------------------------------- | --------- |
| `loginid`  | The username to log into eMedical                                                                                    | `string`  |
| `password` | The password to login into eMedical                                                                                  | `string`  |
| `datadir`  | The full path to where you want to output the data files into                                                        | `string`  |
| `driveid`  | The folder ID in Google Drive. You can get this from the url when selected on the shared drive you want to upload to | `string`  |
| `daysago`  | The amount of days ago to get data from. 1 is yesterday, 0 is today                                                  | `integer` |
