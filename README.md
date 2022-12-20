# Distributed-systems (Replicated log)
The laboratory works of distributed systems in Kyiv Polytechnic Institute

Selfcheck acceptance test
1. initialize Master:
```
docker run -it --rm --network=dist_systems_lab_network -v$(pwd):/home -w/home --name Master python:3 bash
```
2. initialize Secondary1:
```
docker run -it --rm --network=dist_systems_lab_network -v$(pwd):/home -w/home --name Secondary1 python:3 bash
```
3. initialize Secondary2:
```
docker run -it --rm --network=dist_systems_lab_network -v$(pwd):/home -w/home --name Secondary2 python:3 bash
```
4. In Master, Secondary1, Secondary2 instlall:
```
pip3 install sortedcontainers
```



