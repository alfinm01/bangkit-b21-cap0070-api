# Nutrition Analyzer API

## Bangkit Project 2021

API endpoints integrated with Keras ML model to provide food detection and nutrition analysis from uploaded image\
The service is accessible on [http://34.101.205.136:5000/](http://34.101.205.136:5000/)\
Deployed using Compute Engine on Google Cloud Platform (GCP)

## Team B21-CAP0070
1. Muhammad Faishal Ammar Wibowo (A0101051)
2. Muhamad Lutfi Arif (A0101025)
3. Alfian Maulana Ibrahim (C0020060)
4. Andhika Fachri Ramadhan (C1071411)
5. Naradita Kunti Nabila (M0020059)
6. Hana Raissya (M0101024)

## Endpoint API

|Method | Endpoint | Body | Description | Return
|--|--|--|--|--|
| Get | / | - | Service health check | Ok message
| Post | /predict | image (Form data: .jpg, .jpeg, .png) | Get top 3 most relevant food name and nutritions | Json array of food
| Post | /detect-text | image (Form data: .jpg, .jpeg, .png) | Get text from image | Json of text contained on image
| Post | /detect-image | image (Form data: .jpg, .jpeg, .png) | Get relevant name of image | Json of names or description