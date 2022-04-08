# Tool for remove background | U2NET, TRACER


<h2>Quick Start</h2>

Tested on PyTorch 1.11.0 <br>
Check out this folder. We have built a pip package that can remove background an input image with one line of code.

Install with

```python 
pip install bgRemoverApp
```

Code demo

```python 

from PIL import Image
import bgRemoverApp

# './ckpt/TRACER-Efficient-7.pth'
model_path = './ckpt/u2net.pth'
input_image = Image.open('./input.jpg')

# U2NET, TRACER
output_image = bgRemoverApp.remove_bg(input_image, "U2NET", model_path)
output_image.save('output.png')

```
