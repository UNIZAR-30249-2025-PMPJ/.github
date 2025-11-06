# UNIZAR-30249-2025-PMPJ
This GitHub organization hosts the ByronHub project, developed by students of the University of Zaragoza as part of the Software Engineering Laboratory course (2025 edition). ByronHub is a modular and scalable web application for managing space reservations in the Ada Byron building.
## Project Overview
ByronHub enables users to:

- Search and reserve rooms via an interactive map.
- Manage their bookings and receive notifications.
- Access role-based features (e.g., managers can modify users, spaces, and reservations).
- The system is built using a hexagonal architecture and follows Domain-Driven Design (DDD) principles. It integrates geospatial data visualization, asynchronous communication, and layered deployment.

## Architecture
The system is divided into four tiers:

- TIER_NAV: Frontend application using React.js and Leaflet.
- TIER_WEB: API Gateway built with Express.js (Node.js).
- TIER_APP: Backend business logic implemented in Node.js with TypeScript.
- TIER_DB: PostgreSQL database with PostGIS extension.
Communication between tiers is asynchronous via RabbitMQ. The frontend uses PyGeoAPI for geospatial services.

## Repositories

|Repository|	Description|
|---|---|
|[TIER_NAV](https://github.com/UNIZAR-30249-2025-PMPJ/TIER_NAV)|	Frontend UI with interactive map and user interfaces.|
|[TIER_WEB](https://github.com/UNIZAR-30249-2025-PMPJ/TIER_WEB)|	API Gateway for routing, authentication, and messaging.|
|[TIER_APP](https://github.com/UNIZAR-30249-2025-PMPJ/TIER_APP)|	Core backend logic, domain model, and business rules.|
|[TIER_DB](https://github.com/UNIZAR-30249-2025-PMPJ/TIER_DB)|	Database schema, migrations, and setup scripts.|
|[ByronHub](https://github.com/UNIZAR-30249-2025-PMPJ/ByronHub)|	Docker Compose setup for local deployment.|

## Documentation

- API Docs: Swagger Web API
- Async API Docs: RabbitMQ Interface
- Test Coverage: Jest Report
- Sequence Diagram: Reservation Flow

## Testing

- Integration and unit tests implemented using Jest.
- CI/CD pipeline configured with GitHub Actions.
- Manual testing via Postman and frontend review.

## Deployment

- Local: Docker Compose setup available in the ByronHub repository.
- Cloud: AWS EC2 instances for backend and frontend, Railway for frontend hosting, Nginx and Certbot for HTTPS.

## Team

Miguel Aréjula 
Pablo Angusto 
Johan Xu 
Pablo Calvo 


