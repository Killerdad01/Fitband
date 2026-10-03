# Build and install FitBand APK without Android Studio

## Option A — GitHub Actions (recommended if Android Studio does not work)

1. Create a GitHub account if you do not already have one.
2. Create a new repository, for example `FitBandApp`.
3. Upload all files and folders from this project into the repository. Make sure `.github/workflows/build-apk.yml` is included.
4. Open the repository's **Actions** tab.
5. Select **Build FitBand APK**.
6. Click **Run workflow**.
7. When the workflow finishes, open the completed workflow run.
8. Under **Artifacts**, download `FitBand-debug-apk`.
9. Extract the downloaded artifact and find `app-debug.apk`.
10. Send `app-debug.apk` to your Android phone.
11. On the phone, open the APK and allow installation from that source when Android asks.
12. Install and open **FitBand**.

## Option B — Android phone

If you do not want to use a PC, an Android IDE/build environment can also compile the project on the phone, but GitHub Actions is usually easier for a first build.

## Important

This APK is the current prototype. It contains the fitness interface, BMI/weight tracking and adaptive workout logic. The actual Mi Band 3 BLE protocol/data synchronization still needs to be implemented before the app can read the band's real heart rate, steps, sleep, calories and distance.
