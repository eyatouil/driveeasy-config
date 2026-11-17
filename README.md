# driveeasy-config

Dépôt Git lu par le **Config Server** (`driveeasy-backend/config-server`).
Un fichier par service, plus `application.yml` partagé.

| Fichier | Contenu |
|---|---|
| `application.yml` | Eureka, Actuator, Zipkin (commun à tous) |
| `vehicule-service.yml` | port 8081, propriétés métier |
| `client-service.yml` | port 8082, seuils de fidélité, âge minimal |
| `location-service.yml` | port 8083, remises, pénalité de retard |
| `api-gateway.yml` | port 8080, routes `lb://`, CORS |

Vérification : `http://localhost:8888/vehicule-service/default`
