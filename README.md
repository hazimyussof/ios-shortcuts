# ios-shortcuts

- [Smart Timer](#SmartTimer) ( [Link](https://routinehub.co/shortcut/18948/) )

---

## [Smart Timer](https://routinehub.co/shortcut/18948/)

**Smart Timer** is an intuitive iOS shortcut app designed to simplify the way you manage your time, it extends the features of the default iOS timer. Inspired by the powerful timer functionalities found in the macOS app called ["Smart Countdown Timer" by FIPLAB](https://itunes.apple.com/us/app/smart-countdown-timer/id1410709951?mt=12), this Smart Timer iOS shortcut brings the same level of efficiency and convenience to your iPhone and iPad.

### Features

- **Specific Time Calculation:** Input a specific time, and Smart Timer will accurately calculate and create a timer counting down to that exact moment. For example, if you input `15:00` or `3pm`, the timer will be set to expire precisely at 15:00/3pm. _(This will work for both the 24-hour and 12-hour formats)_
- **Natural Language Input:** Set timers effortlessly by typing commands like `1h 30m 30s` or `1 hour 30 minutes 30 seconds`. Smart Timer understands your input and translates it into precise timer settings. _(This will work with multiple combinations and sequences)_

### How to use

When starting the shortcut, it will promt and ask you for an input in the form of a text:

![demo1150](https://github.com/hazimyussof/ios-shortcuts/assets/56122446/3963a3ea-5d04-4def-800f-b373e86d275b)

**Specific time countdown (24-hour)**:

- This will only work if you type in the full format: `00:00`
- `18:00` ✅
- `18`, `18:`, `18:0` ❌

**Specific time countdown (12-hour)**:

- This will only work if you type `am` or `pm` at the end of the number. It is not case-sensitive, and it doesn't matter if there are whitespaces in-between as long as `am` or `pm` is added at the end.
- `6pm`, `6:30 PM` ✅

Specific time countdowns will only work after the current time, and before `00:00` or `12:00am` because the calculations only calculate for the `currentDate` and not for the date after.

**Timer countdown**:

- The following prefixes will work:
- Hour: `h`, `hr`, `hour`, `hours`
- Minute: `m`, `min`, `minute`, `minutes`
- Second: `s`, `sec`, `second`, `seconds`

it's not case-sensitive and will work with multiple combinations and sequences, example: `1h 30 minutes 59SEC`, `50s 1hour 30min`. It will not work if the timer is more than `23 hours 59 minutes 59 seconds` as that's the maximum time allowed by the default iOS timer.

---

# License

[MIT License](LICENSE.md)

Copyright (c) 2024 Hazim Yussof
