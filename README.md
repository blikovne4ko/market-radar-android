# Market Radar (Android)

Android app for monitoring stocks and crypto with **smart watchlists**, **portfolio P&L tracking**, **market heatmaps**, and **news sentiment**, plus on-device **price/volume alerts**.

## ✨ Features
- 📋 **Smart Watchlists** – group tickers by theme, sector, or exchange
- 💼 **Portfolio & P&L** – multiple portfolios, realized/unrealized gains, fees
- 🔥 **Heatmaps** – stocks & crypto by performance, volume, or volatility
- 📰 **News & Sentiment** – aggregated headlines with basic sentiment scoring
- 🔔 **Alerts** – price crosses, % change, volume spikes (local notifications)
- 🧩 **Widgets** – watchlist/portfolio widgets for the home screen
- 🌓 **Light/Dark** themes and dynamic color (Material You)

## 🛠 Tech Stack
- **Language:** Kotlin
- **UI:** Jetpack Compose, Material 3
- **Architecture:** MVVM + Coroutines + Flow, Clean-ish layers
- **DI:** Hilt
- **Networking:** Retrofit/OkHttp + WebSocket for live streams
- **Caching:** Room + DataStore (preferences)
- **Background:** WorkManager for periodic refresh
- **Images:** Coil
- **Quality:** Detekt, Ktlint, JUnit + Turbine

## 🚀 Getting Started

### Prerequisites
- Android Studio **Koala** (or newer)
- JDK **17**
- Gradle **8.x**
- API keys for your data providers (e.g., `STOCKS_API_KEY`, `CRYPTO_API_KEY`)

### Clone & Build
```bash
git clone https://github.com/<your-username>/market-radar-android.git
cd market-radar-android
# (optional) create local.properties or .env style file for keys
./gradlew assembleDebug
