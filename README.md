# diffusion-LLM
repo to run on CPU ModernBERT-large-chat-v0  with [dllm](https://github.com/ZHZisZZ/dllm)

<img src='https://github.com/fabiomatricardi/diffusion-LLM/raw/main/dllm-bert-diffusion.gif' width=1000>
---

## How to use it with CPU only.
- Download from this repo the ZIP archive created with 7zip called [dllmFIX.7z](https://github.com/fabiomatricardi/diffusion-LLM/raw/main/dllmFIX.7z)
- save the file into a directory called `dllm`
- open the terminal in the directory `dllm`
- unpack the archive `tar -xf .\dllmFIX.7z`
- create virtual environment 'python -m venv venv'
- activate the venv `.\venv\Scripts\activate`
- Install the dependencies `pip install torch==2.6.0 torchvision==0.21.0 torchaudio==2.6.0`
- build the dllm project - `pip install -e .`

## Run the inference
To run the inference with [ModernBERT-large-chat-v0](https://huggingface.co/dllm-collection/ModernBERT-base-chat-v0) Diffuison using the [dllm libraries](https://github.com/ZHZisZZ/dllm), from the terminal with the venv activated run
```bash
python -u examples/bert/chat.py --model_name_or_path "dllm-collection/ModernBERT-large-chat-v0" --chat True
```
This will start a Chat session
#### it will take a long time for generation, but low memory footrpint

> 💻 I am running the model on an old Lenovo X260, with no dedicated GPU, 16 Gb of RAM


---




