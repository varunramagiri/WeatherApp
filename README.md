# 🌤️ WeatherApp (iOS)

A simple and elegant **iOS Weather App** built using **SwiftUI**, **Combine**, and a public **Weather API**.  
Displays real-time weather data with temperature, condition icons, and location-based updates.

---

## ✨ Features
- 🌦️ Fetches live weather data via REST API (e.g., OpenWeatherMap)
- 📍 Location-based weather detection
- 🌡️ Displays temperature, weather condition (sunny, cloudy, rainy, etc.), and humidity
- 🌓 Supports light and dark mode
- 🧭 Built using SwiftUI for a modern, responsive design
- ⚡ Uses `async/await` or Combine for asynchronous data loading
- 🚨 Includes error handling for network or API issues

---

## 🧰 Tech Stack
| Category        | Tools / Frameworks                          |
|-----------------|---------------------------------------------|
| **Language**    | Swift                                       |
| **Framework**   | SwiftUI, Combine                            |
| **Networking**  | URLSession / AsyncImage                     |
| **Architecture**| MVVM (Model-View-ViewModel)                 |
| **IDE**         | Xcode                                       |
| **API Source**  | [OpenWeatherMap API](https://openweathermap.org/api) |

## 🗂️ Project Structure
WeatherApp/
├── WeatherAppApp.swift # App entry point
├── Models/
│ ├── WeatherModel.swift # Data model for weather info
│ ├── APIResponse.swift # Codable structs for decoding JSON
├── ViewModels/
│ └── WeatherViewModel.swift # Handles API calls and data binding
├── Views/
│ ├── ContentView.swift # Main view showing weather info
│ ├── WeatherRow.swift # Component for daily/hourly weather
│ └── ErrorView.swift # Error handling / retry view
├── Services/
│ └── WeatherService.swift # API call logic using URLSession
├── Assets.xcassets/ # App icons & design assets
├── Info.plist # Permissions (Location, API config)
└── README.md
