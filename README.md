docker run --name demo-auth-db -p 5433:5432 -e POSTGRES_DB=demo-auth-db -e POSTGRES_USER=admin -e POSTGRES_PASSWORD=123456 postgres:11 -d
docker run --name demo-product-db -p 5434:5432 -e POSTGRES_DB=demo-product-db -e POSTGRES_USER=admin -e POSTGRES_PASSWORD=123456 postgres:11 -d
docker run --name sales-db -d -p 27017:27017 -p 28017:28017 -e MONGODB_USER="admin" e MONGODB_DATABASE="sales-db" -e MONGODB_PASS="123456" tutum/mongodb
