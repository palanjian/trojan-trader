# Trojan Trader 📈
Trojan Trader is a web-based stock trading simulation application that allows users to virtually trade stocks, manage their portfolio, and learn about the stock market.
## Table of Contents
* [Overview](https://github.com/palanjian/trojan-trader#overview-)
* [Features](https://github.com/palanjian/trojan-trader#features-)
* [Demo](https://github.com/palanjian/trojan-trader#demo-)
* [Getting Started](https://github.com/palanjian/trojan-trader#getting-started-)
  - [Prerequisites](https://github.com/palanjian/trojan-trader#prerequisites-)
  - [Installation](https://github.com/palanjian/trojan-trader#installation-)
* [Usage](https://github.com/palanjian/trojan-trader#usage-%EF%B8%8F)
* [Technologies](https://github.com/palanjian/trojan-trader#technologies-)
* [Contributors](https://github.com/palanjian/trojan-trader#contributors-)

## Overview 🔎
Trojan Trader is a web platform designed to provide users with a simulated stock trading experience. Users can view real-time stock prices, track their portfolio performance, and learn about the stock market through educational resources.
![showcase3](https://github.com/palanjian/trojan-trader/assets/134035492/d8972b8c-b536-4a2c-9da4-9705fd30f69d)

This application was developed by a team of [team of 7](https://github.com/palanjian/trojan-trader#contributors-) over the course of two weeks as the Final Project for USC's CS201 (Principles of Software Development.)
## Features 📚
* __User Authentication and Security:__
  - Users can log in using their email addresses and passwords.
  - Sessions are managed using cookies for a secure and personalized user experience.
* __*My Stocks*:__
  - Users can view information about the stocks they own.
  - Real-time stock prices, average purchase prices, and quantity owned are displayed.
  - User's current balance, number of trades, and trade history are shown.
* __*Buy/Sell Stock*:__
  - Users can buy and sell stocks at select quantities.
  - Real-time stock prices are fetched from Finnhub to provide an accurate simulation.
* __*Education:*__
  - Users can access curated articles and guides to enhance their trading knowledge.
* __Account Creation & Login:__
  - Users can create accounts by providing an email address and password.
  - Accounts are validated to prevent duplicate entries.
* __Dynamic Content:__
  - JavaScript is used to update and display content without the need for page refresh.
* __Session Management:__
  - User sessions are managed using cookies to provide a seamless and secure experience.
* __Multithreading:__
  - Used to handle simultaneous buy & sell orders, login requests, and various other requests.

## Demo 🎬
A complete demo of the project can be found on [YouTube](https://www.youtube.com/watch?v=mjQc6VQXqMQ&ab_channel=PeterPalanjian)

## Getting Started 🏁
Follow these steps to set up and run the Trojan Trader application on your local machine.
### Prequisites
* __Java Development Kit (JDK)__ - (recommended version 14.0.0+)
* __Apache Tomcat__ - (recommended version 9.0+)
* __MySQL__ - (recommended version 8.0+)
* __Eclipse IDE__
### Installation
1. Clone this repository to your local machine or download the ZIP archive.
``` git clone https://github.com/palanjian/trojan-trader.git ```.
2. Open MySQL Workbench, create a new instance, and run the ```CreateTrojanTrader.sql``` script located in [SQL Scripts](https://github.com/palanjian/trojan-trader/tree/main/SQL%20Scripts) to generate the appropriate schema.
3. Configure your database connection details in the env class.
```
// env.java
public class env {
    public static final String JDBC_URL = "jdbc:mysql://your-database-url";
    public static final String SQL_USERNAME = "your-username";
    public static final String SQL_PASSWORD = "your-password";
}
```
4. Locate and run the ```stockupdater.py``` script located in [Python Scripts](https://github.com/palanjian/trojan-trader/tree/main/Python%20Scripts) to update real-time stock information.
5. Deploy your application on Apache Tomcat by right-clicking the project in Eclipse Explorer and selecting ``Run as → Run on Server``.

## Usage 🛠️
* User Registration and Login:
  - Users need to create an account by providing their email and password. They can then use these credentials to log in to the platform securely.
* My Stocks Page:
  - After logging in, users are presented with the "My Stocks" page. This page provides an overview of their owned stocks, including current prices, average purchase prices, and quantities.
* Buy/Sell Stocks:
  - Users can navigate to the "Buy/Sell Stock" page, where they can search for stocks, view real-time prices, and make buying or selling decisions based on the current market data. Each user originally given $10,000 balance to trade with, and the objective is to increase this balance over time.

## Technologies 💾
* __HTML & CSS__ → structure & styling
* __Javascript__ → cookies, AJAX requests, & more
* __Font Awesome__ → font and icon toolkit
* __Java__ → main language used for the backend logic
* __Servlets__ → Java classes used to handle HTTP requests and dynamically generate responses.
* __Apache Tomcat__ → web server and servlet container used to deploy/run Java servlets
* __MySQL__ (with JDBC) → persistent account and stock information storage. JDBC driver used to interact with SQL tables through Java. 
* __Python Scripting__ (with External APIs) → utilizes Finnhub to provide real-time accurate stock information
## Contributors 👥
Trojan Trader was developed with the help of [@palanjian](https://github.com/palanjian), [@Dionysssss](https://github.com/Dionysssss), [@shayet-rbj](https://github.com/shayet-rbj), [@Tsayuel](https://github.com/Tsayuel), 
[@Loui-Ikei](https://github.com/Loui-Ikei), [@AngelaSiruiZhu](https://github.com/AngelaSiruiZhu), & [@angela-shuya](https://github.com/angela-shuya)
