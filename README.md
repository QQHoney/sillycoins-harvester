# SillyCoins Harvester

SillyCoins Harvester is an automated tool designed to interact with the panel.sillydev.co.uk website, periodically earning coins and monitoring account balance.

## Features

- Automated login and session management
- Periodic coin earning requests
- Real-time balance monitoring
- Customizable banner styles
- Express server for status monitoring

## Prerequisites

- Node.js (v14 or higher)
- npm (Node Package Manager)

## Installation

1. Clone the repository:

   ```
   git clone https://github.com/QQHoney/sillycoins-harvester.git
   cd sillycoins-harvester
   ```

2. Install dependencies:

   ```
   npm install
   ```

3. Set up the environment variables:
   - Copy the `.env.example` file to `.env`:
     ```
     cp .env.example .env
     ```
   - Edit the `.env` file and replace `your_cookies_here` with your actual cookies from panel.sillydev.co.uk
   - Optionally, you can change the `PORT` if you want the server to run on a different port

## Configuration

You can customize the behavior of SillyCoins Harvester by modifying the `src/constants.js` file:

- `heartbeatInterval`: Time between heartbeat checks (default: 5000ms)
- `displayInterval`: Time between displaying status updates (default: 60000ms)
- `sessionRefreshInterval`: Time between session refreshes (default: 900000ms)
- `earnRequestInterval`: Time between coin earning requests (default: 60000ms)
- `bannerStyle`: Choose the banner style ('ASCII_ART', 'SIMPLE', or 'MINIMAL')
- `debugMode`: Set to `true` to enable debug logs (default: false)

## Usage

To start the SillyCoins Harvester:

```
npm start
```

For development with auto-restart on file changes:

```
npm run dev
```

## API Endpoints

- `GET /`: Returns a simple message indicating that the harvester is running
- `GET /status`: Returns the current status of the harvester

## Important Notes

- This tool is designed for educational purposes only. Use it responsibly and in accordance with the terms of service of the target website.
- Keep your cookie information secure and do not share it with others.
- The tool uses a custom logging system. Check the console output for real-time updates and any error messages.

## License

This project is licensed under the MIT License.

## Author

[mra1k3r0](https://github.com/mra1k3r0)

## Disclaimer

This project is not affiliated with or endorsed by panel.sillydev.co.uk. Use at your own risk.
