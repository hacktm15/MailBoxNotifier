# MailBoxNotifier
Simple ESP8266 MailBox Notifier

At startup tries to connect to AP using the settings stored in EEPROM. If not able then enters Setup mode.

In Setup mode it starts an AP named MAILBOX_NOTIFIER_SETUP wich is a captive portal. You can conect to that portal and configure the device (SSID from scaned available SSIDs, password, SMTP data, Email data). One configured you need to manualy restart the device.

If the device is able to connect to the configured AP it will start monitoring the trigger and send an email (with configured SMTP and Email details).
