# AnimeGAN Studio

Streamlit app for AI-powered anime-style image generation using Stable Diffusion, PyTorch, and AnimeGAN-inspired artistic transformations.

This application converts ordinary photos into cinematic anime artwork inspired by Studio Ghibli, Makoto Shinkai visuals, retro anime aesthetics, fantasy illustrations, and stylized digital paintings.

Dataset and model source: [nitrosocke/Ghibli-Diffusion](https://huggingface.co/nitrosocke/Ghibli-Diffusion) from Hugging Face Diffusers.

## What It Includes

- AI-powered anime image generation using Stable Diffusion
- Multiple anime-inspired artistic styles
- Before vs After image comparison interface
- Download generated anime artwork
- Modern Streamlit dashboard with Dark / Light mode UI
- Fast image preprocessing and CPU compatibility
- Modular project structure for training, testing, and video conversion

## Available Anime Styles

- Ghibli Dream — Soft watercolor anime inspired by Studio Ghibli
- Dreamscape — Surreal vibrant dream-like anime visuals
- Cinematic Sky — Makoto Shinkai-inspired cinematic lighting effects
- Classic Anime — Retro 90s anime cel-shaded appearance
- Night Fantasy — Dark fantasy glowing anime aesthetic
- Oil Paint — Artistic anime oil-painting style transformation

## Important Model Note

This project uses diffusion-based anime generation models and artistic style transfer techniques. Output quality depends on image resolution, lighting conditions, preprocessing quality, and available hardware resources.

- CPU mode is supported for compatibility but may generate images slower
- GPU acceleration significantly improves generation speed and rendering quality
- Different anime styles apply different prompts and visual enhancements internally

## Setup

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install -r requirements.txt
```

## Install Required Models

Option 1: Download models automatically through Hugging Face Diffusers.

Option 2: Manually place model checkpoints inside the `models/` directory.

Example model used:

```text
nitrosocke/Ghibli-Diffusion
```

## Run

```powershell
streamlit run app.py
```

Open the local URL Streamlit prints, usually `http://localhost:8501`.

## Project Structure

```text
AnimeGAN-Studio/
│
├── app.py
├── requirements.txt
├── README.md
├── .gitignore
│
├── dataset/
│   ├── Hayao/
│   ├── Paprika/
│   ├── Shinkai/
│   ├── train_photo/
│   ├── test/
│   └── val/
│
├── models/
│   ├── checkpoint/
│   ├── pb_and_onnx_model/
│   └── net/
│
├── outputs/
│   └── results/
│
├── scripts/
│   ├── train.py
│   ├── test.py
│   ├── AnimeGANv2.py
│   └── video2anime.py
│
├── assets/
│   └── screenshots/
│
└── tools/
```

## Tech Stack

- Python
- Streamlit
- PyTorch
- Diffusers
- Transformers
- Pillow
- OpenCV
- NumPy

## Deployment

You can deploy this project on:

- Streamlit Cloud
- Hugging Face Spaces
- Render
- Railway

## Future Improvements

- GPU acceleration optimization
- Real-time anime conversion
- Additional anime art styles
- Video-to-anime transformation
- Face enhancement models
- AI image upscaling
- Batch image generation

## Git Commands

### Push Updates

```powershell
git add .
git commit -m "Updated project"
git push
```

### Pull Latest Changes

```powershell
git pull
```

## Contributing

Contributions are welcome.

To contribute:

1. Fork the repository
2. Create a new branch
3. Make improvements
4. Submit a Pull Request

## License

This project is licensed under the MIT License.

## Author

Priyanshi

GitHub:
https://github.com/Priyanshi102003

## Acknowledgements

- Hugging Face
- Streamlit
- PyTorch
- AnimeGAN Community
- Stable Diffusion Contributors
