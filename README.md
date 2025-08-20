# cartera_empleo

Modernización del portal: Next.js (frontend), Spring Boot (API), PostgreSQL, OpenSearch y Keycloak.

## Arranque rápido
1. cd infra && docker compose up -d
2. cd ../backend/jobs-service
   - mvn -q -DskipTests package
   - DB_HOST=localhost DB_PORT=5432 DB_NAME=empleo DB_USER=empleo DB_PASS=empleo java -jar target/jobs-service-0.0.1-SNAPSHOT.jar
3. cd ../../frontend/portal-empleo
   - npm install
   - npm run dev

Swagger: http://localhost:9090/swagger-ui/index.html
Front: http://localhost:3000