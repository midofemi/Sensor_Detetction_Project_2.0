# Sensor-Fault-Detection
Problem Statement
The Air Pressure System (APS) is a critical component of a heavy-duty vehicle that uses compressed air to force a piston to provide pressure to the brake pads, slowing the vehicle down. The benefits of using an APS instead of a hydraulic system are the easy availability and long-term sustainability of natural air.

This is a Binary Classification problem, in which the affirmative class indicates that the failure was caused by a certain component of the APS, while the negative class indicates that the failure was caused by something else.

Solution Proposed
In this project, the system in focus is the Air Pressure system (APS) which generates pressurized air that are utilized in various functions in a truck, such as braking and gear changes. The datasets positive class corresponds to component failures for a specific component of the APS system. The negative class corresponds to trucks with failures for components not related to the APS system.

The problem is to reduce the cost due to unnecessary repairs. So it is required to minimize the false predictions. The only difference between this repo and sensor-fault-detection is the implementation of airflow on this project


for linux:
$(pwd)/airflow/dags

docker run -p 8080:8080 -v %cd%\airflow\dags:/app/airflow/dags -e 'MONGO_DB_URL=mongodb+srv://avnish:Aa327030@cluster0.or68e.mongodb.net/?retryWrites=true&w=majority' sensor:latest 



Github Secrets:
```
AWS_ACCESS_KEY_ID=
AWS_SECRET_ACCESS_KEY=
AWS_REGION=
AWS_ECR_LOGIN_URI=
ECR_REPOSITORY_NAME=
BUCKET_NAME=
MONGO_DB_URL=
```