# Echo Sense

A Flutter-based voice analysis web application that performs voice authenticity checks, speech-to-text transcription, and keyword detection.

## Features

- **Audio Upload**: Upload audio files directly from your device
- **Voice Recording**: Record voice directly in the browser using your microphone
- **Voice Authenticity Check**: Analyzes audio to determine if the voice is "Real" or "Not Real"
- **Speech-to-Text**: Converts audio to text transcription
- **Keyword Detection**: Detects predefined keywords from the transcript
- **Keyword Management**: Add, edit, and remove keywords from your detection list

## Getting Started

### Prerequisites

- Flutter SDK (latest version)
- A web browser (Chrome, Firefox, Safari, or Edge)

### Installation

1. Clone the repository
2. Navigate to the project directory
3. Install dependencies:
```bash
flutter pub get
```

### Running the App

To run the app in your browser:

```bash
flutter run -d chrome
```

Or use any other web browser:
```bash
flutter run -d web-server
```

## Project Structure

```
lib/
├── main.dart                          # App entry point
├── theme.dart                         # App theme and styling
├── models/
│   └── analysis_result.dart          # Data model for analysis results
├── screens/
│   ├── home_screen.dart              # Main screen with upload/record options
│   ├── keywords_screen.dart          # Keyword management screen
│   └── results_screen.dart           # Analysis results display
├── services/
│   ├── keyword_service.dart          # Keyword management logic
│   └── voice_analysis_service.dart   # Voice analysis and transcription
└── widgets/
    ├── recording_section.dart        # Voice recording widget
    └── upload_section.dart           # File upload widget
```

## Usage

1. **Upload or Record Audio**:
   - Click "Upload Audio File" to select an audio file from your device
   - Or click "Record Voice" to record directly in the browser

2. **Manage Keywords**:
   - Navigate to the Keywords screen using the top-right icon
   - Add new keywords to detect in transcripts
   - Edit or delete existing keywords

3. **View Results**:
   - After analysis, view:
     - Voice authenticity status (Real/Not Real)
     - Full transcript
     - Detected keywords with match count

## Configuration

### App Name
- Display Name: **Echo Sense**
- Package Name: `com.echosense.app`

### Supported Platforms
- ✅ Web
- ✅ Android
- ✅ iOS

## Technologies Used

- **Flutter**: Cross-platform UI framework
- **Dart**: Programming language
- **Material Design**: UI/UX design system
- **file_picker**: Cross-platform file selection
- **shared_preferences**: Local data persistence

## Note

This is a **Proof of Concept** application. The voice analysis and speech-to-text features are currently simulated for demonstration purposes. For production use, integrate with:
- Real ML models for voice authenticity detection
- Actual speech-to-text APIs (Google Speech-to-Text, Azure Speech, etc.)
- Enhanced audio processing libraries

## License

This project is a proof of concept application.

## Contributing

This is a closed proof-of-concept project. For inquiries, please contact the project maintainer.
