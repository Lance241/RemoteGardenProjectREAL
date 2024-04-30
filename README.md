![RemoteGarden](src/main/java/edu/redwoods/cis18/scam/projectlogo.jpg "Soil Moisture Sensor")

## Overview
Welcome to the RemoteGarden, where we strive to digitally greenify your thumb! This project utilizes an Arduino Uno R3 to monitor soil moisture, reporting it back to a Java-based backend, with data stored in a MySQL database—because even plants have gone digital.

### What It Does
The system reads moisture levels from a soil sensor and sends this data through the mystical ethers of USB to a Java application. The data can eventually be saved in a MySQL database for trend analysis and historical tracking.

### Current Capabilities
- **Arduino Readings**: Every second, our trusty Arduino reads how thirsty your plant is and sends this data serially.
- **Java Application**: Receives this data and processes it for database storage.
- **Database Manager**: Data transfer post-processing initiated from inner class from `ArduinoSerialPortObserver`
- **JavaFX Interface**: loads

# Goals:

## -Tier 1
- **Database Integration**: Implement MySQL for data storage. Implement database structures and queries
- **Data Processing**: Enhanced `processLine` method in `ArduinoSerialPortObserver` to process and store data efficiently.
- **Refactor**: clean up dir tree to remove redundant class files.
- **JavaFX**: Confirm positive connection between GUI and DB
- **Final Migration**: last call to migrate code from the first project

## -Tier 2
- **Arduino Wifi Integration**: Enable communication over WiFi to eliminate the need for wired connections.
- **Additional Sensors**: Expand the system to include light and humidity sensors for comprehensive plant monitoring.

## Installation
1. Ensure Maven, MySQL and JDK 20 are installed.
2. Clone the repository.
3. Install MySQL and DBeaver:
    - **MySQL**: Download and install from [MySQL's official page](https://dev.mysql.com/downloads/mysql/).
    - **DBeaver**: Download and install from [DBeaver's official page](https://dbeaver.io/download/).
    - Setup instructions are included in the 'Database Setup' section.
4. Configure the database using the provided SQL script.
5. Run `mvn clean compile javafx:run`.

## Database Setup
To set up your MySQL database: DON'T FORGET YOUR MYSQL USERNAME AND PASSWORD.
1. Open DBeaver and connect to your local MySQL server.

## Contributions
Contributions are welcomed. If you break something, you get to keep both pieces.

## Known Issues
- No reported issues with the new database integration.
- Consider renaming `cis18/` directory if module name warnings persist.
- GUI enhancements are ongoing.


Happy coding. 🌱
