ShareLaTeX
==========

ShareLaTex on Ubuntu 14

[![](https://badge.imagelayers.io/pengbai/docker-sharelatex:latest.svg)](https://imagelayers.io/?images=pengbai/docker-sharelatex:0.2.0 'Get your own badge on imagelayers.io')

Image on docker hub: [https://hub.docker.com/r/pengbai/docker-sharelatex/](https://hub.docker.com/r/pengbai/docker-sharelatex/)


[ShareLaTeX](https://www.sharelatex.com) is an open-source online real-time collaborative LaTeX editor. We can run directely a hosted version, and you can also run your own local version with docker [ShareLaTex image](https://hub.docker.com/r/pengbai/docker-sharelatex/).

Description
------------

Pull image:
```
docker pull pengbai/docker-sharelatex:0.2.0
```

ShareLaTex container run on port 3000, then visit on your browser http://localhost:49161 :
```
docker run -d -p 49161:3000 pengbai/docker-sharelatex:0.2.0
```

Keep your files on your own, you can volume the /data in container, then you can find your sources in /local-sharelatex-data:
```
docker run -d -p 49161:3000 -v /local-sharelatex-data:/data pengbai/docker-sharelatex:0.2.0
```




License
----

The code in this repository is released under the GNU AFFERO GENERAL PUBLIC LICENSE, version 3. A copy can be found in the `LICENSE` file.

Copyright (c) ShareLaTeX, 2014.
