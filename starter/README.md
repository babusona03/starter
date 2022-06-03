# Build
mvn clean package && docker build -t learn.ee/starter .

# RUN

docker rm -f starter || true && docker run -d -p 8080:8080 -p 4848:4848 --name starter learn.ee/starter 