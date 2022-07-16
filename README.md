
function odd(...sum){
console.log(sum);
    return ;
}
console.log(odd(1,3,5,7,9,11,13,15,17,19));



function odd(...sum){
console.log(sum);
    return ;
}
console.log(odd("HI GUVI"));



var avg = function (marks) {

let sum = 0;

for (let mark of marks) {
 sum = sum + mark;
}
 let avg = sum / marks.length;

return avg;
}
console.log(avg([53,34,45,23,33]));
