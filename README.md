# Coin-Based Mobile Charger

##  Overview
This project presents a *coin-operated mobile charging system* that enables users to charge their phones by inserting coins.  
It provides an affordable and accessible solution for mobile charging in *public places such as bus stops, train stations, and rural areas* where traditional charging options may not be available.

The system combines *embedded systems and IoT* to make charging both intelligent and convenient.

##  How It Works
- When a *coin is inserted, it is validated by the **coin acceptor sensor*.
- The *Arduino Uno* receives a signal indicating a valid coin.
- The system then starts supplying *5V power* to the mobile charging port.
- A *reverse countdown timer* is displayed on the LCD to show the remaining charging time.
- The system uses an *ESP8266 Wi-Fi module* to send data (coin entries and usage stats) to the cloud (ThingSpeak platform).
- After the timer expires, the relay cuts off power to stop charging.

##  Features
- Coin-based activation for mobile charging  
- LCD display showing charging time and status  
- IoT-enabled monitoring via *ThingSpeak Cloud*  
- Secure and reliable Arduino-based control  
- User-friendly interface for public use  
- Works offline with optional online tracking  

##  Components Used
### Hardware
- Arduino UNO  
- Coin Acceptor Module  
- IR Sensors  
- Relay Module  
- ESP8266 Wi-Fi Module  
- 16x2 LCD Display  
- Buzzer  
- Power Supply (5V output)

### Software
- Arduino IDE  
- Embedded C / C++  
- ThingSpeak Cloud (for IoT data visualization)
##  Project Flow
1. User inserts a coin  
2. Arduino verifies if the coin is valid  
3. If valid, charging begins for a set duration (e.g., 2, 5, or 15 minutes)  
4. LCD displays the countdown timer  
5. Once time expires, relay disconnects the circuit  
6. ESP8266 uploads the transaction data to ThingSpeak  

---

##  Algorithm (Simplified)
1. Start  
2. Initialize Arduino and power supply  
3. Detect coin insertion using IR sensors  
4. Validate coin and send pulse to Arduino  
5. Activate relay → begin charging  
6. Display remaining time on LCD  
7. After timeout → stop charging  
8. Update data to ThingSpeak  
9. End  


##  Results
- Achieved average charging efficiency of *1.5% per minute* across devices.  
- Real-time data uploaded to *ThingSpeak* for usage analysis.  
- Outperformed conventional public chargers in *accessibility and convenience*.  
- Validated the concept as a *cost-effective public utility solution*.

<img width="860" height="140" alt="image" src="https://github.com/user-attachments/assets/3f0b1c06-0c6b-4aba-ba3f-8924c9bc4e2e" />
		


##  Significance
This project bridges *embedded systems and IoT* to deliver a real-world, socially impactful innovation.  
It demonstrates how technology can solve everyday problems and provides a scalable idea for *smart cities and rural electrification*.



##  Conclusion
The Coin-Based Mobile Charger provides a *low-cost, reliable, and accessible charging solution* for public spaces.  
By integrating *Arduino control, IR sensing, and IoT connectivity, this project demonstrates innovation in both design and utility - merging **engineering with social impact*.


##  License
This project is open for educational and research purposes.
