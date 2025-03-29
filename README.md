# Google Logo Flutter 🎨📱

## Problem Statement 🚀
I was designing the UI for my mobile application, where I needed to use the Google "G" logo. However, the default icons provided by Flutter did not include an exact match. The closest option looked more like a search icon. After exploring the [Flutter Icons API](https://api.flutter.dev/flutter/material/Icons-class.html), I confirmed that there was no official Google/Gmail logo available.

### Initial Attempt ❌
I found an alternative solution by using the `font_awesome_flutter` package:

```dart
import 'package:font_awesome_flutter/font_awesome_flutter.dart';

Column(
  mainAxisAlignment: MainAxisAlignment.center,
  children: [
    // Google Icon
    FaIcon(
      FontAwesomeIcons.google,
      size: 60,
      color: Colors.red,
    ),
    SizedBox(height: 40),
    // Gmail Icon
    FaIcon(
      FontAwesomeIcons.envelope,
      size: 60,
      color: Colors.red,
    ),
  ],
)
```

### Output Image 📸
![Google Icon Output](https://github.com/Hifza-Khalid/google-logo-flutter/blob/main/screenshots/Google1.JPG)

However, I was not satisfied because:
1. The icon lacked the original gradient shades of the Google logo.
2. It didn't perfectly match Google's branding.

### Final Solution ✅
To get the exact Google "G" logo, I implemented it using `CustomPainter` in Flutter. This approach allowed me to accurately replicate the logo's shape, colors, and gradients.

#### Implementation 🧐
I used `CustomPainter` to draw the Google "G" logo with precise color shading and arc rendering. Check out the code in this repository for the full implementation!

## Features 🎨
- Draws the Google "G" logo accurately.
- Uses `CustomPainter` for custom drawing.
- Provides flexibility to adjust size and colors.
- Does not rely on external icon libraries.

## How to Run 🏃‍♂️
1. Clone the repository:
   ```sh
   git clone https://github.com/Hifza-Khalid/google-logo-flutter.git
   ```
2. Open the project in your preferred Flutter development environment.
3. Run the app:
   ```sh
   flutter run
   ```

### Final Output Image 📸
![Final Google Logo Output](https://github.com/Hifza-Khalid/google-logo-flutter/blob/main/screenshots/Google2.JPG)
<hr>


## Author ✨
- Developed & modified by **Hifza** 🌟🖌️
## Gist Google logo in Flutter 🎨

[![Google Logo gist](https://img.shields.io/badge/Gist-view-blue)](https://gist.github.com/Hifza-Khalid/a029b430a4f089db173734d4fbd30a51)

## License 📚
This project is open-source and available under the [MIT License](LICENSE).

