COMMANDS:

#Stop the container called test if that is running
docker rm -f test 

#Build the image named test:
docker build -t test .

#Start the container:
docker run -d -p 8080:80 -p 2222:2222 --name test test

#Test API:
curl http://localhost:8080/WeatherForecast

#Test
ssh root@127.0.0.1 -p 2222 -c aes128-cbc
The default root password is: Docker!

