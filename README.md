# Another Calculator - Kotlin Multiplatform

This project demonstrates building a calculator application using Kotlin Multiplatform, targeting Android, iOS, Web, and Desktop platforms.

## Project Structure

* /composeApp: Contains shared code for all Compose Multiplatform targets.
  * commonMain: Code shared across all platforms (business logic, core calculations, etc.).
  androidMain: Android-specific code (UI adjustments, platform integrations). 
  * iosMain: iOS-specific code (UI adjustments, platform integrations). 
  * desktopMain: Desktop-specific code (UI adjustments, platform integrations). 
  * wasmJsMain: Web-specific code (UI adjustments, platform integrations).
* /androidApp: Contains the Android application module. 
* /iosApp: Contains the iOS application module. Add SwiftUI code here as needed to integrate with the shared Compose Multiplatform UI.

## Getting Started

1. Clone the repository: `git clone https://github.com/ubinix-warun/another-calculator.git`
2. Open the project in Android Studio: Ensure you have the Kotlin Multiplatform Mobile plugin installed. 
3. Run the desired target:
   * Android: Build and run the androidApp module. 
   * iOS: Open the iosApp project in Xcode and build/run. 
   * Desktop: Run the desktopApp module. `./gradlew run`
   * Web: Execute the Gradle task `:composeApp:wasmJsBrowserDevelopmentRun` to open the web application in your browser.

## Technologies Used
* Kotlin Multiplatform: Enables code sharing across multiple platforms. 
* Compose Multiplatform: Modern declarative UI framework for consistent user experiences. 
* Kotlin/Wasm: Compiles Kotlin code to WebAssembly for web deployment.

## Feedback and Issues

We welcome your feedback on Compose/Web and Kotlin/Wasm in the #compose-web Slack channel.
If you encounter any issues, please report them on the GitHub repository.

## Additional Notes
* This project leverages best practices for Kotlin Multiplatform development. 
* The shared commonMain module maximizes code reuse, reducing development effort. 
* Platform-specific modules allow for tailored experiences on each target platform.

Feel free to explore and contribute to this project!