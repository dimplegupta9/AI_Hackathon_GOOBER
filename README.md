# GOOBER - Smart Garbage Collection System

## Overview
An intelligent waste management solution that leverages Azure cloud services and Microsoft Fabric to automate garbage collection requests through image classification and real-time location tracking.

## Features
- Automated garbage detection using machine learning
- Real-time location tracking and coordinate conversion
- Seamless communication between citizens and garbage collectors
- Comprehensive monitoring and reporting system
- Cloud-native architecture with scalable components

## Architecture
The system consists of the following components:
- User & Garbage Collector Web Applications (Azure App Service)
- Azure Functions (HTTP & Service Bus triggers)
- Microsoft Fabric EventStream
- KQL Database
- Microsoft Fabric Lakehouse
- Image Classification Model
- Power BI Reports

## Prerequisites
- Azure subscription
- Microsoft Fabric workspace
- OpenCage API key
- Node.js (for web applications)
- Python 3.8+ (for ML components)

## Setup Instructions

### Azure Resources
1. Create Azure Function App
2. Set up Azure App Service
3. Configure Service Bus
4. Create KQL Database

### Microsoft Fabric Setup
1. Create workspace
2. Configure EventStream
3. Set up Lakehouse
4. Import ML notebooks and experiments

### Web Applications
Clone the repository
```bash
git clone https://github.com/dimplegupta9/AI_Hackathon_GOOBER/
```

## Usage

### User Application
1. Access the web application
2. Click to capture image of garbage
3. System automatically:
   - Captures location
   - Processes image
   - Sends notification if garbage is detected

### Garbage Collector Application
1. Receive notifications of new requests
2. View request details and location
3. Submit cleanup verification

### Admin Dashboard
1. Access Power BI reports
2. Monitor collection status
3. Generate performance metrics

## Project Structure
```
├── azure-functions/
│   ├── HttpTrigger/
│   └── ServiceBusTrigger/
├── web-apps/
│   ├── user-app/
│   └── collector-app/
├── ml-notebooks/
│   ├── preprocessing/
│   └── model-training/
├── powerbi/
│   └── reports/
└── docs/
```

## Contributing
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## Acknowledgments
- Microsoft Azure Documentation
- Microsoft Fabric Team
- OpenCage API Documentation

## Support
For support, please open an issue in the GitHub repository or contact the development team.
