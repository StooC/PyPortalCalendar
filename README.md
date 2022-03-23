# Introduction

Google calendar schedule display using the Adafruit PyPortal, the code is based on this [ article by Adafruit](https://learn.adafruit.com/pyportal-google-calendar-event-display) 


# Recommend Development Setup
* Visual Studio Code
* [CircUp](https://learn.adafruit.com/keep-your-circuitpython-libraries-on-devices-up-to-date-with-circup) to manage the libraries [also on GitHub](https://github.com/adafruit/circup)
* Edit the code on development machine and use scripts to copy changes
* Terminal program such as Putty (Windows) or [minicom directly or via WSL on Windows](https://www.hanselman.com/blog/connect-to-a-device-over-serial-com-port-on-windows-10-with-wsl1-tty-devices-with-windows-terminal-and-minicom)

# Troubleshooting
* If you are getting ***RuntimeError: ('Error:', {'error': {'details': [{'links': [{'url': 'https://console.developers.google.com/apis/api/calendar-json.googleapi)*** error then ensure you have **Google Calendar API** enabled in the Google development console. More details on [Google's documentation](https://developers.google.com/calendar/api/v3/reference/events)

* If you are getting **RuntimeError: Failed to request hostname** with the last line of the stack trace **File "adafruit_esp32spi/adafruit_esp32spi.py", line 611, in get_host_by_name** this just seems to be a odd issue with the PyPortal and should work after restarting or unpowering it.

* If you've connected via the **correct** device/COM port but don't see any output from the PyPortal even though the connection seems successful, then try restarting a the PyPortal. Such as by copying the code.py file (any file would do) to it `cp .\src\code.py d:\` (bash\zsh or Powershell or `copy .\src\code.py d:\` in Windows Command Prompt)