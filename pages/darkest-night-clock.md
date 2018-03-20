---
layout: page
title: Darkest Night Clock
desc: A very dimmable night clock application written in both
      ReactJS and React Native that can be dimmed to almost black
      to avoid adding ambient light while sleeping.
permalink: /darkest-night-clock/
---

# Darkest Night Clock App

Too much light at night is sad.

A very dimmable night clock web written in both React.js and React Native.

You can make the clock display quite dim in order to be readable at night without adding much illumination to the room. Studies have shown that ambient light at night can reduce sleep quality and can also lead to nearsightedness due to the eyes constantly attempting to focus while sleeping.

Check out the __[Live demo](https://johngorman.io/darkest-night-clock/run)__

## Controls

- Toggle control bar visibility by clicking on the time display.
- The plus (+) and minus (-) buttons control the brightness.
- The color (*) button brings up a color selection bar.
- The seconds (:) button toggles seconds display.
- The date (/) button toggles date display.
- Double click on the time to see the version number.

## Technical Details

- Written in React.js with Redux state management.
- Co-written for Android and iOS as __[Darkest Night Clock - React Native](https://github.com/jgorman/darkest-night-clock-react-native)__!
- There is a lot of shared code between the two projects.
- The appstate.js Redux reducer file is identical between the two projects because the state flow is the same.
- A great pair of simple no frills projects for anyone who wants to see exactly how React.js and React Native differ and how to port between them.
- Both projects store the app preferences state between sessions.

Let me know if you have any comments or suggestions!