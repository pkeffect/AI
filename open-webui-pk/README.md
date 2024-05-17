# README
* The docker-compose.yaml listed above assumes the following:
  *  [Ollama](https://ollama.com/) is installed locally, not in docker.
  * Volumes are stored locally, not in docker.
  * You have a Nvidia GPU. If not, remove the ```deploy``` section.
  * You have [Nvidia Toolkit](https://developer.nvidia.com/cuda-downloads) installed.
* This is the most efficient setup for my system.
  * Windows 11 | [Docker Desktop](https://www.docker.com/products/docker-desktop/) | [WSL2](https://learn.microsoft.com/en-us/windows/wsl/install) - [Ubuntu 22.04](https://ubuntu.com/)
  * AMD Ryzen 9 3900XT | 128GB DDR4 RAM | ASUS TUF RTX 3080 GAMING OC 10GB
  
* Running mutiple docker-compose files at once:

```docker compose -f docker-compose.yaml -f clients-compose-clients.yaml up -d --build```

## Ollama
* [Ollama](https://ollama.com/)
* [Ollama github](https://github.com/ollama/ollama)
* [Ollama Models](https://ollama.com/library?sort=newest)
## OpenWebUI 
* [OpenWebUI](https://openwebui.com/)
* [OpenWebUI github](https://github.com/open-webui/open-webui)
## Huggingface
* [Huggingface](https://huggingface.co/)
## Stable Diffusion(s)
* Working via installs from [Stability Matrix](https://github.com/LykosAI/StabilityMatrix)
* These are under Settings -> Images settings in [OpenWebUI](https://openwebui.com/)
* ```http://host.docker.internal:porthere``` this assumes everything is hosted on the same machine
### Working Engines
### Set as Automatic1111
* [Auto1111](https://github.com/AUTOMATIC1111/stable-diffusion-webui) 
* [Forge](https://github.com/lllyasviel/stable-diffusion-webui-forge)
* [SD.Next.Web UI](https://github.com/vladmandic/automatic)
* [Web UI-UX](https://github.com/anapnoe/stable-diffusion-webui-ux)
### Set as ComfyUI
* [ComfyUI](https://github.com/comfyanonymous/ComfyUI)
* [StableSwarmUI](https://github.com/Stability-AI/StableSwarmUI)
### Not working ... (yet?)
* [Fooocus](https://github.com/lllyasviel/Fooocus)
* [Fooocus-ControlNet](https://github.com/fenneishi/Fooocus-ControlNet-SDXL)
* [Fooocus-MRE](https://github.com/MoonRide303/Fooocus-MRE)
* [InvokeAI](https://github.com/invoke-ai)
* [RuinedFooocus](https://github.com/runew0lf/RuinedFooocus)
* [VoltaML](https://github.com/VoltaML/voltaML-fast-stable-diffusion)
