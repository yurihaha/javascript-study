# javascript-study
'use strict';


// 문자열
const string = 'This is a list of items: cherries, Limes, oranges, apples.';

// 추출한 목록
const array = ['cherries', 'limes', 'oranges', 'apples'];

const start = string.indexOf(':');
const end = string.indexOf('.', start + 1);

const listStr = string.substring(start + 1, end);

const fruits = listStr.split(',');

console.log(fruits); // [' cherries', ' limes', ' oranges', ' apples'];

fruits.forEach((elmnt, indx, arry) => {
  arry[indx] = elmnt.trim();
});

console.log(fruits); // ['cherries', 'limes', 'oranges', 'apples'];

const fruitsEx = listStr.split(/\s*, \s*/);


// chaining

const fruitsChaining = string.substring(start + 1, end).split(",");
