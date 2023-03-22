README= Meraki Device Monitor
Meraki Device Monitor is a Python-based application that monitors the status of devices in a Cisco Meraki organization. The application pings offline devices and sends email notifications if they are unreachable.

Features
Monitor the status of devices in a Cisco Meraki organization
Ping offline devices to check if they are reachable
Send email notifications if devices are unreachable after multiple attempts
Display the monitoring progress in a graphical user interface (GUI)
Requirements
To run this application, you need Python 3.6 or higher installed on your system. The following Python libraries are also required:

requests
smtplib
tkinter
ipaddress
ping3
You can install these libraries using pip:

Copy code
pip install requests ping3
tkinter and ipaddress come pre-installed with Python.

Usage
Clone the repository or download the Python script.

Open the script in a text editor and update the following variables with your own information:

MERAKI_API_KEY: Your Cisco Meraki API key
MERAKI_ORG_ID: Your Cisco Meraki organization ID
EMAIL_SENDER: The email address you want to send email notifications from
EMAIL_PASSWORD: The password for the email address you want to send email notifications from
EMAIL_RECIPIENT: The email address you want to send email notifications to
SMTP_SERVER: The SMTP server for your email provider
SMTP_PORT: The SMTP port for your email provider
Save the script and run it:
Copy code
python your_script.py
The application will open a GUI window. Click the "Start Monitoring" button to start monitoring the devices. The progress will be displayed in the GUI, and email notifications will be sent if any devices are found offline and unreachable.

To stop the application, click the "Exit" button or close the GUI window.

Packaging the Application as an Executable
You can use PyInstaller to package the script as a standalone executable. This allows users to run the application without having Python or the required libraries installed on their computer. Follow the instructions in this answer to package your script as an executable.

License
This project is available under the MIT License.
