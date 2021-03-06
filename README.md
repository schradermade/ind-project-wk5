# _Super Galactic Age Calculator_

#### _Web form to accept user's Earth Age and Life Expectancy, and output users age stats for a given planet, 11.13.2020_

#### By _**Nathan Schrader**_

## Description

_A solar year lasts 365 days on planet Earth. However, the length of a solar year varies from planet to planet. For instance, a solar year on Mercury lasts 88 days. This application will determine a user's age based on a planet's solar years._

* A Mercury year is .24 Earth years, therefore a 35 year old would be "8.4 Mercury years"
* A Venus year is .62 Earth years, therefore a 35 year old would be "21.7 Venus years"
* A Mars year is .1.88 Earth years, therefore a 35 year old would be "65.8 mars years"
* A Jupiter year is 11.86 Earth years, therefore a 35 year old would be "415.1 Jupiter years"
    
Application also determines how many years a user has left to live on each planet, based on a set "user life expectancy". Therefore, for each different planet a user will be returned with both their "planet" age as well las how many years more they are expected to live.

**Example:** If a user inputs a inputs an **Earth Age: 35** and **Life Expectancy: 100** and the user wants to know their age data for Mars, the program should display 3 values:<br><br> **"Your Mars stats: Age - 65.8, Expected life - 188, Your remaining life is about 122.2 years!"** 

## Setup/Installation

### Requirements:

* Internet Browser
* Code editor if you want to explore the code

### Download:

1. Download this repository by clicking the green 'Code' button and selecting "Download Zip"
2. Unzip the file to extract files to your local drive. 
3. In your Terminal navigate to the root directy where the project exists and install webpack by typing:
    `npm install`
4. Open the `index.html` file in your browser.

### Terminal:

1. Open command terminal on local device
2. Navigate to the directory where you want respository to save to
3. Copy repository link by clicking on the green "Code" button and clicking 'clipboard' icon
4. Back in the terminal, type `git clone {Repository-URL-here}`
5. In your code editor program, open the newly created repository directory
6. Right click on the `index.html` file and select "Copy file path"
7. Paste the link into your web browser window

## Spec Table
| Test.# | Describe     |      Test     | `expect().toEqual()` |
|:------:| :------------ |:-------------| :---------------------------|
| 1 | **userAge**  |_should correctly take in user "Earth Age" and desired "Life Expectancy"_ | **expect**(`userInput`("35")).`toEqual`("35")<br><br>**expect**(`userInput`("100")).`toEqual`("100") |
|   | | | |
| 2 | **mercuryAge** |_should correctly output: 1. users age 2. user life expectancy 3. years left;<br><br>All refactored in Mercury years_ |**expect**(`reusableStats.mercury()).toEqual`("Your Mercury stats: Age - 8.4, Expected life - 24, Your remaining life is about 15.6 years!");<br><br>**expect**(`reusableStats2.mercury()).toEqual`("Your Mercury stats: Age - 24, Expected life - 8.4, You have outlived your life expectancy by 15.6 years!"); |
|   | | | |
| 3 | **venusAge** | _should correctly output: 1. users age 2. user life expectancy 3. years left;<br><br>All refactored in Venus years_ | **expect**(`reusableStats.venus()).toEqual`("Your Venus stats: Age - 21.7, Expected life - 62, Your remaining life is about 40.3 years!");<br><br>**expect**(`reusableStats2.venus()).toEqual`("Your Venus stats: Age - 62, Expected life - 21.7, You have outlived your life expectancy by 40.3 years!"); |
|   | | | |
| 4 | **marsAge** | _should correctly output: 1. users age 2. user life expectancy years left;<br><br>All refactored in Mars years_ | **expect**(`reusableStats.mars()).toEqual`("Your Mars stats: Age - 65.8, Expected life - 188, Your remaining life is about 122.2 years!");<br><br>**expect**(`reusableStats2.mars()).toEqual`("Your Mars stats: Age - 188, Expected life - 65.8, You have outlived your life expectancy by 122.2 years!"); |
|   | | | |
| 5 | **jupiterAge** | _should correctly output: 1. users age 2. user life expectancy years left;<br><br>All refactored in Jupiter years_ | **expect**(`reusableStats.jupiter()).toEqual`("Your Jupiter stats: Age - 415.1, Expected life - 1186, Your remaining life is about 770.9 years!");<br><br>**expect**(`reusableStats2.jupiter()).toEqual`("Your Jupiter stats: Age - 1186, Expected life - 415.1, You have outlived your life expectancy by 770.9 years!"); |
|   | | | |
| 6 | **yearsDynamic** | _should correctly assign dynamic value to `this.yearsLeft`, depending on if users age is under or over the expected life_ | **expect**(`reusableStats.yearsDynamic()).toEqual`("Your remaining life is about")<br><br>**expect**(`reusableStats2.yearsDynamic()).toEqual`("You have outlived your life expectancy by"); |

## Known Bugs

No known bugs at this time. If you find a bug, let me know via email!

## Support and contact details

_If you run into any issues or have concerns, please reach out at **nathanschrader@icloud.com**_

## Technologies Used


* HTML
* CSS
* Bootstrap
* JavaScript - ES6
* jQuery
* Test Driven Development
* Visual Studio Code
* Git
* Github


## Legal

Copyright (c) 2020 **_Nathan Schrader_**

This software is licensed under the MIT license.
