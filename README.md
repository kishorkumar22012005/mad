# mad
---

NavigationKeys - Flutter Directional Arrow Button Widget

This Flutter project provides a reusable NavigationKeys widget that displays a directional control panel using arrow icons (Up, Down, Left, Right) to capture movement or navigation input. This can be useful for games, robots, or any application requiring directional interaction.

Features

Directional arrow key inputs: Up, Down, Left, Right

Detects:

Tap down

Tap release

Long press hold

Long press release


Callback to notify direction changes using ValueChanged<Direction>


Preview

> Add a screenshot or screen recording here if you can



Getting Started

1. Clone the Repository

git clone https://github.com/yourusername/navigation_keys_flutter.git
cd navigation_keys_flutter

2. Setup Dependencies

Make sure you have Flutter installed. Then run:

flutter pub get

3. Run the App

flutter run

How It Works

The NavigationKeys widget builds a column of arrow icons (Up, Left-Right row, Down).

Each arrow is built using the ArrowKey widget, which handles gestures like onTapDown, onTapUp, onLongPress, and onLongPressEnd.

Direction changes are sent back via the onDirectionChanged callback.


Usage Example

NavigationKeys(
  onDirectionChanged: (direction) {
    print('Current direction: $direction');
  },
),

Direction Enum

Make sure you define a Direction enum in a file like directions.dart:

enum Direction {
  none,
  up,
  down,
  left,
  right,
}

License

This project is open source and available under the MIT License.
