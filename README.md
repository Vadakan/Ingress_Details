# Ingress_Details

# Why do we need to use ingress when we have 'node port' and 'load balancer' options.?  
# 1) 'node port' is not a good option to use in production.
# 2) also for every service we cannot create 'load balancers' because load balancers are very expensive thing to handle
# 3) Also when we use 'node port' we have to use port number range of 30000 and we have to use the same in our URL as well. It is not good thing
#   to provide URL with port number to clients for accessing our websites. 

# Above are the main reasons,we have to use 'ingress' router.


![image](https://user-images.githubusercontent.com/80065996/164913413-3b856300-223f-430b-ab7c-4575be28bb21.png)


![image](https://user-images.githubusercontent.com/80065996/164913478-1988bcd0-d33d-40bc-99ef-6e89f0495197.png)


![image](https://user-images.githubusercontent.com/80065996/164913524-d491e89e-9505-47bf-9963-12a13ae440e5.png)


# As shown in below diagram, 'ingress' is the abstraction layer which hides all the services. ingress will have routing rules, which is just a map with 'domain names and their corresponding services' so that when incoming requests want to access the particular domain, the corresponding services will get hit based on mapping present in the ingress mapping.


![image](https://user-images.githubusercontent.com/80065996/164914683-2cbc9f45-5f95-43d7-ac54-ffe0dedb8c6e.png)


