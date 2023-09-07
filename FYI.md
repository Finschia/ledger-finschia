# Guide for Finschia

## Install dependencies
```sh
make deps
```

## Set dev mode for testing
> Reset PIN if you need during setting

1. Plug your device while pressing the right button
2.  Your device will show "Recovery" in the screen
3. Double click
4. Run `make dev_init`. This will take about 2 minutes. The device will be initialized to:
5. Run `make dev_ca`. The device will receive a development certificate to avoid constant manual confirmations.
6. Install the app on the device
```sh
# Builds the app (NANO S/SP/X)
COIN=FNSA make

# Load the app onto the device (Install apps on the device)
make load    # Nano S
make loadS2  # Nano S Plus
make loadX   # Nano X
```
