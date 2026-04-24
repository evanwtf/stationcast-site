---
layout: default
title: FAQ
permalink: /faq
description: Frequently asked questions about StationCast — weather icons, data sources, location access, and more.
---

# Frequently Asked Questions

<p class="page-meta">How StationCast works</p>

## What do the weather condition icons mean?

StationCast derives conditions from the station's own sensor readings — not from a weather service's classification. The possible conditions are:

- **Clear** — no precipitation, calm wind, and good solar radiation during the day
- **Partly Cloudy** — reduced solar radiation suggesting partial cloud cover
- **Overcast** — minimal solar radiation at a time when the sun should be strong
- **Drizzle** — very light precipitation detected by the rain gauge
- **Rain** — measurable precipitation
- **Windy** — wind speed is above a significant threshold, even if skies are otherwise clear

At night, the condition icon is replaced by the current **lunar phase** — you may see a crescent, quarter, gibbous, or full moon, whichever is accurate for that night.

## Why does the moon look different shapes?

StationCast calculates the exact lunar phase from the date and time, so the icon reflects reality: waxing crescent, first quarter, waxing gibbous, full moon, waning gibbous, last quarter, or waning crescent. It is not a generic moon icon.

## What does the clock icon next to the timestamp mean?

The clock indicates that the station's last reading is getting old — roughly 15 minutes or more. Once data is over an hour old, the readings fade visually to make it clear you may not be seeing current conditions. The station is still shown, but StationCast won't pretend stale data is fresh.

## Where does the weather data come from?

All data comes from personal weather stations — privately owned instruments operated by individuals and organizations. These are backyard sensors, rooftop stations, harbor monitors, and the like, with owners who opt in to sharing their readings publicly.

## What is a personal weather station?

A personal weather station is a privately owned set of weather instruments — typically a combined sensor for temperature, humidity, wind, rain, pressure, and sometimes UV and solar radiation. Owners install them at their homes, farms, boats, and other locations and opt in to sharing readings publicly. Because they are locally sited, they often give a more accurate picture of conditions at a specific place than the nearest official airport or government sensor. [Here's an example of one.](https://amzn.to/41TabvG)

## Is this a forecast app?

No. StationCast is designed to tell you what conditions are actually like at a specific place, right now — not what a model thinks they might be later. Every reading was measured by a real sensor at that location. There are no forecasts, no model blends, and no estimates.

The daily high and low labeled **today so far** are the observed maximum and minimum since midnight — not a predicted range. If you want to know what it feels like outside your front door, StationCast gets you as close to that as possible in real time.

## What does "feels like" mean?

Feels like is wind chill (when it's cold and windy) or heat index (when it's hot and humid), calculated from the station's own temperature, humidity, and wind readings. It is derived entirely from what that specific station measured — not from a regional weather service.

## Why don't I see UV or solar data for some stations?

Not all personal weather stations include UV or solar radiation sensors. When a station doesn't report those values, StationCast omits those tiles entirely rather than showing a blank or a dash. You only see data the station actually measured. Those tiles are also hidden at night, when solar readings aren't meaningful.

## Why does the app ask for my location?

Location access is entirely optional — the app is fully functional without it. When you grant access, it's used only for convenience features: sorting nearby stations by distance and showing how far each one is from you. If you decline, you can still search for and add any station manually; you just won't see distance information or proximity-based sorting.

You can change location permissions at any time in **Settings → Privacy & Security → Location Services → StationCast**.

## How do I add a station?

Open **Settings** (the gear icon) and tap **Manage Stations**. From there you can search by station ID or use your location to find nearby stations to add to your list.

## Something looks wrong — how do I report it?

Email **[evandhoffman@gmail.com](mailto:evandhoffman@gmail.com)** with the station ID and a description of what you're seeing. Include your iOS version if you can.
