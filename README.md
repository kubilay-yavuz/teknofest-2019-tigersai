# Teknofest AI Competition 2019

This the project that got us to fifth place out of nearly 250 competitors. The project is a joint work of [Melik Burak Bozbey](https://github.com/mburakbozbey) and I under the name [TigersAI](https://github.com/tigers-ai) We made this project with Google Colab and Drive only.

The project mostly depended on Keras-retinanet, and the datasets we used. 
We used 4 different backbones;
* ResNet50 which we end up using as final model.
* ResNet101 gave us a fairly good results but ResNet50 proved to be better.
* ResNet152 gave us results that are close to ResNet152. However, the model is large, and we lacked computing power.
* VGG-19 performed poorly comparing to the others.

The algorithm had a hard time predicting pedestrians because of the anchor sizes. We tried to get smaller anchor sizes but still, the model couldn't fit a perfect anchor size that fit the pedestrians. 

However, for vehicles, our model excelled. We had a perfect precision on every test data we used. Even though we didn't train the model with the night images in the initial stage, the model performed well in the night case like in the day.

You can see in the csv files, the used datasets. Here's some screenshots from the model.

1. An overall performance of the model
![Image from the given dataset](/images/1.jpeg)

2. The pedestrians missed because of the anchors
![The pedestrians missed because of the anchors](/images/anchor-pedes.jpeg)

3. The pedestrians missed because of the anchors
![An image](/images/anchor-pedes-1.jpeg)

4. Our model had a hard time when the subject image is taken in construction site
![Construction Site](/images/construction-site.jpeg)

5. Our model predict a moving car in a night scheme<br>
![Night image](/images/night-moving.jpeg)

6. From the training phase: You see the precision is low on pedestrians (yaya means pedestrian in Turkish)
![Training Phase](/images/trainin-phase.jpeg)
