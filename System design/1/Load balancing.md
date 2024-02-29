***Definition

Load balancing is the process of evenly distributing incoming network traffic, workload, or requests across multiple servers, nodes, or resources to optimize resource utilization, maximize throughput, ensure high availability, and improve overall system performance
Take a look here to see [[Load Balancing Draw]].

Why load balancing in system design ?

***Resource Utilization**:

Load balancing ensures that resources such as CPU, memory, disk I/O, and network bandwidth are evenly distributed across multiple servers or nodes in a system. This prevents some servers from being overwhelmed while others remain underutilized, thus optimizing resource utilization.

***Scalability**: 

Load balancing enables systems to scale horizontally by adding more servers or nodes to handle increased traffic or workload. When new servers are added, the load balancer distributes incoming requests among them, allowing the system to handle more users or process more data without experiencing performance degradation.

***High Availability**:

Load balancers can distribute traffic across redundant servers, ensuring that if one server fails or becomes unavailable, others can continue to handle incoming requests. This improves system reliability and availability by minimizing downtime and ensuring continuous service availability.

***Improved Performance**:

By evenly distributing requests among servers, load balancing can help reduce response times and improve overall system performance. Users experience faster response times and better throughput because requests are processed efficiently across multiple servers.

***Traffic Management**:

Load balancers can route traffic based on various criteria such as server health, geographic location, or type of request. This enables more sophisticated traffic management strategies, such as prioritizing certain types of requests or directing users to the nearest server for improved latency.

***Fault Tolerance**:

Load balancers can detect and mitigate failures in the system by rerouting traffic away from unhealthy or overloaded servers. This helps prevent cascading failures and ensures that the system remains operational even in the face of individual component failures.

***The 5 famous algorithms used in load balancing

**[[Round Robin]]** 

This algorithm distributes incoming requests evenly among a set of servers in a circular order. Each new request is assigned to the next server in the sequence. Round Robin is simple to implement and ensures an equal distribution of load across servers, but it may not take into account server capacity or current load.

**[[Weighted Round Robin]]**

Similar to Round Robin, but allows assigning different weights to servers based on their capacity or performance. Servers with higher weights receive a proportionally larger share of requests, allowing for more efficient resource utilization.

**[[Least Connection]]**

This algorithm directs incoming requests to the server with the fewest active connections at the time of the request. It aims to distribute load based on current server load rather than just the number of requests, which can be beneficial for applications with long-running connections or varying request processing times.

**[[Least Response Time]]**

This algorithm routes requests to the server with the shortest response time or lowest latency. It requires measuring response times for each server and dynamically adjusting routing decisions based on real-time performance metrics.

**[[IP Hash]]**

In this algorithm, the client's IP address is used to determine which server should handle the request. By hashing the client's IP address and mapping it to a specific server, IP Hash ensures that requests from the same client are consistently routed to the same server, which can be useful for maintaining session affinity or caching strategies.