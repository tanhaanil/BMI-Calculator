# BMI Calculator

A simple BMI Calculator built with **Flutter and Dart** as part of my Flutter learning journey. The app allows users to adjust their height and weight using sliders and see their BMI and corresponding category in real time.

## Live Demo

[Click the link](https://bmi-calculator-eight-pearl-40.vercel.app/)

## What the App Does

- Adjust height and weight using interactive sliders
- Calculate BMI in real time
- Display the BMI value and corresponding category
- Change the result indicator based on the BMI range
- Animate the result indicator when the BMI changes

## What I Learned

This project helped me understand the basic structure of a Flutter application and gave me hands-on experience with building UI, handling user input, and managing changing data.

### Flutter & UI

- Building layouts using `Column`, `Row`, `Expanded`, `Padding`, and `SizedBox`
- Working with Flutter's Material widgets
- Creating reusable widgets such as `BmiSlider` and `BmiResult`
- Using `Slider` to handle user input
- Styling text and containers using Flutter's styling and decoration APIs
- Adding simple animations with `AnimatedContainer`

### State Management

I used **Provider** to keep the BMI calculation and related state separate from the UI.

- `ChangeNotifier`
- `ChangeNotifierProvider`
- `Consumer`
- `notifyListeners()`
- Getter-based access to application state

The height and weight values are maintained inside `BmiProvider`. Whenever either value changes, the BMI, status, and result color are recalculated, and the UI updates automatically.

## Project Structure

```text
lib/
├── main.dart
├── bmi_home.dart
├── bmi_provider.dart
└── constants.dart
