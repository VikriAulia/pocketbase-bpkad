## Docker Pocket Base Image
### Build image with this command
```bash
docker build -t pocketbase-3004 .
```

### Run with this command if you want to persist pb_data
```bash
docker run -d -p 3004:8080 -v pb_data:/pb/pb_data/ --name pocketbase-3004 pocketbase-3004 
```

### Same command with explanation
```bash
# Run a detached Pocket Base container
docker run -d \
  # Map port 3004 on the host to port 8080 inside the container
  -p 3004:8080 \
  # Mount the host directory 'pb_data' to '/pb/pb_data/' inside the container
  -v pb_data:/pb/pb_data/ \
  # Assign a name to the container
  --name pocketbase-3004 \
  # Use the 'pocketbase-3004' image
  pocketbase-3004
```
