# Home Assistant Component for a remote picoTTS installation.

[![hacs_badge](https://img.shields.io/badge/HACS-default-orange.svg)](https://github.com/custom-components/hacs)

This is a component for Home Assistant which integrates picoTTS from a remote server.
Its recommended to run the server via my [Home Assistant Supervisor Addon](https://github.com/Poeschl/Hassio-Addons/tree/master/picoTTS).

# Installation

## HACS

Install it in the `Integrations` tab on the [Home Asssistant Community Store](https://github.com/custom-components/hacs).

## Manual way
To use it, copy the `picotts_remote` folder inside your `config/custom_components` folder on your home assistant installation first.


# Configuration

Add following config to your yaml if you are using the Supervisor Addon

```yaml
tts:
  - platform: picotts_remote

```
The integration will connect to picoTTS after an Home Assistant restart.

## Other host

For setting your own host and port:

```yaml
tts:
  - platform: picotts_remote
    host: <host>
    port: <port>

```

## Language

The languge can be set to the languages: `en-US`, `en-GB`, `de-DE`, `es-ES`, `fr-FR` and `it-IT` via the `language` key.

```yaml
tts:
  - platform: picotts_remote
    language: "de-DE"

```
