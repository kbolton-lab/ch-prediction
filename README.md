# CH Prediction Website

## Overview
This application processes CSV data files, performs predictions using pre-trained models, and ranks the risk scores for various genes.

## Docker Image Deployment

### Pulling the Docker Image
Pull the latest Docker image from Docker Hub using the following command:
```bash
docker pull duct/chprediction:latest
```
### Running the Docker Container
Run the Docker container with the following command:
```bash
docker run --rm -p 8180:8180 duct/chprediction:latest
```
The app will be accessible at [http://localhost:8180](http://localhost:8180) on your web browser.

## Data requirements
The application requires a CSV file with the following columns:
- **id**: ID of the participant.
- **age**: Age of the participant.
- **sex**: Sex of the participant. Possible values include: M, F.
- **race**: Race of the participant. Possible values include: White, Black, Asian, Other, Missing.
- **smoking_status**: Smoking status of the participant. Possible values include: 0 (non-smoker), 1 (smoker).
- **anc**: Absolute neutrophil count (10^9 cells/L).
- **alc**: Absolute lymphocyte count (10^9 cells/L).
- **amc**: Absolute monocyte count (10^9 cells/L).
- **hgb**: Hemoglobin concentration (g/dL).
- **mcv**: Mean corpuscular volume (fL).
- **rdw**: Red blood cell distribution width (%).
- **plt**: Platelet count (10^9 cells/L).
