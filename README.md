mnist_brain
===========
Recognizing hand-written digits from MNIST dataset with Brain.js. Neural Networks example.
### Quiqk start


Натренированная модель уже добавлена в репозиторий и сохранета в файле ./data/mnistTrain.json. Она создана с помощью скрипта **train.js**. Вам нет необходимости повторять эти действия заново.

Откройте в браузере страницу **nnTest.html** (пример будет работать, если ваш браузер поддерживает HTML тег **canvas**)

### Prepare

Если вы хотите натренировать нейронную сеть со своими настройками. Вам нужно будет модифицировать данные для библиотеки minst digits. 
По-умолчанию в нее загружаеться только 10 000 записей обучающей выборки. Вы можете загрузить все **60 000**
```javascript
net.train(trainingSet,
    {
        errorThresh: 0.001,  // error threshold to reach
        iterations: 20000,   // maximum training iterations
        log: true,           // console.log() progress periodically
        logPeriod: 1,       // number of iterations between logging
        learningRate: 0.3    // learning rate
    }
```
Вы можете немного уменьшить скорость обучения (learningRate) и передать в trainingSet большее число примеров для обучения. Будьте готовы к тому что система будет обучаться часы а может и дни.  

### Translation note

Very soon I translate this document into English

