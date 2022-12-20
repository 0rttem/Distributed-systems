# Distributed-systems (Replicated log)
The laboratory works of distributed systems in Kyiv Polytechnic Institute

Selfcheck acceptance test
1. create bridge-network dist_systems_lab_network:
```
docker network create -d bridge dist_systems_lab_network
```
2. initialize Master:
```
docker run -it --rm --network=dist_systems_lab_network -v$(pwd):/home -w/home --name Master python:3 bash
pip3 install sortedcontainers
```
3. initialize Secondary1:
```
docker run -it --rm --network=dist_systems_lab_network -v$(pwd):/home -w/home --name Secondary1 python:3 bash
pip3 install sortedcontainers
```
4. initialize Client1:
```
docker run -it --rm --network=dist_systems_lab_network -v$(pwd):/home -w/home --name Client1 python:3 bash
```
5. in Master run ```Master.py```, in Secondary1 run ```Secondary1.py```







