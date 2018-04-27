## Usage
```bash
whattime --now --display new_york,utc
# TZ=America/New_York date; TZ=Etc/UTC date
```

```bash
whattime --when '2pm' --here --display new_york
# TZ=America/New_York date -d 'TZ="/usr/share/zoneinfo/<your timezone>" 2pm'
```

```bash
whattime --when '2pm' --in 'new york' --display chicago
# TZ=America/Chicago date -d 'TZ="America/New_York" 2pm'
```

## TODO
- good flag names and abilities
- helpful region checks (scan in /usr/share/zoneinfo/)
- fixed-width pretty table formatting (printf)
- good date and time zone parsing (use `date` under the hood?)
  - check `info date`
  - maybe accept time offsets and map them to TZs?
- work on Mac OS and Debian
- maybe csv output style?

## Questions we want to answer:
- when it is 2pm in NY, what time is it here and LA
- what time is it in Taipei right now?
- when it is 2pm here, what time is it in Chicago?

Two different kinds of locations:
- where we fix the time `--where`
- location for which to display the time `--display`

## Helpful links:
- https://superuser.com/questions/164339/timezone-conversion-by-command-line/164354#164354
