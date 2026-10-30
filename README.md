# Download-Music

A music downloader with streaming downloads and local persistence.

## Highlights

- Streaming downloads with `dio`, with progress reported to the user.
- Files written to local storage through `path_provider`.
- Hive used for lightweight key-value persistence of app state.
- Runtime permissions handled for storage and network access.

## Tech Stack

| Concern | Choice |
|---|---|
| UI | Flutter, Material |
| State management | `provider` |
| Networking | `dio` |
| Persistence | `hive`, `hive_flutter` |
| Files | `path_provider` |
| Permissions | `permission_handler` |

## Project Structure

```
lib/
- `Services`
- `downloading_dialog.dart`
- `localization`
- `model`
- `provider`
- `screen`
- `widgets`
```

## Getting Started

### Prerequisites

- Flutter `>= 3.16` (Dart `>= 3.2`)

### Run

```bash
git clone https://github.com/developer-rahim/Download-Music.git
cd Download-Music
flutter pub get
flutter run
```

### Test

```bash
flutter test
flutter analyze
```

## Notes

Downloads land in the app's documents directory — not the shared music library — so no additional storage permission is needed on most Android versions.

## License

Released under the MIT License.
