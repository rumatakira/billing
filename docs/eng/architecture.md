API structure - written in Swagger (OpenAPI 2.0). This avoids errors by different programmers, generates clean well-documented code and API documentation.

Site backend: Symfony 5 - all you need "from box".

API backend: RAW PHP with PeactPHP, symfony/routing. These are speeds same to Node.js backend.

Database: MySQL cluster 7.6 (MySQL server 8.0).

Incoming server ReactPHP, Websockets are allowed. Balancer - Nginx.

Messaging between components of the system will be made on the NATS MQ.

Scaling: all system components are assembled in LXC containers. The idea of ​​scaling comes down to the fact that as customers grow, system will consistently move to more powerful servers whith preserving the structure of containers, and later spread the containers to separate servers.
