# AI & IOT Application Platform

## Overview

This project aims to design and implement a unified application platform that supports the deployment of and interaction between applications, AI/ML models, and IoT sensors/controllers. The platform consists of multiple services accessible through a unified UI, which communicates with a request manager service acting as a secure gateway.

### User Roles

- **Data Scientist:** Can upload and deploy trained models along with configuration files.
- **Platform Configurer:** Can register new sensor/controller types and instances.
- **End Application Developer:** Can deploy applications and bind them to sensor/controller types.
- **End User:** Can view and choose deployed applications and available sensor/controller instances.

### Workflow

1. **Data Scientist:**
    - Trains a model locally and uploads it with a contract and config file.
    - The deployment service uses the config file to deploy the model as a service, accessible via an API endpoint.
2. **Platform Configurer:**
    - Registers new sensor/controller types and instances on the platform.
3. **End Application Developer:**
    - Deploys applications using the platform's deployment service.
    - Binds applications to the respective sensor/controller types via the config file.
4. **End User:**
    - Views deployed applications and available sensor/controller instances.
    - Chooses sensor instances based on preferences.

### Services

- **Sensor-Controller Service:** Manages sensors/controllers.
- **Deployment Service:** Manages the deployment of models and applications.
- **Node Manager Service:** Oversees node operations.

This platform ensures seamless interaction and deployment, providing a comprehensive solution for integrating applications, AI/ML models, and IoT sensors/controllers.

## Architecture

![Untitled](images/Architecture.png)
