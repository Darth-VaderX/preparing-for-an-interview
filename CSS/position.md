# Position

---

**Position** - css свойство, задаёт способ позиционирования элемента в документе.

## Значения свойства position:

1. **static** - Значение по умолчанию. Любой элемент, добавленный на страницу, будет иметь это значение и будет расположен в нормальном потоке документа согласно контексту форматирования родительского элемента. Свойства `left`, `right`, `top`, `bottom `и `z-index` игнорируются. Элемент с данным значением не является **опорным** для других позиционированных элементов.
2. **relative** - элемент позиционируется относительно самого себя
3. **absolute** - позиционируется относительно ближайшего элемента со свойством `position` отличающегося от `static`. Элемент становится блочным, а его ширина определяется содержимым. Убирается из основного потока и перестаёт взаимодейстоввать со всеми элементами, кроме потомков
4. **fixed** - работает так же как и `absolute`, но позиционируется относительно окна браузера за исключением случаев, если один из родителей имеет значения свойств `transform`, `perspective` или `filter`, отличные от none. В этом случае блок становится опорным, и позиционирование будет производиться уже относительно него, а не окна браузера.
5. **static** - элемент ведёт себя как элемент `relative` до тех пор, пока его родитель не будет прокручен до определённой границы. Элемент остаётся «приклеенным» во время прокрутки родителя до тех пор, пока не «встретит» противоположную границу своего родителя.

**z-index** - управляет положением элемента в трёхмерном пространстве. `z-index` срабатывает для элементов с позиционированием , отличающимся от статичного. Исключение из правил: `z-index` работает с элементами, у которых значение свойства `opacity` меньше 1. Например, трюк с `opacity`: 0.999 почти не повлияет на внешний вид, но позволит использовать `z-index` без изменения позиционирования элемента. `z-index` также срабатывает у флекс- и грид-элементов и везде, где создаётся контекст наложения.

- [Что такое CSS?](./CSSis.md)
- [Что такое блочная модель?](./boxModel.md)
- [Что такое псевдоклассы?](./pseudoclass.md)
- [Что такое псевдоэлементы?](./pseudoelement.md)
- [Что такое специфичность?(Вес селекторов)](./specificity.md)
- [Какая разница между rem и em?](./emVSrem.md)
- [Какие есть комбинаторы в CSS?](./combinators.md)
- [Вопросы по CSS](./CSS.md)
- [Главное меню](../README.md)