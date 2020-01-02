# data-tricks-for-machine-learning

## Shorthand,useful code for data cleaning, pre-processing and handy ML tricks.


### 1. Removing digits from a sentence in one-line.

```python
remove_digits = str.maketrans('', '', string.digits)
sentence = sentence.translate(remove_digits)
```

### 2. Plotting training loss vs validation loss in kears

```
import keras
from matplotlib import pyplot as plt
history = model.fit(train_x, train_y,validation_split = 0.1, epochs=50, batch_size=4)
plt.plot(history.history['acc'])
plt.plot(history.history['val_acc'])
plt.title('model accuracy')
plt.ylabel('accuracy')
plt.xlabel('epoch')
plt.legend(['train', 'val'], loc='upper left')
plt.show()
```
