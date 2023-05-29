
# Классификатор изображений ResNet
![GitHub repo size](https://img.shields.io/github/repo-size/Odilbek99/intel-image-classification-resnet)
![GitHub contributors](https://img.shields.io/github/contributors/Odilbek99/intel-image-classification-resnet)
![GitHub stars](https://img.shields.io/github/stars/Odilbek99/intel-image-classification-resnet)
![GitHub forks](https://img.shields.io/github/forks/Odilbek99/intel-image-classification-resnet)

## Описание
Этот проект содержит реализацию классификатора изображений, использующего архитектуру ResNet, для работы с набором данных Intel Image Classification из Kaggle.

## Архитектура
Модель использует архитектуру ResNet (Residual Network), которая известна своими "skip connections" или пропускными соединениями, позволяющими эффективно обучать глубокие нейронные сети.

## Набор данных
Используется набор данных Intel Image Classification от Kaggle, включающий изображения, классифицированные в шесть разных классов. Изображения нормализуются и изменяют свой размер перед подачей на вход модели.

## Тренировка модели
Обучение модели происходит с использованием оптимизатора Adam, политики обучения с одним циклом и отсечения градиента.

## Результаты
Модель достигает точности 85% на тестовых данных. Отчет о классификации и матрица ошибок предоставляют детальную информацию о производительности модели.

## Улучшения
Возможны дальнейшие улучшения модели с использованием более сложной версии ResNet, настройкой гиперпараметров или применением техник аугментации данных.


## Загрузка и использование обученной модели
```bash
# Загрузка модели
model = ResNet(ResidualBlock, [2, 2, 2])
model.load_state_dict(torch.load('model_resnet.pth'))


Пожалуйста, адаптируйте пути, имена файлов и другие особенности в соответствии 
с фактической структурой и потребностями вашего проекта.


