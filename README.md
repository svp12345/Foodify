# Foodify

Order food from the comfort of your home. Foodify provides the latest restaurants available in your city with all the details. Pick a dish, add it to your cart, place an order, and get it delivered right to your doorstep.

## Features
- Fetch live restaurant data from the Swiggy API.
- Display restaurants with details like area name, cuisine category, and ratings.
- Search restaurants by name.
- View available dishes for any restaurant with detailed pricing per quantity.
- Add items to the cart.
- User authentication for secure transactions.
- Place orders seamlessly.

## Tech Stack
- **Frontend Library:** React JS
- **Styling:** Tailwind CSS
- **Database:** Firebase
- **Bundler:** Parcel
- **Authentication:** Firebase Authentication
- **State Management:** Redux Toolkit

## Installation and Setup

Follow these steps to set up the project on your local machine:

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/yourusername/foodify.git
   cd foodify
   ```

2. **Install Dependencies:**
   ```bash
   npm install
   ```

3. **Add Firebase Configuration:**
   - Create a Firebase project at [Firebase Console](https://console.firebase.google.com/).
   - Set up Firebase Authentication and Firestore Database.
   - Copy your Firebase configuration details.
   - Create a `.env` file in the root directory and add the following:
     ```env
     REACT_APP_FIREBASE_API_KEY=your_api_key
     REACT_APP_FIREBASE_AUTH_DOMAIN=your_auth_domain
     REACT_APP_FIREBASE_PROJECT_ID=your_project_id
     REACT_APP_FIREBASE_STORAGE_BUCKET=your_storage_bucket
     REACT_APP_FIREBASE_MESSAGING_SENDER_ID=your_sender_id
     REACT_APP_FIREBASE_APP_ID=your_app_id
     ```

4. **Run the Development Server:**
   ```bash
   npm start
   ```
   The app will be available at `http://localhost:3000/`.

## Working of the Project

1. Fetches live restaurant data from the Swiggy API, displaying the latest updates.
2. Displays restaurant information such as area name, cuisine category, and ratings.
3. Enables search functionality to find restaurants by name.
4. Shows detailed menus for restaurants, including dish details and prices.
5. Allows users to add items to the cart, authenticate via Firebase, and place orders securely.

## Key Features Implemented

- **Configuration-Driven UI:** Streamlined a configuration-driven UI where data dynamically updates based on location-specific configurations.
- **Performance Optimization:** Implemented lazy loading and code splitting, reducing page load time by 35%.
- **Loading Experience:** Added Shimmer UI for loading skeletons to improve the user experience when data is being fetched.
- **Custom Hooks:** Created reusable custom hooks to manage component logic and utilized the `useContext` hook to avoid props drilling.
