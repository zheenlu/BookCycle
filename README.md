# Project Overview

This project demonstrates a web application consisting of a login page and a home page, highlighting the benefits of using Docker for deploying a full-stack application. The application is designed to showcase high performance, high load, and high availability.

## Key Features

- **Docker Integration**: The project utilizes Docker containers to deploy the frontend, backend, MySQL, and Redis, enabling efficient testing and management of different service nodes.
- **Load Balancing with Nginx**: Nginx is used to distribute traffic across multiple server nodes, enhancing the app's responsiveness and reliability.
- **High Availability with Keepalived**: Implementing Keepalived ensures that if one server node fails, another node can seamlessly take over, providing continuous service without interruption.
- **Clustering for Performance and Reliability**: 
  - Multiple database clusters are deployed to handle a high volume of requests, significantly improving speed.
  - In case of a node failure, other nodes in the cluster are readily available to take over, ensuring uninterrupted operation.

## Application Screenshots

### Login Page
![Screenshot 2024-03-19 at 7 11 31 AM](https://github.com/zheenlu/docker_K8S/assets/121406160/50e8a59d-6eea-4032-87e1-76cffb181262)

### Home Page
![Screenshot 2024-03-19 at 7 11 55 AM](https://github.com/zheenlu/docker_K8S/assets/121406160/ccf2e07b-cde9-44b8-a164-b2714a99ca97)

## Docker Node Testing

Testing the application involves pausing a few nodes within the Docker environment to simulate real-world scenarios.

- **Database Cluster**: With 5 nodes, pausing 2 demonstrates continued functionality.
 ![Screenshot 2024-03-19 at 7 14 22 AM](https://github.com/zheenlu/docker_K8S/assets/121406160/791f804d-00a8-4751-8f2c-becd304c15f9)

- **Redis Cluster**: Out of 6 nodes, pausing 2 showcases resilience.
 ![Screenshot 2024-03-19 at 7 15 19 AM](https://github.com/zheenlu/docker_K8S/assets/121406160/5d996afc-1025-4e12-b9f0-c9309aac889f)

- **Backend Services**: Pausing 1 out of 3 nodes tests backend reliability.
 ![Screenshot 2024-03-19 at 7 15 19 AM](https://github.com/zheenlu/docker_K8S/assets/121406160/692dcdcd-8366-4922-a4a7-3280a6af0466)
 
- **Frontend Services**: Testing by pausing 1 out of 3 nodes for frontend responsiveness.
 ![Screenshot 2024-03-19 at 7 16 35 AM](https://github.com/zheenlu/docker_K8S/assets/121406160/780f386d-ed42-46c5-9366-eb743ab1834f)


## Conclusion

Even with several nodes paused, the application maintains its functionality, allowing users to reload the home page and log in successfully. This resilience is due to the effective use of clustering, ensuring that other available nodes can compensate for any downtime, thus demonstrating the robustness of high performance, high load, and high availability in this application.
![Screenshot 2024-03-19 at 7 17 21 AM](https://github.com/zheenlu/docker_K8S/assets/121406160/1ac192c5-b38a-42d9-9d36-5932c1851a06)
![Screenshot 2024-03-19 at 7 17 44 AM](https://github.com/zheenlu/docker_K8S/assets/121406160/2317df08-1197-4962-9c46-4f4cb2d643be)

