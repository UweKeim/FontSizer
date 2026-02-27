# Font Sizer (Uwe Custom)

Public fork of [madskristensen/FontSizer](https://github.com/madskristensen/FontSizer) with an important behavior change for environment font sizing.

## Download

Install the latest VSIX from this repository's releases:

- [Latest release](https://github.com/UweKeim/FontSizer-UweCustom/releases/latest)
- Direct VSIX download (current):
  [FontSizer-UweCustom.vsix](https://github.com/UweKeim/FontSizer-UweCustom/releases/download/v1.1.0-uwecustom.1/FontSizer-UweCustom.vsix)

## What changed in this fork

- Added an options page in Visual Studio:
  `Tools > Options > Font Sizer (Uwe) > General`
- Added **Environment font step** setting.
- Default environment step is now **1** (instead of fixed **2**).
- Allowed range for environment step: **1..10**.
- The extension has its own VSIX identity, so it can be installed separately from the original extension.

## Features

Quickly change the editor font sizes or the Visual Studio environment font size.

![Tools menu](art/screenshot.png)

Recommended command shortcuts:

- CTRL + Num Pad Arrow Up = Increase editor font sizes
- CTRL + Num Pad Arrow Down = Decrease editor font sizes
- CTRL + Num Pad Arrow Right = Increase environment font size
- CTRL + Num Pad Arrow Left = Decrease environment font size

### Change Editor Font Size

Editor-related commands still use the same deltas as the original extension:

- TextEditor changes by 2
- StatementCompletion changes by 1
- TextOutputToolWindows changes by 1
- Tooltip changes by 1
- CodeLensCategory changes by 1

### Change Environment Font Size

Environment-related commands now use the configurable **Environment font step** value from options.

- Default: 1
- Min: 1
- Max: 10

## Credits

Originally based on [craigeddy/FontSizer](https://github.com/craigeddy/FontSizer), later updated by Mads Kristensen to support newer Visual Studio versions.

## License

[Apache 2.0](LICENSE)
