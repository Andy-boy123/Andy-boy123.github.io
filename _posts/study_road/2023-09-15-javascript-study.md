---
layout:       post
title:        "Javascript初学"
author:       "Andy"
header-style: text
catalog:      true
tags:
    - javascript
    - web
---
# Javascript 初学
```
const s = 'Hello World!';
console.log(s.length);//空格也算一个字符
console.log(s.toLowerCase());
console.log(s.substring(0,5).toUpperCase());
console.log(s.split(' '));//以空格为分隔符，分割字符串
console.log(s.split('， '));//以逗号和空格为分隔符，分割字符串
let age = 20;
console.log(age);

const name = 'John';
console.log(`I am ${name} and I am ${age} years old.`);
const Hello = `I am ${name} and I am ${age} years old.`;
console.log(Hello);

const fruits = ['apples', 'oranges', 'pears', 10, true];
fruits[5] = 'grapes';//添加元素
fruits.push('mangos');//在数组的末尾添加元素
fruits.unshift('strawberries');//在数组的开头添加元素
fruits.pop();//删除最后一个元素
console.log(Array.isArray(fruits));//判断是否为数组
console.log(fruits.indexOf('oranges'));//查找元素的索引
console.log(fruits);

const person = {
    firstName: 'John',
    lastName: 'Doe',
    age: 30,
    hobbies: ['music', 'movies', 'sports'],
    address: {
        street: '50 main st',
        city: 'Boston',
        state: 'MA'
    }, 
};//对象

console.log(person.firstName, person.lastName);//访问对象的属性

const { firstName, lastName, address: { city } } = person;//解构
console.log(firstName, city);
person.email = '123@123';//添加属性

const todos = [
    {
        id: 1,
        text: 'Take out trash',
        isCompleted: true
    },
    {
        id: 2,
        text: 'Meeting with boss',
        isCompleted: true
    },
    {
        id: 3,
        text: 'Dentist appt',
        isCompleted: false
    },
];//数组中包含对象
console.log(todos[1].text);//访问数组中的对象的属性

const todoJSON = JSON.stringify(todos);//对象转换为JSON
console.log(todoJSON);

const x = 10;
const y = 11;
if (x === 10) { // === 严格相等  == 相等
    console.log('x is 10');
}
 //三目运算符
const color = x > 10 ? 'red' : 'blue';//如果x大于10，color为red，否则为blue

switch (color) {
    case 'red':
        console.log('color is red');
        break;
    case 'blue':
        console.log('color is blue');
        break;//important
    default:
        console.log('color is not red or blue');
        break;//break语句
}//switch语句

for (let i = 0; i < 10; i++) {
    console.log(`For Loop Number: ${i}`);
}//for循环
//while循环
let i = 0;
while (i < 10) {
    console.log(`While Loop Number: ${i}`);
    i++;
}
//do while循环
let j = 0;
do {
    console.log(`Do While Loop Number: ${j}`);
    j++;
}
while (j < 10);
const todos1 = [
    {
        id: 1,
        text: 'Take out trash',
        isCompleted: true
    },
    {
        id: 2,
        text: 'Meeting with boss',
        isCompleted: true
    },
    {
        id: 3,
        text: 'Dentist appt',
        isCompleted: false
    },
];
for (let i = 0; i < todos1.length; i++) {
    console.log(todos1[i].text);
}//for循环
for (let todo of todos1) {
    console.log(todo.text);
}//for of循环

```