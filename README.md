# Next Generation Intrusion Detection System (NGIDS)

Next Generation Intrusion Detection System (NGIDS) is an advanced anomaly-based Intrusion Detection System (IDS) that utilizes machine learning algorithms to predict anomalies in network traffic. It captures network data using the TShark utility and analyzes 26 features, including IP addresses, packet length, TCP flags, HTTP requests, and more.

NGIDS incorporates three machine learning models: Principal Component Analysis (PCA), Isolation Forest, and One-Class Support Vector Machines (SVM). These models analyze the captured network traffic data in real-time to detect anomalies effectively.

## Key Features

- Machine Learning Models: NGIDS employs PCA, Isolation Forest, and One-Class SVM algorithms to identify anomalies in network traffic data.
- Cloud Database: Network traffic data is securely stored in a cloud-based MongoDB database, ensuring data integrity and availability.
- User Authentication: NGIDS implements user authentication functionality, allowing registered users to securely access and utilize the system.
- Real-Time Analysis: The system continuously monitors and analyzes network traffic data in real-time, promptly detecting anomalies as they occur.
- Alert Notifications: NGIDS sends immediate alert notifications via email to users when anomalies are detected, providing detailed information about the anomaly, including the date and time of capture.

## Getting Started

To use NGIDS, follow these steps:

1. Download the NGIDS Client utility.
2. Run the application and provide login credentials. If you don't have an account, sign up using the provided signup page.
3. Once logged in, you will see a window with options to capture network traffic data or navigate to the dashboard.
4. Start the capture process to begin capturing network traffic data, which will be securely stored in a cloud-based MongoDB database.
5. Access the dashboard to view real-time anomaly detection results. The dashboard fetches the latest network traffic data from the cloud database and feeds it to the machine learning models for analysis.
6. If an anomaly is detected, NGIDS will send an alert to your registered email, providing detailed information about the anomaly, including the date and time of capture.

## Requirements

- TShark utility
- MongoDB
- Python packages:
  - Flask
  - PyQt5
  - pandas
  - numpy
  - sklearn
  - joblib
  - pymongo
  - bcrypt
  - plyer
  - yagmail

## Usage

1. Set up the required dependencies and ensure the MongoDB connection details are correctly configured.
2. Run the NGIDS application by executing the main script.
3. Use the NGIDS Client utility to log in, capture network traffic data, and access the dashboard.
4. Monitor the real-time anomaly detection results on the dashboard and receive alert notifications via email when anomalies are detected.

## Contributing

Contributions to NGIDS are welcome! If you encounter any issues or have suggestions for improvements, please submit a pull request or open an issue on the GitHub repository.

## License

NGIDS is released under the MIT License. Feel free to use, modify, and distribute the code as permitted by the license.

## Acknowledgments

NGIDS is built using various open-source libraries and tools. We would like to acknowledge the developers and contributors of these projects for their valuable work.

## Disclaimer

NGIDS is provided as-is without any warranties or guarantees. The developers and contributors of NGIDS are not responsible for any damages or consequences resulting from the use or misuse of this software. Use NGIDS at your own risk.

## Installation

To run NGIDS, follow these steps:

1. Clone this repository to your local machine.
2. Open a terminal and navigate to the cloned NGIDS directory.
3. Install the required Python dependencies by running the following command:

   ```shell
   pip install -r requirements.txt
   ```
 4. Navigate to the NGIDS Core folder.

5. Open two separate terminals and execute the following commands in each terminal:
   ```shell
   python NGIDS_Core.py
   ```
    ```shell
    python NGIDS_User_Auth.py
    ```
    (Make sure no other programs are running on ports 8080 and 8888.)
6. Go to the NGIDS Client folder and either run the NGIDS Client.exe file or the NGIDSClient.pyw file.
7. Sign up using your credentials and then log in using the same credentials.
8. Click on the "Capture" button to start capturing network traffic data.
9. Access the dashboard to monitor real-time anomaly detection results.

###### Note: Ensure that you have the required dependencies installed and configured properly, and the MongoDB connection details are correctly provided for seamless operation of NGIDS.
