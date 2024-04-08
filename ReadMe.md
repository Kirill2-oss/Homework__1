# HomeWork
"use strict";

function solveEquation(a, b, c) {
    let discriminant = b ** 2 - 4 * a * c;
    if (discriminant < 0) {
        return [];
    } else if (discriminant === 0) {
        let root = -b / (2 * a);
        return [root];
    } else {
        let root1 = (-b + Math.sqrt(discriminant)) / (2 * a);
        let root2 = (-b - Math.sqrt(discriminant)) / (2 * a);
        return [root1, root2];
    }
}

// Пример использования функции
let a = 1;
let b = -3;
let c = 2;
let roots = solveEquation(a, b, c);
console.log("Roots:", roots);