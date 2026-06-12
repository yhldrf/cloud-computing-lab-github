# Lab7 Experiment Record

- Experiment: Containerization with Docker
- Repository: https://github.com/whatokk/lab7-containerization-with-docker
- Successful Actions run: https://github.com/whatokk/lab7-containerization-with-docker/actions/runs/27258893987
- Docker image: cloud-lab-image:v1
- Image size: 62.3MB
- Main container: my-web-container, mapped host port 8080 to container port 80
- Second container: second-container, mapped host port 8081 to container port 80
- Port conflict: reproduced by trying to bind another container to host port 8080
- Cleanup: docker ps returned no running containers after stopping/removing instances
- Generated at: 2026-06-10 15:00:52 +08:00

## Key Results

The Nginx Alpine Docker image was built successfully. The web page was reachable through port 8080. After editing the source file, the running container did not change, proving image/container immutability. Container filesystem isolation was verified with docker exec. Runtime stats showed the web server using about 10.39MiB memory. Scaling to a second instance worked on port 8081, while reusing port 8080 caused the expected port allocation error.
