# Screenshots
To help review your infrastructure, please include the following screenshots in this directory::

## Deployment Pipeline
* DockerHub showing containers that you have pushed
![Picture16](https://user-images.githubusercontent.com/86393854/200703389-8c81cc65-b86b-4345-8306-bd24ddbea7c8.png)


* GitHub repository’s settings showing your Travis webhook (can be found in Settings - Webhook)
![Picture17](https://user-images.githubusercontent.com/86393854/200703363-c738a7d8-8576-4b7e-8404-ff508e0b167b.png)


* Travis CI showing a successful build and deploy job
![Picture18](https://user-images.githubusercontent.com/86393854/200703417-98c77309-d10f-4d81-9cf1-b5374bffb302.png)

## Kubernetes
* To verify Kubernetes pods are deployed properly
```bash
kubectl get pods

```
![Picture19](https://user-images.githubusercontent.com/86393854/200703445-c241b688-7a15-4b4a-b8a2-831620a91b1a.png)

* To verify Kubernetes services are properly set up
```bash
kubectl describe services
```
![Picture20](https://user-images.githubusercontent.com/86393854/200703522-93412164-32c3-4a11-bbac-ed9d329d0686.png)
![Picture21](https://user-images.githubusercontent.com/86393854/200703545-00638071-b3c1-4e0e-9304-159b0fe96bf1.png)



* To verify that you have horizontal scaling set against CPU usage
```bash
kubectl describe hpa
```
![Screenshot (104)](https://user-images.githubusercontent.com/86393854/200855263-86bea880-b9db-4f81-9ad9-aab93671a850.jpg)

![Screenshot (105)](https://user-images.githubusercontent.com/86393854/200855389-b4e76a23-92be-48c4-8eef-c965d4d57448.jpg)




* To verify that you have set up logging with a backend application
```bash
kubectl logs {pod_name}
```

![Screenshot (202)](https://user-images.githubusercontent.com/86393854/200897049-b484d44d-ea92-4a41-b109-0f80b6123ffc.jpg)



