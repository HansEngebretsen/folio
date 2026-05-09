# Portfolio Forecaster

A high-density, interactive financial projection tool built with React, Recharts, and Tailwind CSS. It allows users to forecast portfolio growth based on historical stock data, customizable monthly contributions, and inflation rates.

## Features

- **Interactive Projections:** Visualize portfolio growth over time with a dynamic area chart.
- **Stock Analysis:** Pre-populated with historical 10-year CAGR data for popular stocks and indices.
- **Scenario Planning:** Adjust upside and downside factors to see how your portfolio might perform in different market conditions.
- **Financial Controls:** 
  - Time Horizon (1-40 years)
  - Monthly Contributions
  - Inflation Rate adjustment
  - Upside/Downside risk multipliers
- **Real-time Calculations:**
  - 3.5% and 4% withdrawal rate projections (Safe Withdrawal Rate analysis).
  - Total principal vs. total projected value.
- **Interactive UI:**
  - Resizable panels (Holdings, Chart, Controls).
  - Dark, Light, and High Contrast themes.
  - Scrubbable inputs for quick value adjustments.
  - Interactive pie chart for asset allocation.
- **Persistence:** Automatically saves your portfolio state to local storage (browser cache).

## Tech Stack

- **Frontend:** React (v18)
- **Styling:** Tailwind CSS
- **Charts:** Recharts
- **Icons:** Lucide React
- **Runtime:** Single-file HTML application using Babel for in-browser JSX/TSX compilation.

## Getting Started

Simply open `index.html` in any modern web browser. No build step or server is required as all dependencies are loaded via ESM/CDN.

## How it Works

The application calculates future value using standard compound interest formulas, accounting for both initial principal and recurring monthly contributions. Growth rates for stocks are initialized with their 10-year historical averages (where available), while "Cash" positions are adjusted based on the user-defined inflation rate.
