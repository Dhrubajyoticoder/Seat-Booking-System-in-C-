<div align="center">
  <h1 align="center">Seat Booking System in
 C++🚀
</h1>
  <h3>Supposed to develop a seat booking system for a theater with 5 rows by 10 columns of seats available to the users to reserve interactively.</h3>

</div>

<br/>



I took a 2D boolean array, seats[Row] [Col] to represent seat availability.
Initially, all the seat arranged to false means no sign of booking.

## Features

- **Seat Display :** The program displays the current seat arrangement in a grid format.
Available seats are represented by “[ ]”, and booked seats are represented by “X”.
Rows are labeled from A to E, and columns are numbered from 1 to 10.
- **Seat Reservation :** Users can input the desired row (A-E) and column (1-10) to book a seat.
The program checks if the selected seat is already booked or if it’s an invalid seat.
If the seat is available, it marks it as booked and provides a success message.
- **Input Validation :** The program ensures that the user enters valid row and column values.
If the input is invalid (e.g., out of range), it prompts the user to enter valid values.

- **Interactive Booking Loop:** The program allows users to book multiple seats in one session.
After booking a seat, it displays the updated seat arrangement.
Users can choose to continue booking more seats or exit the loop.

- **User-Friendly Interface:** The program provides clear instructions and prompts for user input.
It uses labels (A-E, 1-10) to make seat selection intuitive.

- **Dynamic Seat State Management:** The program maintains the state of each seat (booked or available) using a 2D boolean array.
When a seat is booked, it updates the array accordingly.

## Demo

![Papermark Welcome GIF](.github/images/papermark-welcome.gif)

## Tech Stack

- [C++](https://cplusplus.com/doc/tutorial/) – Language


## Getting Started

## Prerequisites

Here's what you need to be able to run Seat Booking System :

- ### Common C++ compilers include:
g++ (GNU Compiler Collection) for Linux.
MinGW (Minimalist GNU for Windows) for Windows.
Clang for cross-platform development.
- ### Text Editor or IDE:
Choose a text editor or an integrated development environment (IDE) to write your C++ code.
- ### Some popular options include:
Visual Studio Code (VS Code) with C/C++ extension.
Code::Blocks.
Dev-C++.
Sublime Text.
- ### Operating System:
C++ programs can run on various operating systems, including Windows, Linux, and macOS.
Ensure that your chosen compiler and IDE are compatible with your OS.
Hardware Requirements:
A standard computer with sufficient RAM and processing power.
Full HD resolution (ideally 1920x1080) for a comfortable coding experience.
- ### Basic Understanding of C++:
Familiarize yourself with C++ syntax, data types, control structures, and functions.
If you’re new to C++, consider learning the basics before diving into more complex programs.

## 1. Clone the repository

```shell
git clone https://github.com/mfts/papermark.git
cd papermark
```

### 2. Install npm dependencies

```shell
npm install
```

### 3. Copy the environment variables to `.env` and change the values

```shell
cp .env.example .env
```

### 4. Initialize the database

```shell
npx prisma generate
npx prisma migrate deploy
```

### 5. Run the dev server

```shell
npm run dev
```

### 6. Open the app in your browser

Visit [http://localhost:3000](http://localhost:3000) in your browser.

## Tinybird instructions

To prepare the Tinybird database, follow these steps:

0. We use `pipenv` to manage my Python dependencies. If you don't have it installed, you can install it using the following command:
   ```sh
   pkgx pipenv
   ```
1. Download the Tinybird CLI from [here](https://www.tinybird.co/docs/cli.html) and install it on your system.
2. After authenticating with the Tinybird CLI, navigate to the `lib/tinybird` directory:
   ```sh
   cd lib/tinybird
   ```
3. Push the necessary datasources using the following command:
   ```sh
   tb push datasources/*
   tb push endpoints/get_*
   ```
4. Don't forget to set the `TINYBIRD_TOKEN` with the appropriate rights in your `.env` file.

#### Updating Tinybird

```sh
pipenv shell
## start: pkgx-specific
cd ..
cd papermark
## end: pkgx-specific
pipenv update tinybird-cli
```

## Contributing

Papermark is an open-source project and we welcome contributions from the community.

If you'd like to contribute, please fork the repository and make changes as you'd like. Pull requests are warmly welcome.

### Our Contributors ✨

<a href="https://github.com/mfts/papermark/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=mfts/papermark" />
</a>
