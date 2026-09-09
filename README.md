# Super Converter — minimal Android prototype

This is deliberately tiny: a local WebView containing HTML/JavaScript and a cloud
GitHub Actions build.

The current screen is only a proof of concept:

- numeric keypad
- decimal point
- Backspace
- Clear
- recalculation after every press
- `2 + 2 = 4` as the initial calculation

No Internet permission is requested and no external web resources are used.

## Cloud build

1. Create a new GitHub repository.
2. Upload the contents of this directory.
3. Push to `main`, or use **Actions → Build APK → Run workflow**.
4. Open the completed workflow run.
5. Download the `super-converter-debug` artifact.
6. The artifact contains `app-debug.apk`.

The next step is to replace `app/src/main/assets/index.html` with the
small, local version of `cvt.htm`.
