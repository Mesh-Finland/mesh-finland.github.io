# Enabling MQTT on Meshtastic: A Short Guide (Non-CLI)

Meshtastic is a versatile open-source communication platform that can be enhanced with MQTT (Message Queuing Telemetry Transport) for extensive messaging capabilities. Here’s a quick guide on enabling MQTT for your Meshtastic

## Prerequisites

1. **Meshtastic Device**: Ensure your device is properly set up and operational.
2. **Meshtastic Firmware**: Update your device to the latest firmware version that supports MQTT.
3. **MQTT Broker**: Use the default MQTT broker `mqtt.meshtastic.org` or set up your own broker if preferred.

## Step-by-Step Guide

### 1. Access Device Settings

1. **Wait for Device to Start and Connect**: Ensure your Meshtastic device has started up and connected.
2. **Open Settings**: Access the settings or configuration section of the Meshtastic app or web interface.

### 2. Configure MQTT Settings

1. **Locate MQTT Settings**: Find the MQTT configuration section in the settings menu.
2. **Enable MQTT**: Toggle the setting to enable MQTT.
3. **Set MQTT Broker**: If not already set, enter the default MQTT broker address and port.
   - **Broker Address**: `mqtt.meshtastic.org`
   - **Port**: `1883` (default port)
4. **Set MQTT Root Topic**: Enter the root topic `msh/Finland`.
5. **Save Changes**: Press the `Send` button to save the MQTT settings. The device will restart automatically.

### 3. Enable Uplink and Downlink for Specific Channels

1. **Wait for Device to Start and Connect**: After the device restarts, ensure it has started up and connected.
2. **Locate Channel Settings**: Navigate to the channels configuration section.
3. **Select Channel (LongFast)**: Choose the `LongFast` channel (or any other channels you want to configure).
4. **Enable Uplink**: Toggle the setting to enable uplink for the selected channel.
5. **Enable Downlink**: Toggle the setting to enable downlink for the selected channel.
6. **Save Changes**: Press the `Send` button to save the channel settings. The device will restart automatically.

### 4. Disable MQTT Ignoring in LoRa Settings

1. **Wait for Device to Start and Connect**: After the device restarts again, ensure it has started up and connected.
2. **Locate LoRa Settings**: Navigate to the LoRa settings section.
3. **Disable `Ignore MQTT`**: Ensure the `Ignore MQTT` setting is disabled.
4. **Save Changes**: Press the `Send` button to save the LoRa settings. The device will restart automatically.

### 5. Verify Configuration

1. **Wait for Device to Start and Connect**: After the final restart, ensure your device has started up and connected.
2. **Verify Settings**: Check the settings again to confirm that the MQTT configuration is active and all changes have been applied.

## Conclusion

By following these steps, you should have MQTT successfully enabled on your Meshtastic device with the root topic `msh/Finland`. Ensure that only the desired channels have uplink and downlink enabled, and that the `Ignore MQTT` setting in LoRa settings is disabled. Remember, the device will restart automatically each time you press the `Send` button after making changes. Enjoy enhanced messaging capabilities with your Meshtastic network!
