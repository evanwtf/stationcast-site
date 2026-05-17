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

Wire this one up yourself from the Shortcuts app — the **Get Humidity** action is registered, but the spoken phrase isn't pre-bound to keep the suggestion list within Apple's recommended size. The full weather summary always reports humidity and dew point.

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

Always answers about the **next** sunrise, dated — for example, *"Sunrise at Home on May 16 is at 5:42 AM."* If today's sunrise has already happened, you'll get tomorrow's instead.

To ask about the most recent sunrise:

- "Hey Siri, when was sunrise in StationCast?"
- "Hey Siri, what time was sunrise in StationCast?"
- "Hey Siri, when did the sun come up in StationCast?"

Answers with a "today" or "yesterday" qualifier — *"Sunrise at Home today was at 5:42 AM."*

## Sunset

- "Hey Siri, what time is sunset in StationCast?"
- "Hey Siri, how long until sunset in StationCast?"
- "Hey Siri, when does the sun set in StationCast?"

Always answers about the **next** sunset, dated — for example, *"Sunset at Home on May 16 is at 8:00 PM."* If today's sunset has already happened, you'll get tomorrow's instead.

To ask about the most recent sunset:

- "Hey Siri, when was sunset in StationCast?"
- "Hey Siri, what time was sunset in StationCast?"
- "Hey Siri, when did the sun go down in StationCast?"

Answers with a "today" or "yesterday" qualifier — *"Sunset at Home today was at 8:00 PM."*

## How fresh is the reading?

Every metric reply (temperature, rain, wind, humidity, pressure, UV) carries an *"as of N ago"* clause when the reading isn't brand-new — for example, *"Temperature at Home is 62 degrees Fahrenheit, partly cloudy, as of 32 minutes ago."* If the observation is less than a minute old, the clause is omitted so the answer stays terse. Sunrise and sunset are computed from solar geometry, so they don't carry a freshness clause.

## Tips

- The first time you use a phrase, iOS may ask you to confirm StationCast can handle it. Tap **Allow**.
- You can drop the "Hey Siri" if your phone is unlocked and you're holding the side button.
- These commands all read from your most recently fetched observation. If you've been offline or the app hasn't run in a while, the answer is based on the freshest data StationCast was able to retrieve.
