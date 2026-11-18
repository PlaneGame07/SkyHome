# SkyHome

A landscape tablet dashboard for **Android Only**. It shows the weather for your location, live aircraft within a chosen radius, airports on a map, and airport weather.

**For recreational use and situational awareness only.** SkyHome must not be used for navigation, flight planning or any tactical decision. Nothing in it is checked against official aviation or weather sources.

## Features

- Current weather, hourly and 7 day forecast, with a choice of forecast models
- Live planes within your chosen radius, with a card showing route, aircraft, altitude, speed and airline
- Airports on the Sky map, with raw or plain English weather and a photo
- Plane logbook grouped by aircraft family
- Three themes (Classic, Black, White), and Liquid Glass styles
- Standby clock mode

## In App Images

  <img width="640" alt="image" src="https://github.com/user-attachments/assets/4a665427-c185-4970-b48e-52c37a3aed66" />
  <img width="640" alt="image" src="https://github.com/user-attachments/assets/ad976c5e-664c-40d5-896d-72f8f631e51d" />
  <img width="640" alt="Home" src="https://github.com/user-attachments/assets/d94a01f4-8b65-4e74-a1f5-348e9c8025fd" />
  <img width="640" alt="SkyMap" src="https://github.com/user-attachments/assets/48301ea3-758f-4ba7-9369-538d0b0631a2" />
  <img width="640" alt="Plane Card" src="https://github.com/user-attachments/assets/a30cbfde-79bd-447d-913c-91cdf4fcf64c" />
  <img width="640" alt="Logbook" src="https://github.com/user-attachments/assets/ff669a16-0c2e-4053-95b7-85ead2cb486e" />


# SkyHome

Tablet dashboard for weather, nearby planes and airports. Built with Claude.

## Install

Go to here --> https://github.com/PlaneGame07/SkyHome/releases/
Download the latest APK from the **Releases** page and install it on an Android tablet. Android will warn that the app is from an unknown source. That's normal for apps installed outside the Play Store.

## Build it yourself

1. Install Node.js and Android Studio.
2. Make a folder, copy the contents of `app/` into a subfolder called `www`.
3. In that folder run:

```
npm init -y
npm install @capacitor/core @capacitor/android
npm install -D @capacitor/cli
npx cap init SkyHome com.skyhome.app --web-dir www
npx cap add android
npx cap sync
npx cap open android
```

4. In Android Studio, go to **Build → Build APK(s)**.

## Map key (Optional)

The map uses OpenStreetMap by default. For a sharper dark map, get a free key from CARTO and paste it into Settings under Map key.

## Tips for plane data

Keep the check interval at 2 seconds or slower. The plane sources are free volunteer networks.

## Good to know

If you happen to find any issues let me know 
https://github.com/PlaneGame07/SkyHome/issues

Let me know what you would like to see next!
https://github.com/PlaneGame07/SkyHome/discussions/1

## Credits

- Weather: [Open-Meteo](https://open-meteo.com)
- Maps: [OpenStreetMap](https://www.openstreetmap.org/copyright) contributors, [CARTO](https://carto.com) (optional key)
- Aircraft photos: [Planespotters.net](https://www.planespotters.net) and [Airport-Data.com](https://www.airport-data.com) photographers
- Airport and aircraft type photos: [Wikipedia](https://www.wikipedia.org) and [Wikimedia Commons](https://commons.wikimedia.org) contributors
- Flight data: [adsb.lol](https://adsb.lol), [adsbdb](https://www.adsbdb.com), [AviationWeather.gov](https://aviationweather.gov)
- Airport list: [OurAirports](https://ourairports.com)

## Privacy

SkyHome has no server and collects nothing. Your approximate location is sent to the services above so they can return local weather, nearby aircraft and map tiles.

## Licence

MIT. See [LICENSE](LICENSE).
