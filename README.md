# Databar

Databar shows your daily mobile data in the notification panel, all day, and warns you before it runs out.

## Why it is useful

Many people finish their daily 1.5 GB by evening and have nothing left for the night. Databar fixes that.

- **Always visible.** A notification stays in your panel: "Used 1.12 GB of 1.50 GB" with a progress bar. You do not need to open the app.
- **Night reserve.** You choose a reserve, for example 200 MB. When only the reserve is left, Databar sends an alert, so you can keep it for maps, UPI and calls.
- **Real usage.** It reads your phone's own mobile data meter. You do not type or paste anything.
- **Daily reset.** The count starts again at midnight, like your daily quota.
- **SIM choice.** On a dual SIM phone, pick your Jio SIM in settings. Databar counts data only while that SIM is the one set for mobile data. It picks a Jio SIM for you when it finds one.
- **Any plan.** Search your recharge by price, data or days, or type your own numbers. The daily data is not fixed at 1.5 GB.
- **Plan expiry.** The app shows how many days are left on your plan.
- **Restarts itself.** Monitoring starts again after the phone restarts.

## How to use it

1. Install the app (see below) and open it.
2. Tap **Allow usage access** and switch Databar on. This is how it reads your data. Allow notifications when asked.
3. Tap the small circle at the top right (settings).
4. Under **SIM**, tap **Allow SIM access** and choose your Jio SIM.
5. Search your plan, for example `299` or `84`, and tap it. Check the price, data per day and days.
6. Set your night reserve (default 200 MB) and tap **Save plan**.
7. Look at the notification panel. Databar now updates it every minute.

At the bottom of the main screen, **Check with Jio** has two buttons: **Refresh now** and **Open MyJio**. Compare the numbers once, because Jio can count slightly differently from your phone.

## How to get the app (no computer needed)

1. Create a free account on github.com.
2. Create a new repository named `databar`.
3. Upload `databar.zip` with **Add file, Upload files**. Do not unzip it.
4. Create the file `.github/workflows/build.yml` with **Add file, Create new file**, and paste in the contents of `build-from-zip.yml`. Commit it.
5. Open the **Actions** tab and wait for a green tick (about 5 minutes).
6. Open that run, download **Databar-apk**, unzip it, and install `app-debug.apk`.

## Good to know

- Needs Android 10 or newer.
- Android has no per-SIM data meter for apps, so Databar counts new data only while your chosen SIM is the mobile data SIM. If you switch the data SIM during the day, the count is approximate.
- It counts all mobile data on the phone, including hotspot use. Wi-Fi is not counted.
- It reads data used since midnight, so it matches a daily quota.
- Android may stop background apps on some phones. If the notification disappears, allow Databar to run without battery limits in phone settings.
- Your data stays on your phone. The app has no internet permission and sends nothing anywhere.
