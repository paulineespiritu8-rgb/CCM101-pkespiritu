# MinIO Deployment

## Docker Command

I deployed the MinIO object storage server using Docker with the following command:

```bash
docker run -d -p 9000:9000 -p 9001:9001 \
--name minio-server \
-e "MINIO_ROOT_USER=cloudadmin" \
-e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
minio/minio server /data --console-address ":9001"

## Web Console Port

The MinIO Web Console was accessed through port 9001 using the Traffic/Ports option in the KillerCoda Playground.

## Bucket Created

The bucket I created was named client-photos. This bucket was used to store the sample file uploaded during the activity.

## Environment Variables

The -e flags in the Docker command were used to set the login credentials for the MinIO server.

MINIO_ROOT_USER=cloudadmin sets the root username for the MinIO server.
MINIO_ROOT_PASSWORD=CloudNova2026! sets the root password for the MinIO server.

These environment variables provide the username and password that MinIO uses when accessing the Web Console.
