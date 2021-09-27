# flutter_debugprint_web_issue

# Issue

when a Flutter project is run in release mode on the web, debugPrint() prints to the console surfacing print statements used for debuging purposes.


## Reproduction Steps

1. Create the template Flutter project with web capabilities
2. Add `debugPrint('Counter incremented')` statement in the _incrementCounter() function
3. Run: `flutter build web`
4. Run: `flutter run --release -d chrome`
5. Inspect the page and go to the console tab
6. Press the "+" increment button and the debugPrint() statement prints to the console