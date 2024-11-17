
# Water Quality Monitoring System (WQMS)

### Project Overview
The Water Quality Monitoring System (WQMS) is an IoT-based solution for real-time monitoring and classification of water quality. By leveraging sensor technologies and machine learning models, this system provides actionable insights into water quality parameters such as **Temperature**, **Total Dissolved Solids (TDS)**, and **pH levels**.

Key features include:
- Real-time data acquisition using IoT sensors.
- Machine learning models for water quality classification (**Good** or **Bad**).
- Cloud-based data storage and visualization through **Firebase**.
- An intuitive user interface for monitoring trends and results.

---

### **Key Features**
- **Real-Time Monitoring**: IoT sensors measure temperature, TDS, and pH levels.
- **Data Analysis**: Classification of water quality using **Random Forest** and **Decision Tree** models.
- **Cloud Integration**: Firebase for secure data storage and retrieval.
- **User Interface**: Web-based dashboard for monitoring and visualizations.

---

### **System Architecture**
1. **Sensors**: Collect data on temperature, TDS, and pH.
2. **Microcontroller**: Transmit sensor data to the cloud.
3. **Firebase**: Store and manage real-time data streams.
4. **Machine Learning Models**: Classify water quality using pre-trained models.
5. **Dashboard**: Display water quality metrics and classification results.



---

### **Tech Stack**
- **IoT Hardware**: Sensors (Temperature, TDS, pH), Arduino/Raspberry Pi.
- **Back-End**: Python, Flask/Django.
- **Front-End**: HTML, CSS, JavaScript.
- **Cloud Platform**: Firebase (Realtime Database).
- **Machine Learning**: Scikit-learn (Random Forest, Decision Tree).

---

### **Installation**

#### **1. Clone the Repository**
```bash
git clone https://github.com/vikasJ07/WQMS.git
cd WQMS
```



#### **2. Set Up Firebase**
- Configure Firebase with your credentials and place them in the `config/firebase_config.json` file.
- Ensure appropriate rules are set in the Firebase Realtime Database.

#### **3. Run the Application**
Start the back-end server:
```bash
python src/app.py
```

Access the application at `http://127.0.0.1:5000`.

---

### Usage
1. **Connect IoT Devices**: Ensure sensors (Temperature, TDS, pH) are streaming data to Firebase.
2. **Monitor Water Quality**: Use the dashboard to view real-time data and classifications.
3. **Visualize Trends**: Analyze water quality over time using charts and graphs.
4. **Classification**: View whether the water is classified as **Good** or **Bad**.

---




### **Machine Learning Models**
- **Random Forest**: Trained on water quality datasets for robust classification.
- **Decision Tree**: Provides interpretable results for water quality status.
- Models are trained using the data in `data/water.csv`.

---

### **Future Enhancements**
- Add support for additional parameters (e.g., turbidity).
- Integrate alert systems (email/SMS) for poor water quality detection.
- Cloud deployment using platforms like AWS, Azure, or Heroku.
- Mobile app integration for on-the-go monitoring.

