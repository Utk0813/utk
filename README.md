# FYP SolarShare
Final Year Project 2020- Energy Monitoring and Management System Based on Blockchain Technology

Verison 1.0 with NEM Blockchain (Testnet)
### Note:
unpack "node_modules" and "design" at ../UniversalAssets/ <br>
Version 1.0 may no longer work correct as of today

Used with localhost via XAMMP
Run to start -> http://localhost:8080/P2PTrading/homepage2.php

### Prerequisite process and Program

This program runs on localhost machine,
requires XAMMP with MySQL for demo

### Requires a database named "household_solar2"
List of tables:

1. boughtenergyfromtrader
-Price int(11)
-EnergyAmt int(11)
-Total int(11)
-DateTime date

2. soldenergytotrader
-Price int(11)
-EnergyAmt int(11)
-Total int(11)
-DateTime date

3. buyfromsolar
-Price int(11)
-EnergyAmt int(11)
-Total int(11)
-DateTime date

4. solarpanel
- Solar_ID varchar(6)
- Address varchar(50)
- Status carchar(100)


### Grant access to database with SQL

GRANT ALL ON household_solar2.* TO 'testuser'@'localhost' IDENTIFIED BY 'password';

### Symbol-sdk installation
"npm install symbol-sdk rxjs" at 
1. P2PTrading/UniversalAssets/js
2. P2PTrading/userpageserver/js
<br>P2PTrading = project name </br>
### Coversion of Symobol-sdk for browser environment

"cd" command --> to "./UniversalAssets"

Browserify -r ./UniversalAssets/js/node_modules/symbol-sdk -o symbol-sdk.js

Browserify -r ./UniversalAssets/js/node_modules/rxjs -o rxjs.js

Browserify -r .UniversalAssets/js/node_modules/rxjs/operators -o rxjs_operators.js


===== OPTIONAL ======

Blockchain monitoring:
install symbol-cli on cmd.exe
"npm install --global symbol-cli"

"symbol-cli account monitor all" to monitor 
blockchain network

Symbol wallet:
Install symbol official testnet wallet program

# FYP SolarShare 2.0
Version 2.0 with SYMBOL Blockchain TEST_NET(by NEM).
This version is not available to the public.
Below is the sample screenshot of 2.0:

![alt text](https://github.com/yangben526/FYP_SolarShare/blob/main/Platform_img/Front.PNG)
![alt text](https://github.com/yangben526/FYP_SolarShare/blob/main/Platform_img/Front_2.PNG)
![alt text](https://github.com/yangben526/FYP_SolarShare/blob/main/Platform_img/main_dash.PNG)
![alt text](https://github.com/yangben526/FYP_SolarShare/blob/main/Platform_img/main_dash2.PNG)
![alt text](https://github.com/yangben526/FYP_SolarShare/blob/main/Platform_img/ENergydata.PNG)
![alt text](https://github.com/yangben526/FYP_SolarShare/blob/main/Platform_img/exchnage.PNG)

# Energy Monitoring and Monitoring, and P2P Energy Trading System
Trading tokenised energy(vagabond.energy) with intrinsic tokens/cryptocurrencies(SYMBOL.xym by NEM)
![alt text](https://github.com/yangben526/FYP_SolarShare/blob/main/Platform_img/SolarShareP2PDiagram.png)

The P2P Energy Trading with Smart Contract
![alt text](https://github.com/yangben526/FYP_SolarShare/blob/main/Platform_img/smart_contract.png)
