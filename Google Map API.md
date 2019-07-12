first, follow this https://medium.com/nycdev/create-a-react-native-app-with-google-map-using-expo-io-68041252023d to get your API Key, and enable google place and google maps api two service.
Then, in the root, create a file as apiKey.js, inside write: export const googleApiKey = "Your API Key";
In app.json file, change:  "ios": {
  "bundleIdentifier": "any thing you like to put here",
  "config": {
    "googleMapsApiKey": "YOUR IOS API KEY HERE"
  }
},
