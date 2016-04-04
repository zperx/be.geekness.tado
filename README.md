# com.tado

Unofficial Tado thermostat app for Homey.

## Installation

```sh
# Install Homey development tools
npm install -g athom-cli

# Connect to your Homey
athom login

# Download Tado application
git clone https://github.com/hellhond/com.tado.git

# Install app on Homey
cd com.tado
athom project --install
```

## Flow

### Triggers (device)

- The temperature changed (temperature token, in increments of 0.5 °C)

- The target temperature changed (temperature token)


### Triggers (app)

- Weather state changed to ... (state token)

- Weather changed (state token, different values: RAIN, CLEAR, NIGHT_CLOUDY, CLOUDY_PARTLY, THUNDERSTORMS, SUN, WINDY, etc.) (1)

- Solar intensity changed (intensity token, value in percentage [0..100])

- Outside temperature changed (temperature token, in increments of 0.5 °C)


### Conditions

- none at the moment, any ideas ?


### Actions (device)

- Set the temperature


## Bugs & Features

If you find a bug, please use the Github Issue system for this repository to submit the details of your bug report.

If you would like to have a new feature implemented, use the Github Issue system to submit your feature request.


## Legal

This is an unofficial Tado app, built by/for the Homey community. The app is provided "as is", without warranty of any kind.



