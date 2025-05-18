# ✈️ SkyRadar Bot

SkyRadar is a VATSIM-integrated Discord bot built for virtual pilots and ATC. It brings powerful flight simulation tools into your server — including live flight tracking, METAR/TAF weather, controller listings, and automated logging.

> 🛰 Built for VATSIM, flight sim communities, and aviation Discords.

---

## 📦 Features

- ✈️ `/track` – Track any flight by VATSIM callsign  
- 📋 `/flightplan` – View the filed flight plan of a pilot  
- 🧑‍✈️ `/myflight` – Check your own current VATSIM flight (via linked CID)  
- 🔔 `/arrivalalert` – Get alerted when a callsign nears its destination  
- 📜 `/metar` & `/taf` – Fetch real-world METAR/TAF weather data  
- 📅 `/events` – Show upcoming official VATSIM events  
- 🛢 `/fuelestimate` – Estimate fuel/time for a flight based on aircraft & distance  
- 📊 `/flightstats` – View your flight history (flights tracked, date range)  
- 🛫 `/airportinfo` – Show airport data: runways, elevation, frequencies  
- 🛩 `/aircraftinfo` – Get info about any aircraft type (ICAO)

---

## 🧱 Tech Stack

- **Discord.js v14**
- **Prisma ORM**
- **PostgreSQL** or **SQLite**
- Axios for VATSIM & weather APIs
- Modular command & event system

---

## 🚀 Getting Started

1. **Clone the repository**

   ```bash
   git clone https://github.com/YOUR-ORG/skyradar-bot.git
   cd skyradar-bot
   ```

2. **Install dependencies**

   ```bash
   npm install
   ```

3. **Create your `.env` file**

   ```env
   DISCORD_TOKEN=your-bot-token
   DATABASE_URL=your-prisma-database-url
   DISCORD_ANALYTICS_API_KEY=your-api-key-if-used
   ```

4. **Generate & migrate your database**

   ```bash
   npx prisma generate
   npx prisma migrate dev --name init
   ```

5. **Start the bot**

   ```bash
   npm run dev
   ```

---

## 📁 Project Structure

```
sky-radar-bot/
├── src/
│   ├── commands/
│   ├── events/
│   ├── tasks/
│   ├── config/
│   ├── utils/
│   └── index.js
├── prisma/
│   └── schema.prisma
├── config/statusMessage.json
├── .env
├── package.json
└── README.md
```

---

## 🤝 Contributing

Pull requests are welcome! Please fork the repo and submit a PR.  
Open an issue for major features or bug reports.

---

## 📃 License

MIT © [SkyRadar Team](https://github.com/SkyRadar-Bot)

