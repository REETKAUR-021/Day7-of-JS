//Functions

function greet(){
    console.log("Good Morning");
}
greet();  //Good Morning

function sum(a , b){
    console.log(a + b);
}
sum( 3 , 2);  //5

//Arrow Functions
const arrowsum = (a , b) => {
    console.log(a + b);
};
arrowsum(5 , 9);  //14

const arrowmul = (a , b) => {
    console.log(a * b);
};
arrowmul(3 , 9); //27

const print = () => {
    console.log("Hello, World!");
}
print();  //Hello, World!

//Practice question
function vowels(str){
    let count = 0;
    for(let char of str){
        if(char === "a" || char === "e" || char === "i" || char === "o" || char === "u"){
            count++;
        }
    }
    console.log(count);
}
vowels("a b e i o u v"); //5

//forEach loop 
let arr = [1 , 2, 3, 4 , 5];
arr.forEach(function value(val){
   console.log(val);
});
arr.forEach((val , idx , arr) => {
    console.log(val , idx , arr);
});

//practice question
let numbers = [2 , 3, 4, 5, 6];
numbers.forEach(function number(num){
    console.log(num*num);
}) //4 , 9, 16 , 25, 36

//Map method
let num = [45 , 5, 78, 89];
let newArr = num.map((val) => {
    return val*3;
});
console.log(newArr);  //[135, 15, 234, 267]

//Filter method
let array = [1 ,2 ,4, 5, 6, 7, 8];
let evenArr = array.filter((value) => {
    return value % 2 === 0;
});
console.log(evenArr); //[2, 4, 6, 8]

//Reduce
let Arr = [3 , 4, 5,6 ,7 ,8 ,8 ,9 ];
const output = Arr.reduce((res , curr) => {
    return res + curr;
});
console.log(output); //50

//Practice Question
let marks = [ 33 , 56, 79, 89, 76, 92];
let mark =marks.filter((val) => {
    return val > 60;
})
console.log(mark); //[79, 89, 76, 92]



