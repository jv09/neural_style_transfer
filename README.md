# Neural Style Transfer

I tried to follow the paper [A Neural Algorithm of Artistic Style](https://arxiv.org/pdf/1508.06576v2.pdf).

But some of the things are implemented differently.

A simple MSE loss function is used instead of more complicated one which is used in the paper. 
Content is used as the input instead of Noise.

These might be the reasons for some differences in the result. 
I didn't notice any differences when changing the alpha and beta values. The biggest change happens when changing the learning rate. A higher learning rate leads to more significant changens to the original content.


### Setup
You will need a virtualenv with `python>=3.8`.

```bash
pip install poetry
poetry install
```

### To run style transfer
```bash
poetry run python neural_style_transfer/nst.py
```

### Results from some example content and style images

**Example 1:**

![alisha_result](https://user-images.githubusercontent.com/70435148/193102420-aca5866e-b305-41ab-97eb-4d70da9ba1cc.png)


**Example 2:**
Taking Starry night and snow as style and content images respectively

![snow](https://user-images.githubusercontent.com/70435148/193103028-60d481a1-1f30-469a-91fd-b91b2cb28d1b.png)
