# Credit Card Fraud Detection System

A full-stack Django application that combines e-commerce functionality with real-time fraud detection to identify suspicious online transactions before payment authorization.

## Overview

Online payment systems are vulnerable to fraudulent transactions caused by account compromise, unusual spending behavior, and location-based anomalies. This project implements a rule-based Fraud Detection System (FDS) that evaluates transaction risk using behavioral profiling and IP-based geolocation analysis.

The system integrates fraud screening directly into the checkout workflow, allowing suspicious transactions to be flagged before payment processing.

## Key Features

* Real-time transaction risk assessment
* Behavior-based anomaly detection
* IP-based geolocation verification using ipinfo.io
* Stripe payment integration
* Secure user authentication and account management
* Shopping cart and checkout workflow
* Order tracking and payment history
* Fraud scenario simulation and testing

## Fraud Detection Logic

The fraud detection engine evaluates transactions using multiple signals:

### Behavioral Analysis

* Learns historical user spending patterns
* Calculates an expected spending range for each user
* Flags transactions that significantly exceed normal behavior

### Location Verification

* Retrieves transaction location using IP intelligence
* Compares current location with expected user activity
* Generates risk alerts for unusual geographic patterns

### Risk-Based Decision Making

* Normal transactions proceed through payment authorization
* Suspicious transactions are flagged for review
* Multiple risk signals are combined before a decision is made

## Tech Stack

### Backend

* Django
* Python
* SQLite
* Stripe API

### Frontend

* HTML
* CSS
* JavaScript

### External Services

* ipinfo.io API
* Stripe Payments

## Project Structure

```text
core/           # Business logic and fraud detection
templates/      # Frontend templates
static_in_env/  # Static assets
djecommerce/    # Django project configuration
```

## Future Improvements

* Machine Learning-based fraud detection
* Device fingerprinting
* Risk scoring models
* Transaction analytics dashboard
* Multi-factor authentication
* Real-world fraud dataset evaluation

## Learning Outcomes

Through this project, I gained practical experience with:

* Full-stack web development using Django
* Payment gateway integration
* Fraud detection concepts
* Risk-based decision systems
* API integration
* Secure application development

## Disclaimer

This project is intended for educational and demonstration purposes. The fraud detection mechanism is rule-based and is not intended to replace production-grade financial risk systems.
