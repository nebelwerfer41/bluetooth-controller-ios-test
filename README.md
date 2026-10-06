[Catalog](https://nebelwerfer41.github.io/) · [Repository](https://github.com/nebelwerfer41/bluetooth-controller-ios-test)

# Bluetooth HID Tester

Log keyboard, mouse, pointer, and gamepad events exposed by the browser. A test page for iOS devices.

## Usage

Connect the device through the operating system, open the page, and activate the test. Move the controls and inspect the log. Available events depend on the device, operating system, and browser. The page does not use Web Bluetooth or perform pairing.

## Local setup

Serve the folder with a static server and open the local address in a browser:

```sh
python3 -m http.server 8000 --bind 127.0.0.1
```

No build step is required. A single HTML file with embedded CSS and JavaScript.

## Limitations

The repository name describes the test context. The page observes browser input APIs and does not guarantee compatibility with every Bluetooth controller or iOS version. The log retains at most 150 lines.

## License

[MIT](LICENSE). Copies and derivative works must retain the copyright notice and license text. Dependencies and third-party materials retain their own licenses.
