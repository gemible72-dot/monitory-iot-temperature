# Surveillance de la température IoT

## Description
Ce projet utilise **Node-RED** pour collecter des données de température via MQTT, les stocker dans **InfluxDB** et les visualiser sur **Grafana**.

## Architecture Technique
* **Node-RED** : Logique de récupération et d'envoi (fichier `flows.json`).
* **InfluxDB** :capteur_iot
  * **Port** : 8086
* **Grafana** : Dashboard de visualisation (fichier `dashboard.json`).

## Instructions
1. Importer `flows.json` dans Node-RED.
2. Créer le bucket dans InfluxDB.
3. Importer `dashboard.json` dans Grafana en liant la source InfluxDB.
