
=========How LB Nginx Work In Docker==========

Command for Run LB on Host Machine:

docker run -it --rm -d -p 8087:80 lb

Here 8087 is Host Port and 80 is lb container space port

Can access LB through>>>http://localhost:8087/

Result on First HIT: 

![image](https://user-images.githubusercontent.com/19544130/221406504-715b5dc1-e4a4-4b93-ac8e-30762863f806.png)


Result on Second HIT: 

![image](https://user-images.githubusercontent.com/19544130/221406584-0773092b-ca00-4b08-9539-8c8aa2849338.png)

