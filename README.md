# st - Simple Terminal

**st** is a lightweight and efficient terminal emulator for X, designed to "suck less."

## Requirements

To build **st**, you need the following:

- Xlib header files

## Installation

1. Edit the `config.mk` file to match your local setup. By default, **st** is installed into the `/usr/local` namespace.

2. Build and install **st** using the following commands (use `sudo` if required):

   ```bash
   make clean install
   ```

## Running st

If you did not install st with make clean install, you must compile
the st terminfo entry with the following command:

   ```bash
   tic -sx st.info
   ```

See the man page for additional details.

   ```bash
   man st
   ```

## Customization
The configuration of st is handled through the config.h file. Modify this file to customize the terminal's appearance and behavior, then recompile the source code.

## Credits

Based on Aurélien APTEL <aurelien dot aptel at gmail dot com> bt source code version 0.9.2, with additional modifications by Andrew <andres.ferra@mi.unc.edu> (2024).

## License
st is released under the MIT/X Consortium License. See the LICENSE file for more details.

