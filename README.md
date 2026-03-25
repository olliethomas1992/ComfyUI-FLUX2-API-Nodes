# ComfyUI-FLUX2-API-Nodes

ComfyUI V3 nodes for generating images with [FLUX.2](https://blackforestlabs.ai/) models via the BFL API. Accepts ComfyUI IMAGE tensors directly — no separate base64 conversion needed.

## Nodes

| Node | Display Name | Image Inputs |
|---|---|---|
| **Flux2Max** | FLUX.2 [Max] (BFL) | 8 |
| **Flux2Pro** | FLUX.2 [Pro] (BFL) | 8 |
| **Flux2ProPreview** | FLUX.2 [Pro] Preview (BFL) | 8 |
| **Flux2Klein9B** | FLUX.2 [Klein 9B] (BFL) | 4 |
| **Flux2Klein4B** | FLUX.2 [Klein 4B] (BFL) | 4 |
| **Flux2Klein9BKV** | FLUX.2 [Klein 9B KV] (BFL) | 4 |
| **Flux2Flex** | FLUX.2 [Flex] (BFL) | 8 |
| **FluxConfig** | Flux Config (BFL) | — |

## Installation

```bash
cd ComfyUI/custom_nodes
git clone https://github.com/olliethomas1992/ComfyUI-FLUX2-API-Nodes.git
pip install -r ComfyUI-FLUX2-API-Nodes/requirements.txt
```

## Configuration

1. Get an API key from [api.bfl.ai](https://api.bfl.ai/)
2. Either:
   - Add a **Flux Config** node to your workflow and enter your key, or
   - Create `config.ini` in the node pack directory:
     ```ini
     [API]
     key = your_bfl_api_key
     ```

## Requirements

- ComfyUI with V3 node support
- Python 3.10+
- `torch`, `aiohttp`

## Credits

Huge thanks to [Black Forest Labs](https://blackforestlabs.ai/) for building incredible image models and making them accessible via API.

Original node pack by [@gelasdev](https://github.com/gelasdev), [@pleberer](https://github.com/pleberer), and [@Duanyll](https://github.com/Duanyll).
