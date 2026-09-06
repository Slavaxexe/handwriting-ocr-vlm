# Handwriting OCR with Qwen2.5-VL

An experiment in extracting Russian handwritten text from photographs with the `Qwen2.5-VL-7B-Instruct` vision-language model.

The model runs with 4-bit quantization, while large input images are resized automatically to reduce memory usage. Recognition quality is evaluated on six samples using character error rate (CER).

## Result

The experiment achieved a mean CER of approximately **0.173**. Clear handwriting was recognized almost perfectly, while irregular handwriting remained the main source of errors.

## Stack

Python, PyTorch, Transformers, BitsAndBytes, Pillow, Qwen VL Utils, and CER.

Install `requirements.txt` and open `handwriting_ocr_vlm.ipynb` to reproduce the experiment.
