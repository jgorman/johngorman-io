---
layout: page
title: Darkest Night Clock
desc: A very dimmable night clock application written in both
      ReactJS and React Native that can be dimmed to almost black
      to avoid adding ambient light while sleeping.
permalink: /darkest-night-clock/
---

# Darkest Night Clock App

A very dimmable night clock web written in both React.js and React Native.

You can make the clock display quite dim in order to be readable
at night without adding much illumination to the room. Studies
have shown that ambient light at night can reduce sleep quality
and can also lead to nearsightedness due to the eyes constantly
attempting to focus while sleeping.

<br>
<iframe
  style="max-width: 600px; width: 100%; height: 200px; border: none"
  src="https://johngorman.io/darkest-night-clock/run/"
></iframe>
<br>

Click the clock time above to control color, brightness, seconds
and date display.

You can embed this clock in any page by dropping this code in.

```html
<iframe
  style="max-width: 600px; width: 100%; height: 200px; border: none"
  src="https://johngorman.io/darkest-night-clock/run/"
></iframe>
```

Here is the
<a href="https://johngorman.io/darkest-night-clock/run/" target="_blank">
full page</a> version.

Install on your [Android Phone](/darkest-night-clock.apk).

## Controls

- Adjust clock brightness by swiping left and right.
- Toggle control bar visibility by clicking on the time display.
- The plus (+) and minus (-) buttons also control the brightness.
- The color (*) button
  brings up the color selections.
- The seconds (:) button toggles seconds display.
- The date (/) button toggles date display.

## Technical Details

- Written in React.js and React Native with useReducer state management.
- The source code for Android and iOS:
   [Darkest Night Clock - React Native](https://github.com/jgorman/darkest-night-clock-react-native)
- The source code for the web app:
   [Darkest Night Clock - React.js](https://github.com/jgorman/darkest-night-clock-react-js)
- There is a lot of shared code between the two projects.
  - The main application logic in Clock.js is identical.
  - The appstate.js Redux reducer file is identical.
- A great way to see exactly how React.js and React Native differ.
- Both projects store the app preferences state between sessions.
