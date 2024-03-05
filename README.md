# TestovoeZadanie
Общие вопросы: 
  1. QA инженер тестирует приложения и сервисы до того как они попадут в руки заказчика или пользователей, его задачами является выявлять баги, дефекты в приложениях и прочих продуктах программного обеспечения в соответствии с требованиями и спецификацией.
  2. Тестирование - это проверка ПО на соответствие требованиям и выявление ошибок или дефектов. Включает в себя запуск программы, проверку её функциональсти, производительности, безопасности и прочего.
  3. Проверка ПО помогает установить надёжность, стабильность, качество программы, повышает уровень удовлетворённости пользователя или заказчика.

Логическая задача:

  Первому пирату никак не получить максимально возможное количество монет и остаться в живых, так как в условиях сказано, что каждый пират поддержит предложенный вариант если он для него выгоднее чем альтернатива, а альтернативой для пирата видится сокращение количества желающих получить деньги, соответственно каждый следующий будет против.

Задачи на тестирование:
  1. Как протестировать сломанный тостер?
     
  Необходимо узнать какие требования у тостера были в рабочем состоянии. Как, в чём и где проявляется неисправность, при каких обстоятельствах и в следствии чего появилась неисправность. Исходя из этого продолжать искать дефект. Внешний осмотр на повреждения, подключение в розетку, проверяем рычажок, температурное колесо, фиксацию внутренних элементов, нагрев тенов, проверяем плату, контакты и т.д.
  
  2. В приложении к тестовому заданию вы найдете 2 скриншота - реальное приложение (приложение №1) и макет (приложение №2). Найдите ошибки при реализации. Опционально - дайте рекомендации по улучшению.
  
  Исходя из макета при реализации визуально картинка сместилась вправо, также в макете приложение должно было оповестить пользователя о готовности карты, при реализации выходит "доставка карты" по адресу, без предупреждения о диапозоне времени доставки и кнопка "закрыть", ставя пользователя перед фактом без возможности выбора.
  
  Рекомендация по улучшению визуала: провести модульное тестирование, исправить код. Опционально пользователя необходимо оповестить о готовности карты, после иметь возможность выбора "забрать по адресу" или "доставить по адресу", а также иметь возможность выбора времени, ну и обязательное предупреждение о наличии паспорта при получении карты во всех перечисленных случаях.
  
  3. Вам передали на тестирование калькулятор и список проверок к нему, которые написал предыдущий QA. Требования описаны чуть ниже. Ваша задача - проверить корректность этих проверок.
  1) В первом тесте пишут 2 действия (1+1+1), когда как в требовании указано о возможности калькулятора посчитать 1 действие, в ожидаемом результате хотят видеть 1+1=2, фактический результат дает 1+1=2, но калькулятор должен дать ответ "некорректный ввод, введите одно действие", чтобы не вводить пользователя в заблуждение и не допустить ошибку при расчётах.
  2) Ошибки нет, в требованиях не указано возможность подсчётов с 0.
  3) Ошибка есть, "данная операция не найдена", в требованиях указано что калькулятор помимо целых чисел должен уметь считать десятичные дроби с точностью до 5 знаков после запятой.
  4) .
  5) По ожидаемому и фактическому результату видим что не реализовано округление десятичных дробей, калькулятор просто считывает первые пять знаков после запятой.
  6) "Минус один + 1", калькулятор считает первый знак (минус один) за одно действие, не видит +1, не реализованы отрицательные числа.
  7) "Триста четырнадцать минус 14", в ожидаемом результате должен быть "некорректный ввод", так как в требованиях указана возможность печатать числа состоящие из одного слова или вводить цифрами, калькулятор фактически считает "триста минус 14", пропустив "четырнадцать". 314 это трехзначное число, которое в печатном виде состоит из двух слов.
  8) Ошибки нет. В ожидаемом результате и фактичсеком получен корректный ответ, после запятой 5 знаков учтены верно.
    
