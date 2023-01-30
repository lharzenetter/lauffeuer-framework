# Install Mosquitto

1. `sudo apt-add-repository ppa:mosquitto-dev/mosquitto-ppa`
2. `sudo apt-get update`
3. `sudo apt-get install mosquitto`
4. `sudo nano /etc/mosquitto/conf.d/default.conf` --> <https://hostadvice.com/how-to/how-to-install-and-configure-mosquitto-mqtt-on-your-ubuntu-18-04-server/>
    File is empty - add:
    ```
    listener 1883
    Allow_anonymous true
    ```
5. <kbd>Ctrl</kbd> + <kbd>O</kbd> -> Speichern
6. <kbd>Ctrl</kbd> + <kbd>X</kbd> -> Exit
7. `sudo systemctl restart mosquitto`
8. `sudo systemctl status mosquitto`

--> Mosquitto is listening on port 1883 for all requestes