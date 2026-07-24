Flutter Profile Screen

A simple profile screen built with Flutter as part of my learning process. The project focuses on creating a clean interface with basic Flutter widgets, organizing the layout, and reducing repeated code through reusable components and centralized colors.

Preview

The screen displays:

A custom app bar

A profile avatar

The user's name and occupation

Cards with profile statistics

A bottom navigation bar

Concepts Practiced

This project was created to practice:

Building an application with MaterialApp and Scaffold

Organizing widgets with Column and Row

Adding spacing with SizedBox

Styling widgets with Container and BoxDecoration

Using Material icons

Creating a reusable custom widget

Passing data through widget constructors

Using const constructors

Centralizing application colors in an AppColors class

Reusable Component

The statistics section uses a custom StatisticCard widget. The icon, value, and label are received through the constructor, allowing the same component to display different information without duplicating its layout.

const StatisticCard(
  icon: Icons.article,
  value: '128',
  label: 'Posts',
)

Color Organization

The main color is stored in an AppColors class:

class AppColors {
  AppColors._();

  static const Color primary = Color(0xFF146C43);
}

The color can then be reused with:

AppColors.primary

This makes the interface easier to maintain because the primary color can be changed in one place.

Technologies

Flutter

Dart

Material Design

How to Run

Make sure Flutter is installed and an emulator or physical device is available.

Clone this repository:

git clone <repository-url>

Enter the project folder:

cd <project-folder>

Install the dependencies:

flutter pub get

Run the application:

flutter run

Project Structure

The main interface is currently located in:

lib/main.dart

The file contains:

MyApp: configures the application theme and builds the profile screen

StatisticCard: reusable widget for profile statistics

AppColors: stores colors shared across the interface

Current Status

This is a static interface created for study purposes. The buttons and bottom navigation bar do not navigate to other screens yet.

Possible Improvements

Add navigation between screens

Load profile information from a model or API

Make the statistics responsive on smaller screens

Move widgets and theme settings into separate files

Add light and dark themes

Author

Developed as a Flutter learning project.
