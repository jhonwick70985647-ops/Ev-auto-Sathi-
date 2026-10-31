# EV Auto Saathi

A phone-friendly starter app for one EV auto driver.

## Run on Android
1. Extract this ZIP.
2. Put the folder on a simple HTTPS static host (or run locally with a web server).
3. Open `index.html` in Chrome. For PWA installation, open the hosted HTTPS page, Chrome menu ⋮ → **Add to Home screen** / **Install app**.
4. In Settings, enter the driver's UPI ID and payee name, then set the daily goal and incentive.
5. Use Add trip to record each fare and expenses.

## Features
- Daily and all-time fare, expense, net and trip totals
- Editable daily goal and incentive threshold
- UPI payment QR with optional fixed amount
- Trip and expense activity log
- CSV export and JSON backup
- Local browser storage

## Important limitations
- The QR code creates a UPI payment request only. It does not verify that money arrived. Check the driver's UPI/bank app before treating a payment as received.
- Records remain on this device/browser. There is no cloud sync, multi-driver admin panel, automated GPS tracking, or automatic bank/UPI transaction import.
- QR rendering uses a small QRCode.js library loaded from a CDN, so internet is needed when generating the QR.
- Incentives are calculated and displayed only; the app does not transfer or pay incentive money.

This is a starter web app, not a signed Android APK. A native APK build needs an Android wrapper/build environment and signing.
