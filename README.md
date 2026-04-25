# Trip-Estimation-Service

• Integrated Nominatim (geocoding) and OSRM (routing) APIs into a unified service layer, abstracting third-party
complexity and shielding consumers from external schema changes through a single, clean endpoint.
• Utilized Java 17 Records for immutable DTOs to minimize boilerplate and memory overhead
• Implemented a DAO layer with JPA/Spring Data Repositories for persistent trip data management.
• Applied SOLID principles to decouple business logic from external dependencies, utilizing a dedicated transformation
layer for coordinate conversions and unit rounding to ensure high testability.
• Leveraged OpenFeign for declarative REST communication, implementing custom connection pooling and read
timeouts to prevent thread exhaustion and ensure service stability during API outages.
• Engineered a Global Exception Handler to intercept domain failures, delivering standardized, well-structured HTTP
responses across the microservice to improve reliability for downstream consumers.
