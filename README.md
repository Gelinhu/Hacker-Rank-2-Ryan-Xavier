# Hacker-Rank-2-Ryan-Xavier

Staircase Problem

function staircase(n) {
    // Write your code here
    
    for(let i = 1; i <= n; i++){
        console.log(" ".repeat(n - i) + "#".repeat(i));

    }

}

Birthday Cake Candles

function birthdayCakeCandles(candles) {
    // Write your code here
let max = candles[0];
let count = 1;

    for (let i = 1; i < candles.length; i++) {
        if (candles[i] > max) {
            max = candles[i];   
            count = 1;          
        } 
    else if (candles[i] === max) {
            count++;            
        }
}

Breaking the records

function breakingRecords(scores) {
    // Write your code here
    
    let countmax = scores[0];
    let countmin = scores[0];
    let recordmax = 0;
    let recordmin = 0;
    
    for(let i = 0; i < scores.length; i++){
      if(countmax < scores[i]){
        recordmax = recordmax + 1;
        countmax = scores[i];
      }  
      if (countmin > scores[i]){
        recordmin = recordmin + 1;
        countmin = scores[i];
      }
    }
    return [recordmax, recordmin];

}

Compare The Triples

function compareTriplets(a, b) {
    let alice = 0;
    let bob = 0;
    
    for(let i = 0; i < a.length; i++){
        if(a[i] > b[i]){
            alice = alice + 1; 
        }
        if(b[i] > a[i]){
            bob = bob + 1;
        }
    }
    return [alice, bob]

}

A Very Big Sum

function aVeryBigSum(ar) {
    // Write your code here
    let soma = 0;
    
    for(let i = 0; i < ar.length; i++){
        soma = soma + ar[i];
    }
    return soma

}






