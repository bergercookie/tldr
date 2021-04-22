# Docker Debugging Cheatsheet

> Common issues and solutions for docker.

- When you use docker pull, without a :tag, it will default to the tag: latest.:

`docker pull buildbot/buildbot-master:master # <-- Specify :master`
