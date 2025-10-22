# WeatherApp (iOS)

A simple and elegant **iOS Weather App** built using **SwiftUI**, **Combine**, and a public **Weather API**.  
Displays real-time weather data with temperature, condition icons, and location-based updates.

---

## ✨ Features
- Fetches live weather data via REST API (e.g., OpenWeatherMap)
- Location-based weather detection
- Displays temperature, condition (sunny, cloudy, rainy, etc.), and humidity
- Responsive layout supporting both light and dark mode
- SwiftUI-based modern interface
- Uses `async/await` or Combine for asynchronous data loading
- Error handling for invalid API responses or network issues

---

## 🧰 Tech Stack
**Language:** Swift  
**Framework:** SwiftUI, Combine  
**Networking:** URLSession / AsyncImage  
**Architecture:** MVVM (Model-View-ViewModel)  
**IDE:** Xcode  
**API Source:** OpenWeatherMap API or similar

---

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

🧠 What I Learned

- Working with REST APIs in Swift
- Using Combine / async-await for reactive data handling
- Implementing MVVM architecture
- Designing adaptive layouts with SwiftUI
