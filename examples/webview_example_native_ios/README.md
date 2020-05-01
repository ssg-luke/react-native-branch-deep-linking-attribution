# webview_example_native_ios

This app presents a list of the planets in a UITableView. When each
row is tapped, an RCTRootView is displayed with a React Native Article component.
Both the native app and the React Native component make use of the Branch SDK.

The Article component contains a WebView and displays the Wikipedia page for the
selected planet. It creates a Branch Universal Object in
`componentWillMount` and registers a view event. A large Share button at the
bottom of the Article component calls `showShareSheet` on the BUO.

In the app delegate, the `RNBranchLinkOpenedNotification` is used to route
inbound links and pushes an Article component for the appropriate article when
a link is opened.

The app was produced following the methodology outlined in these tutorials:

- https://facebook.github.io/react-native/docs/integration-with-existing-apps.html
- https://www.raywenderlich.com/136047/react-native-existing-app

## Building

To build and run:

```bash
yarn
```

or

```bash
npm i
```

then

```bash
bundle check || bundle install
bundle exec pod install
```
