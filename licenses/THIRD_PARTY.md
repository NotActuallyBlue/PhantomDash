# Third-party software and fonts in PhantomDash

PhantomDash is built on the open-source work below, used under the licences named. The notices are kept here as those licences require, and must stay with
every copy of the firmware or its source that is handed out (on the product's page and, for a device, in an About or licence screen).

| Part | Used for | Licence |
|---|---|---|
| [LVGL](https://github.com/lvgl/lvgl) 9.2 | the user interface | MIT, text below |
| [QR Code generator library](https://www.nayuki.io/page/qr-code-generator-library) by Project Nayuki, bundled in LVGL | the QR codes on the download and update screens | MIT, text below |
| stb_truetype (bundled in LVGL's tiny_ttf) | drawing the TrueType fonts | public domain / MIT |
| [Fira Sans](https://github.com/mozilla/Fira) (Mozilla, Telefonica, Carrois Corporate, bBox Type) | all text, and the italic numbers | SIL Open Font License 1.1, `licenses/FiraSans-OFL.txt` |
| [DSEG](https://github.com/keshikan/DSEG) 7-segment fonts by keshikan | the digital numbers | SIL Open Font License 1.1, `licenses/DSEG-OFL.txt` |
| [ESP-IDF](https://github.com/espressif/esp-idf) by Espressif Systems and the components it includes (FreeRTOS, lwIP, mbed TLS and others) | the firmware platform | mostly Apache 2.0, see [its licence page](https://github.com/espressif/esp-idf/blob/master/LICENSE) |

The fonts are embedded in the firmware as data (`firmware/dash/src/font_*.c`, generated from the files in `firmware/dash/fonts/`). The OFL does not allow
selling the fonts by themselves, and does allow bundling them with software; the licence texts above travel with them.

## LVGL

```
MIT licence
Copyright (c) 2021 LVGL Kft

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

## QR Code generator library (Project Nayuki)

```
QR Code generator library (C)

Copyright (c) Project Nayuki. (MIT License)
https://www.nayuki.io/page/qr-code-generator-library

Permission is hereby granted, free of charge, to any person obtaining a copy of
this software and associated documentation files (the "Software"), to deal in
the Software without restriction, including without limitation the rights to
use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
the Software, and to permit persons to whom the Software is furnished to do so,
subject to the following conditions:
- The above copyright notice and this permission notice shall be included in
  all copies or substantial portions of the Software.
- The Software is provided "as is", without warranty of any kind, express or
  implied, including but not limited to the warranties of merchantability,
  fitness for a particular purpose and noninfringement. In no event shall the
  authors or copyright holders be liable for any claim, damages or other
  liability, whether in an action of contract, tort or otherwise, arising from,
  out of or in connection with the Software or the use or other dealings in the
  Software.
```
