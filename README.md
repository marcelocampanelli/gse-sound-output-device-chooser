# Gnome Shell Extension - Sound Input & Output Device Chooser
A simple selector to enabled selection of sound source and sink based on Gnome Control Center

### Dependency
Python 2 or 3. New version needs Python as optional dependency. Use option to turn off new profile identification logic, if Python is to be avoided. But the old logic has language dependency and works only with English display language

### Installation Instructions

The official method to install this extension is from [extensions.gnome.org](https://extensions.gnome.org/extension/906/sound-output-device-chooser).

To install from source on GNOME 45–51, run from the repository root:
```bash
make install
```
Log out and back in after installing, then enable the extension. The **Sound Devices**
button in Quick Settings contains the input/output selectors, profiles and optional
application mixer. The Shell's own volume sliders remain available. The old
“expand volume menu” and “integrate with slider” settings apply only to the legacy UI.

For the previous implementation (GNOME 3.32–43), use `make install LEGACY=1`.
The legacy JavaScript and metadata are preserved in `legacy/`, since GNOME 45's
module format cannot load on older versions. GNOME 44 is not supported by this tree.

Enable the extensions from [GNOME Extensions App](https://gitlab.gnome.org/GNOME/gnome-shell/-/tree/main/subprojects/extensions-app).

### Gnome shell versions compatible
* Modern implementation: 45, 46, 47, 48, 49, 50, 51.
* Legacy implementation: 3.32, 3.34, 3.36, 3.38, 40, 41, 42, 43 (previously declared support).
* Loading validated in an isolated GNOME Shell 51.1 session. Audio switching and GNOME 45–50 still need runtime validation.

### Notes:
* May conflict with extensions which modify volume menu.
* Extension works with Volume Mixer extension. Restart shell, if errors encountered.

### [Change log](CHANGELOG.md)

