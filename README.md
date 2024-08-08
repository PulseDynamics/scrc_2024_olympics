# SCRC Olympics Pool 2024

Welcome to the **SCRC Olympics Pool 2024** repository! This project hosts the source code and data for the SCRC Olympics Pool website, which allows participants to engage with the 2024 Summer Olympics by making predictions, viewing standings, and checking results in real-time.

## Table of Contents

1. [Project Overview](#project-overview)
2. [Website Features](#website-features)
    - [Home](#home)
    - [Participants' Picks](#participants-picks)
    - [Standings](#standings)
    - [Event Results](#event-results)
3. [Data Files](#data-files)
4. [How the Website Works](#how-the-website-works)

## Project Overview

The SCRC Olympics Pool website is an interactive platform designed to enhance the Olympics viewing experience by allowing participants to predict the outcomes of various events. Participants can view the overall standings, individual picks, and the results of the completed events.

The website is built with **HTML**, **CSS**, and **JavaScript**, utilizing the **XLSX.js** library to process and display data from Excel files in real-time.

## Website Features

### Home

The **Home** page serves as the landing page for the website and includes the following elements:
- **Welcome Message**: A brief welcome message and introduction to the pool.
- **Live Clock**: A live clock showing the current date and time in Eastern Daylight Time (EDT).
- **Race Schedule**: A list of upcoming events with their scheduled dates and times. Clicking on an event reveals additional details such as start lists, and once the event is completed, it is marked with a "COMPLETED" status.

### Participants' Picks

The **Participants' Picks** page displays the predictions made by each participant. The page includes:
- **Color Codes**: An explanation of the color codes used to indicate the status of picks:
  - **Yellow**: Event is still to come.
  - **Red**: Incorrect pick.
  - **Green**: Correct pick.
- **Picks Table**: A table for each participant showing their picks for each event (Winner, 2nd Place, and 3rd Place). The picks are color-coded based on the accuracy of the predictions.

### Standings

The **Standings** page provides a real-time leaderboard showing the current points of each participant. It includes:
- **Sorted Standings**: Participants are listed in descending order based on their total points.
- **Points Calculation**: Points are awarded based on the accuracy of the predictions:
  - **Winner**: 10 points.
  - **2nd Place**: 6 points.
  - **3rd Place**: 4 points.
  - **Bonus**: An additional 5 points if all three picks are correct for an event.

### Event Results

The **Event Results** page shows the results of the completed events. The results are manually updated and include:
- **Event Details**: Information on each event, including the positions of the top 8 competitors.
- **Updates**: This section will dynamically update as more event results are entered into the system.

## Data Files

The website relies on two key Excel files stored in this repository:
- **SCRC_2024_Olympics_Pool_PICKS.xlsx**: Contains the picks made by each participant for each event.
- **SCRC_2024_Olympics_Pool_Results.xlsx**: Contains the official results of the events.

These files are loaded dynamically by the website to display the most up-to-date information.

## How the Website Works

### Data Loading

When the website loads, it fetches data from the provided Excel files using the **XLSX.js** library. This allows the site to dynamically display participants' picks, standings, and event results without requiring manual updates to the HTML or JavaScript code.

### Real-Time Updates

The website updates in real-time as the data in the Excel files changes. For example:
- **Participants' Picks**: When a new event result is added, the corresponding picks are immediately checked and color-coded on the Picks page.
- **Standings**: As event results are updated, the standings are recalculated, and participants' scores are updated accordingly.
- **Event Results**: The Event Results page displays the latest event results entered into the system.

### Popup Information

On the **Home** page, hovering over an event shows a popup with detailed information such as start lists and other relevant details. This information is hidden by default and only displayed when the user interacts with the event list.

### Responsiveness

The website is fully responsive and adapts to different screen sizes, ensuring a smooth user experience across devices, including desktops, tablets, and smartphones.
