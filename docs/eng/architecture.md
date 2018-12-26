First of all, single-threaded systems were deleted from consideration. We had to choose between Erlang, Golang and Rust.
Golang was chosen as the main programming language because it is difficult to find Erlang programmers, although stability and hot-swappable code went to Erlang plus. Rust, in spite of the formal lack of a race condition, is still more suitable not for writing applications, but for drivers and operating systems.

Messaging between components of the system made not on the classic RabbitMQ, but on NATS - the latter benchmarks on the server that is currently used, showed 1M messages (+ 360K in clustering) per second against 40K by RabbitMQ. Besides NATS clustered faster and easier than RabbitMQ.

Database: MySQL cluster 7.6 (MySQL server 8.0).

API - written in Swagger (OpenAPI 2.0). This avoids errors by different programmers, generates clean well-documented code and API documentation. Unfortunately, Swagger uses [gorilla/mux] (https://github.com/gorilla/mux) by default for routing, but after generating the entire API, the routing will be rewritten to [kataras/muxie] (https://github.com / kataras / muxie) - it is twice faster.

Frontend: between Iris, Beego and Revel - selected [Revel] (https://revel.github.io/). Slower than Iris, but everything is out of the box, including integration with graphics. The main load will still be carried by the API.

Scaling: all system components are assembled in LXC containers, now they are preceded by a HAProxy balancer. The idea of ​​scaling comes down to the fact that as customers grow, system will consistently move to more powerful servers whith preserving the structure of containers, and later spread the container to separate servers, replacing HAProxy with NATS. In addition to the classic hardware scaling, there is always the possibility to increase the amount of goroutine inside the containers handling requests to the API and the site. Although this process, as practice has shown, has logical limitations.