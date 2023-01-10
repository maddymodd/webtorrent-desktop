<h1 align="center">
  <br>
  <a href="https://webtorrent.io">
    <img src="https://webtorrent.io/img/WebTorrent.png" alt="WebTorrent" width="200">
  </a>
  <br>
  WebTorrent Desktop with Speed Limits
  <br>
  <br>
</h1>

<h4 align="center">WebTorrent Desktop, the streaming torrent client, with speed limits.</h4>

## Download

- Download specific installer files from the [GitHub releases](https://github.com/webtorrent/webtorrent-desktop/releases) page.

## Screenshots

<p align="center">
  <img width="953" alt="scr1" src="https://user-images.githubusercontent.com/121954045/211557899-c72be231-d691-42cb-a71e-bbb2bd6a989d.png" align="center">
  <img width="396" alt="speedlimits" src="https://user-images.githubusercontent.com/121954045/211557989-910671dd-360c-4951-b3aa-286e031f98e6.png" align="center">
</p>

## How to Contribute

### Get the code

```
$ git clone https://github.com/maddymodd/webtorrent-desktop-with-speed-limits
$ cd webtorrent-desktop-with-speed-limits
$ npm install
```

### Run the app

```
$ npm start
```

### Watch the code

Restart the app automatically every time code changes. Useful during development.

```
$ npm run watch
```

### Run linters

```
$ npm test
```

### Package the app

Builds app binaries for Mac, Linux, and Windows.

```
$ npm run package
```

To build for one platform:

```
$ npm run package -- [platform] [options]
```

Where `[platform]` is `darwin`, `linux`, `win32`, or `all` (default).

The following optional arguments are available:

- `--sign` - Sign the application (Mac, Windows)
- `--package=[type]` - Package single output type.
   - `deb` - Debian package
   - `rpm` - RedHat package
   - `zip` - Linux zip file
   - `dmg` - Mac disk image
   - `exe` - Windows installer
   - `portable` - Windows portable app
   - `all` - All platforms (default)

Note: Even with the `--package` option, the auto-update files (.nupkg for Windows,
-darwin.zip for Mac) will always be produced.

#### Windows build notes

The Windows app can be packaged from **any** platform.

Note: Windows code signing only works from **Windows**, for now.

Note: To package the Windows app from non-Windows platforms,
[Wine](https://www.winehq.org/) and [Mono](https://www.mono-project.com/) need
to be installed. For example on Mac, first install
[XQuartz](http://www.xquartz.org/), then run:

```
$ brew install wine mono
```

(Requires the [Homebrew](http://brew.sh/) package manager.)

#### Mac build notes

The Mac app can only be packaged from **macOS**.

#### Linux build notes

The Linux app can be packaged from **any** platform.

If packaging from Mac, install system dependencies with Homebrew by running:

```
npm run install-system-deps
```

### Privacy

WebTorrent Desktop collects some basic usage stats to help us make the app better.
For example, we track how well the play button works. How often does it succeed?
Time out? Show a missing codec error?

The app never sends any personally identifying information, nor does it track which
torrents you add.

## License

MIT License: https://github.com/maddymodd/webtorrent-desktop-with-speed-limits/blob/master/LICENSE
