```{.python .input}
from mxnet import image
import matplotlib.pyplot as plt
import glob, os

for file in glob.glob("img/style/*.jpg"):
    style_img = image.imread(file)
    plt.imshow(style_img.asnumpy())
    plt.show()
```

```{.python .input}
for file in glob.glob("img/content/*.jpg"):
    content_img = image.imread(file)
    plt.imshow(content_img.asnumpy())
    plt.show()
```
