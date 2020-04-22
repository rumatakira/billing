Phalcon PHP framework was chosen as the main programming language for the core API because it is an open source full stack framework for PHP, written as a C-extension. Phalcon is optimized for high performance. Its unique architecture allows the framework to always be memory resident, offering its functionality whenever it’s needed, without expensive file stats and file reads that traditional PHP frameworks employ.

Messaging between components of the system will be made on the classic RabbitMQ.

Database: MySQL cluster 7.6 (MySQL server 8.0).

API structure - written in Swagger (OpenAPI 2.0). This avoids errors by different programmers, generates clean well-documented code and API documentation.

Frontend: Symfony 5 - all you need "from box".

Incoming server and balancer - Nginx. Websockets are allowed.

Scaling: all system components are assembled in LXC containers. The idea of ​​scaling comes down to the fact that as customers grow, system will consistently move to more powerful servers whith preserving the structure of containers, and later spread the containers to separate servers.