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






