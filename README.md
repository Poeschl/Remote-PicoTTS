# remote picoTTS Home Assistant Component

This is a new component for [Home-Assitant](https://www.home-assistant.io/) which integrates picoTTS as a remote server. The server is running inside my [Hass.io picoTTS Addon](https://github.com/Poeschl/Hassio-Addons/tree/master/picoTTS).

# Installation

To use it, copy the `picotts_remote` folder inside your `config/custom_components` folder on your home assistant installation first.

Afterwards add following config to your yaml:

```yaml
tts:
  - platform: picotts_remote
    host: <host>
    port: <port>

```

# Note

I intend to integrate this one in the official home assistant components, but got only limited time right now. If you want to help out, go on.
