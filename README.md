# Smart India Hackathon Workshop
# Date:21.09.2025
## Register Number:25010044
## Name:Pavan Kalyan. P
## Problem Title
SIH 25010: Smart Crop Advisory System for Small and Marginal Farmers
## Problem Description
A majority of small and marginal farmers in India rely on traditional knowledge, local shopkeepers, or guesswork for crop selection, pest control, and fertilizer use. They lack access to personalized, real-time advisory services that account for soil type, weather conditions, and crop history. This often leads to poor yield, excessive input costs, and environmental degradation due to overuse of chemicals. Language barriers, low digital literacy, and absence of localized tools further limit their access to modern agri-tech resources.

Impact / Why this problem needs to be solved

Helping small farmers make informed decisions can significantly increase productivity, reduce costs, and improve livelihoods. It also contributes to sustainable farming practices, food security, and environmental conservation. A smart advisory solution can empower farmers with scientific insights in their native language and reduce dependency on unreliable third-party advice.

Expected Outcomes

• A multilingual, AI-based mobile app or chatbot that provides real-time, location-specific crop advisory.
• Soil health recommendations and fertilizer guidance.
• Weather-based alerts and predictive insights.
• Pest/disease detection via image uploads.
• Market price tracking.
• Voice support for low-literate users.
• Feedback and usage data collection for continuous improvement.

Relevant Stakeholders / Beneficiaries

• Small and marginal farmers
• Agricultural extension officers
• Government agriculture departments
• NGOs and cooperatives
• Agri-tech startups

Supporting Data

• 86% of Indian farmers are small or marginal (NABARD Report, 2022).
• Studies show ICT-based advisories can increase crop yield by 20–30%.

## Problem Creater's Organization
Government of Punjab

## Theme
Agriculture, FoodTech & Rural Development

## Proposed Solution
It starts with farm registration and profile management, wherein information like name, landhold, location-based GPS-based coordinates, soil type, crop history, and language choice are stored in a safe manner. Registered, the process of collecting data and integrating is made simple by importing location-based weather data from APIs such as OpenWeather and IMD feeds, soil data from IoT sensors or government soil health cards, and market price data from APMC portals and government websites.
At the center is the crop suggestion and input engine that uses AI/ML algorithms to offer appropriate crops based on season, climate, and soil. It also gives accurate fertilizer and pesticide recommendations, including organic fertilizer and pesticide recommendations, and creates irrigation schedules by utilizing a combination of weather forecast and soil water level. For convenience, the support advisory system provides support through a multilingual chat interface with text and voice interfaces, native-language speech-to-text and text-to-speech functionality, and escalation to human experts in case farmers need more assistance.
The system also includes a pest and disease identification module, where farmers can upload photos of crops that are scanned through computer vision models (CNNs developed using TensorFlow or PyTorch and OpenCV). Based on the diagnosis, the system prescribes remedies that are either organic or chemical. This is complemented by warnings and notifications, which send timely warnings of weather activities like rainfall, drought, or frost, indicating outbreaks of pests and fluctuations in market prices. Lastly, a learning and feedback loop enables farmers to score the value of the advice, and that information is taken back into the ML algorithms to get more accurate and personalized with time.


## Technical Approach
Technically, the application will be developed on React Native or Flutter as the mobile client, with Python (FastAPI or Django REST Framework) and Node.js being the backend to integrate with chatbots. The data will be stored with PostgreSQL for time-series crop and farmer data and MongoDB for weather and sensor data. AI/ML layer will employ TensorFlow, PyTorch, and Scikit-learn for yield estimation, pest detection, and crop recommendation. IoT integration will be done through MQTT brokers such as Mosquitto and LoRaWAN/GSM modules for remote area connection. For language and chatbot support, technologies like Rasa or Dialogflow will be utilized, and Google Speech-to-Text and Text-to-Speech APIs for voice. The whole system will be deployed on cloud scalable platforms like AWS, Azure, or GCP.

The logical flow of the system starts with farmer registration, location, soil, weather, and market data capture. This is passed on to the crop recommendation engine, which responds accordingly in terms of advisory via mobile app, SMS/IVR for low-literacy farmers, or human experts in the event of escalation. The subsequent steps are detection of pest and disease, alerts and notifications, feedback from the farmer and data logging, and retraining of ML model for ongoing improvement.

![alt text](<flowchart.jpeg>)

## Feasibility and Viability
In the feasibility aspect, the solution is viable as it uses established open-source platforms, cost-effective cloud infrastructure, and inexpensive IoT kits. The biggest challenges are connectivity gap, digital literacy barrier, and sensor maintenance. These can be addressed by offline-first app architecture, SMS/IVR fallback mechanisms, and sensor maintenance support from local cooperatives.

## Impact and Benefits
The advantages are enormous: the farmers will realize a 20–30% increase in their overall yield, lower input costs in terms of reduced consumption of fertilizer and pesticides, ease through advisory in local languages, and long-term environmental stability through precision farming methods.


## Research and References
<h3>Remove These Lines</h3>
<ul><li>Details / Links of the reference and research work</li></ul>
