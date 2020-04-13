#SMOMI

При выполнении данной работы я использоавл предобученную нейронную сеть VGG16 с обученным классификатором. 

a) В первом пункте для аугментации данных использовал горизонтальное отражение данных с помощью tf.image.random_flip_left_right(image). Файл train_randomFlipping.py, lr = 1*10^(-11)
Графики:

![Image alt](https://github.com/Repsolka/SMOMI/blob/Lab4/randomFlipping/flip_1e-11.jpg)

c) В данном пункте проводилась аугментация данных с помощью случайного изменения яркости и контраста 

    image = tf.image.random_brightness(image, 0.5, seed=None)
    image = tf.image.random_contrast(image, lower=0.2, upper=1.2 seed=None)
Файл train_randomBrightness.py, lr = 1*10^(-11).
Графики:

![Image alt](https://github.com/Repsolka/SMOMI/blob/Lab4/Graphs/randomBrightness/bright_1e-11.jpg)
