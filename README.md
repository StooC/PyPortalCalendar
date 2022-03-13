# Introduction

Google calendar schedule display using the Adafruit PyPortal, the code is based on this [ article by Adafruit](https://learn.adafruit.com/pyportal-google-calendar-event-display) 


# Recommend Development Setup
* Visual Studio Code
* [CircUp](https://learn.adafruit.com/keep-your-circuitpython-libraries-on-devices-up-to-date-with-circup) to manage the libraries [also on GitHub](https://github.com/adafruit/circup)
* Edit the code on development machine and use scripts to copy changes

# Troubleshooting
* If you are getting ***RuntimeError: ('Error:', {'error': {'details': [{'links': [{'url': 'https://console.developers.google.com/apis/api/calendar-json.googleapi)*** error then ensure you have **Google Calendar API** enabled in the Google development console. More details on [Google's documentation](https://developers.google.com/calendar/api/v3/reference/events)

* If you are getting **RuntimeError: Failed to request hostname** with the last line of the stack trace **File "adafruit_esp32spi/adafruit_esp32spi.py", line 611, in get_host_by_name** this just seems to be a odd issue with the PyPortal and should work after restarting or unpowering it.