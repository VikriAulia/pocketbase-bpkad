## docker pocket base image

### Build image with this command
```bash
docker build -t pocketbase-3004 .


### run with this command if you want to presis pb_data

```bash
docker run -d -p 3004:8080 -v pb_data:/pb/pb_data/ --name pocketbase-3004 pocketbase-3004 

