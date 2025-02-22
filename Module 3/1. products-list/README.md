# Корзина товаров

## Задача

Написать React компонет для добавления товаров из списка в корзину

Компонент (`src/components/ProductsList.js`) принимает 1 значение в `props`:

- `products` - массив объектов формата `{ name: "PRODUCT NAME", available: true }`

Компонент (`src/components/ProductsList.js`) должен показывать на экране:

- количество товаров в корзине (изначально - 9)
- список товаров
- у каждой строки товара должно быть выведени на экран название и кнопка добавления в корзину

### Условия:

- Изначально в корзине 0 товаров
- При нажатии на любую из кнопок добавления, данный товар добавляется в корзину и, как результат, счетчик товаров в корзине увеличивается на 1
- У товаров со свойством `available: false` кнопка должна быть неактивна (и как результат ничего не должно происходить по нажатию)

### Проверка:

Чтобы мы могла автоматически проверить ваше решение, добавте в ваш компонент следующие атрибуты:

- `data-testid="basket-items-count"` элементу, который содержит количество элементов в корзине
- `data-testid="product"` у каждого из элементов, рисующих один товар из списка. Пример:

```jsx
...
  <div data-testid="product">
    {/* Информация по товару */}
  </div>
...
```

### Смотреть результаты

После решения задачи, сделайте `push` вашего решения. Это запустит Github Action с тестами вашего задания.
Во вкладке Actions в GitHub слева вы увидите все запуски тестов для всех задач. Найдите там "Модуль 3, Задача 1: Список товаров" и выберите его. Вы увидете список всех запусков тестов на вашем решении.
Если иконка возле последнего запуска зеленая - все хорошо, задание решено верно. Если нет - вы можете зхайти внутрь и посмотреть, что не сработало.

Также можно запускать эти тесты на вашем компьютере через `npm test`.
