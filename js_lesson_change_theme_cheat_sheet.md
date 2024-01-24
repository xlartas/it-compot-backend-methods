```javascript
// Создание переменных
const variable = 'Some string';
const something = 765;
const something_else = [123, 321, 'EE', [], [1, '']];
const omg_i_dont_know = {
    'name': 'Petr',
    'age': 12,
    'gender': 'Unknown',
    'address': 'Deep Forest'
};



// Получение первого найденного элемента по селектору в переменную
const a1 = document.querySelector('.classname');
const a2 = document.querySelector('.classname > img');
const a3 = document.querySelector('header');
const a4 = document.querySelector('.some_class.classname');
const a5 = document.querySelector('body');
const a6 = document.querySelector('header > nav > .nav-link');
// Получение всех найденных элементов по селектору в массиве в переменную
const a1 = document.querySelectorAll('.classname');
// Это массив, если элементов не найдено, то пустой массив.



// Функция addEventListener может быть 
// пременена почти к любому видимому html тэгу.
// Первым аргументом она принимает название отслиживаемого события,
// Вторым аргументом функцию.

// Можно использовать анонимную функцию:
a2.addEventListener('click', function () {
    console.log('text!!!');
});

// Можно просто создать функцию и передавать её.
function someFunc() {
    console.log('text!!!');
}
a2.addEventListener('click', someFunc);

// Можно использовать стрелочную функцию.
a2.addEventListener('click', () => {
    document.querySelector('body').style.backgroundColor = '#ff0';
});



// Атрибутами в html называются надписи вида: 
// class, id, src, style, alt, name, type, value, placeholder и т.д.
// Для получения атрибута:
const param1 = a2.getAttribute('class');
// Для установки атрибута или его изменения:
a2.setAttribute('class', 'd-flex mx-auto');



// В локальном хранилище браузера могут хранится ТОЛЬКО строки.
// Установка пары ключ-значнеие в локальное хранилище или её изменение. 
localStorage.setItem('some_key1', 'Some string!');
localStorage.setItem('some_key2', 126..toString()); // Число в строку
localStorage.setItem('some_key3', (1.33).toString()); // немного другой способ число в строку
// Получение значения по ключу
localStorage.getItem('some_key1');
const l2 = localStorage.getItem('some_key2');
console.log(localStorage.getItem('some_key3'));




// Использование условного оператора
if (2 > 1) {
    console.log('some text...')
}

if (l2 == '3') {
    console.log('some text...')
} else {
    console.log('some text...')
}

if (l2 != 100 and
l2 > 5
)
{
    console.log('some text...')
}
else
if (l2 == 0) {
    console.log('some text...')
} else {
    console.log('some text...')
}
```