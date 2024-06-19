# Redox keyboard

## change keymap


### producing a pre-compiled binary firmware (bin/hex) to be flashed

1. Use the [qmk configurator](https://config.qmk.fm/#/redox/rev1/base/LAYOUT)
2. Upload the redox.json in this repo for a starting point
3. Hit compile and donwload the `.hex` artifact

### Using [QMK Toolbox](https://github.com/qmk/qmk_toolbox)

1. Using [QMK Toolbox](https://github.com/qmk/qmk_toolbox) upload the `.hex` file
2. hit auto-flash and press reset button below the keyboard for flashing

In alternative of point 4/5 you can use `qmk` CLI locally (QMK Toolbox not available for linux):

1. Issue the `qmk flash` command:
    ```sh
    qmk flash -kb redox/rev1/base redox_rev1_base_redox.hex
    ````
2. press reset button below the keyboard


