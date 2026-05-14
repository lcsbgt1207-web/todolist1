Sprint 10 — Monitoring Grafana

Description:
Mise en place d'un dashboard de monitoring Grafana connecté à SonarCloud pour visualiser en temps réel la qualité du code du projet todolist1.

Liens:
Dashboard Grafana : https://lcsbgt1207web.grafana.net/public-dashboards/5c59aea78ce1484dba505dc6211d7325
Projet SonarCloud : https://sonarcloud.io/project/overview?id=lcsbgt1207-web_todolist1

Configuration:
Datasource : JSON API connectée à https://sonarcloud.io/api via Bearer Token SonarCloud.
Chaque panneau est de type Gauge. La valeur est extraite via JSONPath $.component.measures[0].value sur l'endpoint /measures/componen
