All connection hostnames are derived as per docker-compose.yml. Services communicate with each other using the docker network created along with service name & internal port number of the respective docker containers.

## MQTT

* Hostname: mosquitto
* Port: 1883

## HTTP Client Connection

This single connection is used for both HTTP lookups in the processor map function and also to update the current values back into postgresql via springboot api. Additional resource path values are appended to structure the GET/PUT requests

* URL: http://nginx-reverse-proxy:8080

## Processor Map HTTP Lookup Operation

* Method: GET
* Resource Path:
    * gpsinventory/
    * gpsterminalId (select is Replacement variable?)


## gpsinventory-http-put-operation (update current values back into postgresql via springboot)

Prior to the operation, there is a set properties shape to set the replacement variable via the Dynamic Document property
* Dynamic Document Property: gpsterminalId
* Derived value: JSON profile element of gpsterminalid from gpsinventory-http-req-res-profile

### PUT Operation

* Method: PUT
* Resource Path:
    * gpsinventory/
    * gpsterminalId (select is Replacement variable?)

## Set properties for Kafa topic name

* Kafka Topic name: static value of "gps"

## Kafka connection

* Broker list: kafka:9092

## Kafka publisher

* Import:  Allow dynamic topics
* Client ID: Random unique value

## Kafka consumer

* Import: 
