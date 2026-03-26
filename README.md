# SetTrack 💪

**The fastest way to log your gym workouts.**

SetTrack is a modern, no-nonsense workout tracker for iOS. Built for lifters who know their routine and just want to track progress — without the noise.

No accounts. No subscriptions. No complicated setup.  
Just open, log your sets, and get back to lifting.

## ✨ Features

### 🎯 Built For Speed
- **Minimal taps while training** - designed to be gym-friendly
- **Large, easy-to-hit buttons** - perfect when your hands are shaky
- **Works offline** - no internet connection required
- **No login needed** - your data stays on your device

### 📋 Simple Workout Logging
- Create your workouts once (Push, Pull, Legs, etc.)
- Log sets in seconds with reps and weight
- Edit on the fly during your workout
- Clean, distraction-free interface

### 🏋️ Exercise Tracking
- Track weight and reps for each set
- Support for kg and lbs
- Visual feedback with checkmarks when sets are completed
- View your workout history at a glance

### ⏱️ Smart Rest Timer
- Configurable rest timer between sets (30s - 180s)
- Per-set rest time adjustments
- Visual and haptic feedback
- Stay focused without watching the clock

### 💾 Privacy-First
- All data stored locally with SwiftData
- No account required
- No subscriptions
- No tracking or analytics
- Your workouts, your device, period.

## 🎯 Why SetTrack?

Most fitness apps try to do everything: meal tracking, AI coaches, social features, complicated workout plans.

**SetTrack focuses on one thing:** logging your sets quickly and clearly.

Perfect for:
- 💪 Strength training & bodybuilding
- 🏋️ Powerlifting
- 🔁 Anyone with a consistent gym routine
- 📊 Lifters who want to track progress without the noise

If you already know what exercises you're doing, SetTrack is the fastest way to log them.

## 🛠️ Technical Details

### Built With
- **SwiftUI** - Modern declarative UI framework
- **SwiftData** - Local data persistence
- **Swift 5.9+** - Latest Swift features
- **iOS 17.0+** - Minimum deployment target

### Architecture
- MVVM pattern with SwiftData models
- Reactive UI with `@Query` and `@Observable`
- Type-safe data modeling
- UserDefaults for app preferences

### Data Models
```swift
@Model
class Workout {
    var name: String
    var date: Date
    var exercises: [Exercise]
}

@Model
class Exercise {
    var name: String
    var sets: [ExerciseSet]
}

@Model
class ExerciseSet {
    var reps: Int
    var weight: Double?
    var restTimeAdjustment: Int?
}
```

## 📱 Screenshots

<!-- Add screenshots here when available -->

## 🚀 Getting Started

### Requirements
- Xcode 15.0 or later
- iOS 17.0 or later
- macOS Sonoma or later (for development)

### Installation

1. Clone the repository:
```bash
git clone https://github.com/marcoletics/settrack.git
cd settrack
```

2. Open the project in Xcode:
```bash
open SetTrack.xcodeproj
```

3. Build and run on your device or simulator (⌘R)

## 📖 Usage

### Creating a Workout
1. Tap the "+" button to create a new workout
2. Give your workout a name
3. Add exercises with the "Add Exercise" button
4. For each exercise, add sets with reps and optional weight

### During Your Workout
1. Check off sets as you complete them
2. Use the rest timer between sets
3. Adjust rest times per set if needed
4. Save your workout when done

### Viewing History
- All workouts are displayed in chronological order
- Tap any workout to view details
- Swipe to delete workouts you no longer need

## 🗺️ Roadmap

### Planned Features (v0.2.0+)
- [ ] **Previous workout values** - see your last performance automatically
- [ ] **Workout templates** - save your favorite routines for quick starts
- [ ] **Progress tracking** - charts and statistics to visualize strength gains
- [ ] **Exercise library** - searchable database with descriptions
- [ ] **Notes per workout** - track how you felt, energy levels, etc.
- [ ] **Export/import** - backup your data or move between devices
- [ ] **Apple Watch** - log sets from your wrist
- [ ] **iPad optimization** - enhanced layouts for larger screens

### What SetTrack Will NEVER Have
- ❌ Subscriptions or paywalls
- ❌ Meal tracking
- ❌ Social features
- ❌ Mandatory accounts
- ❌ Ads

## 🤝 Contributing

Contributions are welcome!

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Code Style
- Follow Swift API Design Guidelines
- Use SwiftLint for consistency (if configured)
- Write clear commit messages
- Add comments for complex logic

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**marcoletics**

- GitHub: [@marcoletics](https://github.com/marcoletics)

## 🙏 Acknowledgments

- Built with Apple's SwiftUI and SwiftData frameworks
- Icons and design inspired by Apple's Human Interface Guidelines
- Thanks to the iOS development community

## 📞 Support

For questions, feedback, or bug reports:
- Open an [issue](https://github.com/marcoletics/settrack/issues)
- Reach out via GitHub discussions

---

**Version:** 1.0.0  
**Last Updated:** March 2026

*Made with ❤️ for fitness enthusiasts*
