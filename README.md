# Eden Challenge - Lung Segmentation

This repo contains the solution for the part 1 of the Challenge described in `README_research.md`.

## Setup

### Prerequisites
- Python 3.9 or higher
- pip

### Virtual Environment Setup

1. **Create a virtual environment:**
   ```bash
   python -m venv venv
   ```

2. **Activate the virtual environment:**
   ```bash
   # Windows
   venv\Scripts\activate
   
   # Linux/macOS
   source venv/bin/activate
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Verify installation:**
   ```bash
   python -c "import torch; print(f'PyTorch version: {torch.__version__}')"
   ```

### Deactivating the environment
When you're done working on the project:
```bash
deactivate
```

## Project Structure

This project implements lung segmentation on chest X-ray images using deep learning techniques with PyTorch and MONAI.