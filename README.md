# Nagios Agent
Nagios의 NRPE(Nagios Remote Plugin Executor)를 Container 형태로 배포하기 위해 만들었습니다.

##### - 사용법
```sh
[root@ruo91 ~]# docker build --rm -t nagios:agent https://github.com/ruo91/docker-nagios-agent.git
[root@ruo91 ~]# docker run -d --name="nagios-agent" -h "nagios-agent" \
-p 5666:5666 -p 5667:5667 nagios:agent
```