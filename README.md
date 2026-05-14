# sabaego

> 日本語のREADMEはこちらです: [README.ja.md](README.ja.md)

A location-based game for collaborative town exploration and issue reporting (codename: 鯖江GO). This project is a modification of [gsimaps](https://github.com/gsi-cyberjapan/gsimaps) by [Taisuke Fukuno](http://fukuno.jig.jp/1326).

## Features
- **Team-based Gameplay**: Organize teams with defined start/goal times and assigned exploration areas.
- **Live Location Tracking**: View the real-time map locations of your team members.
- **Issue Reporting**: Report local issues (`sabarepo`) and collect virtual items (e.g., cultural assets) as rewards.
- **Gamification**: A scoring system based on the number and type of items collected.
- **Mail-Posting Tools**:
    - Differentiate building types (e.g., apartment complexes, single-family homes).
    - Mark and identify "posting prohibited" areas.
    - Receive warnings for previously covered areas.
    - Use custom on-map buttons for data input (e.g., "Posting NG," "Hand-delivered," "Wealth Assessment").
    - Set up alerts for specific addresses, such as existing customers.

## Demos (Base Project)
As this is a modified fork, refer to the original `gsimaps` project for base functionality:
- **Official GSI Maps:** http://maps.gsi.go.jp/
- **GSI Maps (Repository Demo):** http://gsi-cyberjapan.github.io/gsimaps/

## Usage
1.  Download or clone this repository.
2.  Place the files onto a web server.
3.  Open `index.html` in a browser.

*Note: While many functions work when opening `index.html` from the local filesystem, a web server is required for full functionality, especially for handling vector tile data.*

## Dependencies
- Based on [GSI Maps](https://github.com/gsi-cyberjapan/gsimaps) (Geospatial Information Authority of Japan)
- [Leaflet](LICENSE_LIBRARIES.md)
- [jQuery 1.11.1](jquery/jquery-1.11.1.min.js) & [jQuery UI](jquery/jquery-ui.min.js)
- [ZeroClipboard 2.0.2](jquery/ZeroClipboard2.0.2/)

## External Services & APIs
- Utilizes a geocoding service from [CSIS, University of Tokyo](http://newspat.csis.u-tokyo.ac.jp/geocode/).
- **Disclaimer:** Server-side services are not guaranteed to be persistently in operation and may be updated or abandoned without prior notice.

## Related Tools (from gsimaps)
- [Layers Definition Editor](http://gsi-cyberjapan.github.io/gsimaps/config/config.html)
- [Layers Definition Specifications](https://github.com/gsi-cyberjapan/layers-dot-txt-spec)

## License
The original work by GSI is provided under a 2-clause BSD license. See [LICENSE](LICENSE) and [LICENSE_LIBRARIES.md](LICENSE_LIBRARIES.md).