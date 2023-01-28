# homey-log-to-file

Capture stdout/stderr of a Homey app and write it to a logfile (default: `/userdata/std.log`).

The logfile can be retrieved through an HTTP request to your Homey (default port: 8008)

## Usage

```
const LogToFile = require('homey-log-to-file');
...

class MyApp extends Homey.App {

  async onInit() {
    await LogToFile();
    ...
  }
}
```
