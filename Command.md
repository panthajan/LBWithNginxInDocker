
=========How LB Nginx Work In Docker==========

Docker Image  build Command: 
1. App1: $docker build -t app1 .
2. App2: $docker build -t app2 .
3. LB:  $docker build -t lb .

Docker Container Run Command:

1. App1: $docker run -d app1
2. App2: $docker run -d app2
3. LB: Command for Run LB on Host Machine:

$docker run -it --rm -d -p 8087:80 lb

Here 8087 is Host Port and 80 is lb container space port
==========================================================
We can access LB through>>>http://localhost:8087/

Result on First HIT in Host Browser: 

![image](https://user-images.githubusercontent.com/19544130/221406504-715b5dc1-e4a4-4b93-ac8e-30762863f806.png)


Result on Second HIT in Host Browser: 

![image](https://user-images.githubusercontent.com/19544130/221406584-0773092b-ca00-4b08-9539-8c8aa2849338.png)

Result on Third HIT in Host Browser:

![image](https://user-images.githubusercontent.com/19544130/221784253-81533956-d0e4-4536-894c-f099dff015d6.png)
