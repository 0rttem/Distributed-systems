# Distributed-systems (Replicated log)
The laboratory works of distributed systems in Kyiv Polytechnic Institute

Selfcheck acceptance test
1. initialize Master:
```
docker run -it --rm --network=dist_systems_lab_network -v$(pwd):/home -w/home --name Master python:3 bash
pip3 install sortedcontainers
```
2. initialize Secondary1:
```
docker run -it --rm --network=dist_systems_lab_network -v$(pwd):/home -w/home --name Secondary1 python:3 bash
pip3 install sortedcontainers
```
3. initialize Client1:
```
docker run -it --rm --network=dist_systems_lab_network -v$(pwd):/home -w/home --name Client1 python:3 bash
```
4. in Master run ```Master.py```, in Secondary1 run ```Secondary1.py```







