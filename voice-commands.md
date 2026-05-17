---
layout: default
title: Voice Commands
permalink: /voice-commands
description: Siri phrases StationCast supports — temperature, rain, wind, humidity, pressure, UV, sunrise, sunset, and a full weather summary.
---

# Voice Commands

<p class="page-meta">Ask Siri about your saved stations on iOS</p>

StationCast registers Siri shortcuts for each metric your saved stations report. Phrases include "in StationCast" because Siri uses the app name to route the request — without it, Siri may hand the question to its own weather source instead.

By default each command answers about the station you've labeled **Home**. If no station is labeled Home, StationCast falls back to the first station in your saved list. You can also wire a specific station into a Shortcut from the iOS Shortcuts app.

## Full weather report

- "Hey Siri, what's the weather in StationCast?"
- "Hey Siri, give me a weather report from StationCast."

Speaks a multi-sentence summary: current temperature and conditions, wind (with gusts), dew point and humidity, today's rainfall, pressure trend, the next sunrise or sunset, and the daily high and low so far.

## Temperature

- "Hey Siri, what's the temperature in StationCast?"
- "Hey Siri, check the temperature in StationCast."

## Is it raining?

- "Hey Siri, is it raining in StationCast?"
- "Hey Siri, how much rain has there been in StationCast?"
- "Hey Siri, check the rain in StationCast."

Reports the current rate when it's raining ("raining at Home at 0.12 inches per hour") and otherwise frames the answer around the daily total ("not raining at Home right now — 0.31 inches today").

## Wind

- "Hey Siri, how windy is it in StationCast?"
- "Hey Siri, what's the wind in StationCast?"
- "Hey Siri, check the wind in StationCast."

Includes the direction, and adds a gust clause when gusts exceed the sustained speed.

## Humidity

- "Hey Siri, how humid is it in StationCast?"
- "Hey Siri, what's the humidity in StationCast?"
- "Hey Siri, what's the dew point in StationCast?"

Reports the relative humidity together with the dew point.

## Pressure

- "Hey Siri, what's the pressure in StationCast?"
- "Hey Siri, is the pressure rising in StationCast?"
- "Hey Siri, check the barometer in StationCast."

Reports the current pressure and whether it's rising, falling, or steady.

## UV index

- "Hey Siri, what's the UV index in StationCast?"
- "Hey Siri, check the UV in StationCast."

Speaks the index plus a risk word (low, moderate, high, very high, extreme). At night, or when the station doesn't report UV, the command declines rather than reading a misleading value.

## Sunrise

- "Hey Siri, what time is sunrise in StationCast?"
- "Hey Siri, when does the sun come up in StationCast?"
- "Hey Siri, when is sunrise in StationCast?"

## Sunset

- "Hey Siri, what time is sunset in StationCast?"
- "Hey Siri, how long until sunset in StationCast?"
- "Hey Siri, when does the sun set in StationCast?"

The sunrise and sunset commands switch phrasing based on proximity: when the next event is within a few hours, you'll hear both a duration and a clock time ("Sunrise at Home is in 2 hours and 15 minutes, at 5:42 AM"). If it's further off, you'll just hear the clock time. If sunrise or sunset happened in the last hour, you'll hear how long ago it was instead.

## Tips

- The first time you use a phrase, iOS may ask you to confirm StationCast can handle it. Tap **Allow**.
- You can drop the "Hey Siri" if your phone is unlocked and you're holding the side button.
- These commands all read from your most recently fetched observation. If you've been offline or the app hasn't run in a while, the answer is based on the freshest data StationCast was able to retrieve.
