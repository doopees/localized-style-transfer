# Localized style transfer
Just a small project to test instance segmentation with [Mask R-CNN](https://arxiv.org/abs/1703.06870) (He et al.) and neural style transfer (NST) as described in [A Neural Algorithm of Artistic Style](https://arxiv.org/abs/1508.06576) (Gatys et al.). A similar work can be found in [Localized Style Transfer](http://cs231n.stanford.edu/reports/2017/pdfs/416.pdf) (Wells et al.), although I was not aware of it at the time I did this project.

Basically, first Mask R-CNN is used to detect people in an image, and then NST is applied to stylize the segmented instances. For a single instance, the algorithm is illustrated clearly in the following self-explanatory figure:

<p align="center">
<img src="/media/algorithm.png" width="1000"/>
</p>

In the figure above, the artwork employed for style transfer was Vincent van Gogh's [*The Starry Night*](https://upload.wikimedia.org/wikipedia/commons/thumb/e/ea/Van_Gogh_-_Starry_Night_-_Google_Art_Project.jpg/970px-Van_Gogh_-_Starry_Night_-_Google_Art_Project.jpg).

The resulting images should look something like this:

<p align="center">
<img src="/media/result.png" width="350"/>
</p>

Jupyter notebook [here](https://colab.research.google.com/github/doopees/localized-style-transfer/blob/main/code/localized_style_transfer.ipynb)
