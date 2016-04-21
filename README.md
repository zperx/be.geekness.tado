# be.geekness.tado

Unofficial Tado thermostat app for Homey.

## Configuration

Go to the Homey settings for Tado, and enter your Tado login and password, this is the same account you use to access https://my.tado.com. This data is only saved locally on your Homey, and not shared with either me or Athom.


## How does it work

The Tado Homey app uses the unofficial my.tado.com API, and does not directly communicate with your Tado device. All data is sent over https, via https://my.tado.com.


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



