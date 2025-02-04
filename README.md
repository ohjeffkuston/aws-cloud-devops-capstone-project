# DevOps QR Code Project

This repository contains a sample application for the DevOps Capstone Project. It includes a QR code generator for provided URLs, with a front-end built using Next.js and an API developed with FastAPI in Python.

## Application Overview

**Front-End**: A web interface where users can input URLs.

**API**: An API that accepts URLs and generates QR codes, storing them in an AWS S3 bucket.

## Running Locally

### API

The API code is located in the `api` directory. To run the API server locally:

- Clone this repository.
- Navigate to the `api` directory.
- Create a virtual environment: `python -m venv .venv`
- Install the required packages: `pip install -r requirements.txt`
- Create a `.env` file and add your AWS Access and Secret keys (refer to `.env.example`).
- Update the `BUCKET_NAME` in `main.py` to your S3 bucket name.
- Start the API server: `uvicorn main:app --reload`
- The API server will be available at `http://localhost:8000`.

### Front-End

The front-end code is in the `front-end-nextjs` directory. To run the front-end server locally:

- Clone this repository.
- Navigate to the `front-end-nextjs` directory.
- Install the dependencies: `npm install`
- Start the Next.js server: `npm run dev`
- The front-end server will be available at `http://localhost:3000`.

## Objective

The objective is to practice DevOps methodologies such as containerization, CI/CD, and monitoring.

