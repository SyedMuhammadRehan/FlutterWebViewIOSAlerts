# FlutterWebViewIOSAlerts

🔍 **Problem Faced**: 

In our Flutter app, we encountered a challenge where JavaScript alert boxes were not popping up as expected when using the `flutter_webview` package on iOS. This was a crucial feature for our app's user experience, especially for interactive web content.

👨‍💻 **Solution Implemented**: 

To tackle this, extended the functionality of the app's AppDelegate class in Swift. The key was to use an `@objc` extension with FWFUIDelegate. This extension included custom methods to handle JavaScript alerts (`runJavaScriptAlertPanelWithMessage`) and confirms (`runJavaScriptConfirmPanelWithMessage`) using WKWebView.

🔧 **Code Insight**: 

By leveraging Swift's powerful capabilities alongside Flutter, we were able to implement `UIAlertController` to display the necessary alerts and confirmations. The solution involved intricate use of view controller hierarchy to present alerts from the topmost view controller, ensuring a seamless and native user experience.

🙌 **Result**: 

 The app now smoothly displays `web view alerts` on iOS, enhancing the functionality and user interaction of our app.
