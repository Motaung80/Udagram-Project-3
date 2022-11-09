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
![Picture22](https://user-images.githubusercontent.com/86393854/200703569-e7992b8c-6fa5-409f-99c2-f5886a730ba8.png)
![Picture23](https://user-images.githubusercontent.com/86393854/200703591-ddd28d86-7d40-4bdb-805e-49575a6a5085.png)
![Picture24](https://user-images.githubusercontent.com/86393854/200703606-d1e3570b-77f4-4440-a37e-9c6a1f626c6b.png)





* To verify that you have set up logging with a backend application
```bash
kubectl logs {pod_name}
```
![Picture25](https://user-images.githubusercontent.com/86393854/200703614-f9079e85-3275-4cfa-8375-c4b03381bad2.jpg)

