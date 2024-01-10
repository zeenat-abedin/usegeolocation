# React Geolocation App

This React app uses the Geolocation API to get the user's current position and display it on a map.

## How to use

1. Clone the repo:

```
git clone https://github.com/username/react-geolocation-app.git
```

2. Install the dependencies:

```
npm install
```

3. Start the development server:

```
npm start
```

4. Open your browser and go to `localhost:3000`.

## Code Overview

The app consists of a single component, `App`, which is responsible for managing the state of the app and handling user interactions.

### State

The `App` component uses the `useState` hook to manage the following state variables:

- `isLoading`: A boolean that indicates whether the app is currently loading the user's position.
- `countClicks`: A number that represents the number of times the user has clicked the "Get my position" button.
- `position`: An object that contains the user's latitude and longitude coordinates.
- `error`: A string that contains an error message if the app encounters an error while trying to get the user's position.

### Event Handlers

The `App` component defines the following event handlers:

- `getPosition`: This function is called when the user clicks the "Get my position" button. It increments the `countClicks` state variable and then uses the `navigator.geolocation` API to get the user's current position. If the API call is successful, the `setPosition` state variable is updated with the user's position. If the API call fails, the `setError` state variable is updated with an error message.

### Rendering

The `App` component renders the following elements:

- A "Get my position" button.
- A loading indicator that is displayed while the app is loading the user's position.
- An error message that is displayed if the app encounters an error while trying to get the user's position.
- A map that displays the user's position if the API call is successful.
- A counter that displays the number of times the user has clicked the "Get my position" button.

## Conclusion

This React app demonstrates how to use the Geolocation API to get the user's current position and display it on a map. The app is simple to use and understand, and it can be
