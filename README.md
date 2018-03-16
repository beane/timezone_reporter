## Usage
```bash
times --now --tz America/New_York,America/Chicago,America/Los_Angeles
```

```bash
times --at '2pm' --in 'new york' --tz America/New_York,America/Chicago,America/Los_Angeles
```

## TODO
- good flag names and abilities
- helpful region checks (scan in /usr/share/zoneinfo/)
- fixed-width pretty table formatting (printf)
- good date and time zone parsing (use `date` under the hood?)
- work on Mac OS and Debian
- maybe csv output style?
