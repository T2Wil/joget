# Joget

## Architecture Diagram
<img width="856" alt="image" src="https://github.com/T2Wil/joget/assets/30593186/79586ffe-ca02-43dd-b33f-5365c8c90caa">


## CI/CD
<img width="927" alt="image" src="https://github.com/T2Wil/joget/assets/30593186/04898a1a-fa3b-49eb-9b07-74a07070a47b">

## Considerations to make application scalable and manageable. 
- Configured `horizontal scaling` by running multiple instances Joget and added HAProxy for loadbalancing efficient loadbalancing of the requests
- Used `.env` for ease management of the codebase. Useful in multiple environments scenario.
- Set `resource constraints` on your Docker containers to prevent resource contention and ensure that the application operates within defined resource boundaries. This is crucial for efficient scalability.
- Utilize `Docker volumes for persistent data storage`. Mounting volumes allows you to separate data from the container, making it easier to scale instances without worrying about data loss.
- Health checks are implemented on LB to only forward traffic to live instances.
