# ollama-intel
ollama0.5.4 with intel iGPU surport
The Ollama version is 0.5.4 
the intel-oneapi-base-toolkit is 2025.0.1.46.
webui:https://github.com/n4ze3m/page-assist
# install
```
$ git clone https://github.com/mocikate/ollama-intel
$ cd ollama-intel
$ docker-compose -f docker-compose-intel.yml up 
```
or
```
docker run --name=ollama20250207-intel-gpu --hostname=e3119405733d --mac-address=02:42:ac:11:00:02 --env=DISPLAY= --env=SYCL_CACHE_PERSISTENT=1 --env=ZES_ENABLE_SYSMAN=1 --env=OLLAMA_HOST=0.0.0.0:11434 --env=PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin --volume=/usr/lib/wsl:/usr/lib/wsl:rw --volume=/tmp/.X11-unix:/tmp/.X11-unix:rw --volume=ollama-intel_ollama-intel-gpu:/root/.ollama --network=bridge --workdir=/llm/ollama -p 11434:11434 --restart=always --device /dev/dri:/dev/dri --device /dev/dxg:/dev/dxg --runtime=runc -d mocikate/ollama-intel-gpu:Ollama0.5.4
```
webui:All versions of webui compatible with  Ollama, but please consider recommending "pagesAssist". 
```
https://github.com/n4ze3m/page-assist
```
https://chromewebstore.google.com/detail/page-assist-a-web-ui-for/jfgfiigpkhlkbnfnbobbkinehhfdhndo
```

![image](https://github.com/user-attachments/assets/394ef9c1-a621-48a7-9ad4-1ca3cafe5631)
