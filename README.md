# JavaScript-for-Tip-Calculator
//A JavaScript code for calculating the tip depending on the total bill.

function tipCalc(totAmt) {
    if (totAmt<50)
        return 0.2 * totAmt;
    else if (totAmt>50 && totAmt<200)
        return 0.15*totAmt;
    else 
        return 0.1 * totAmt;
}

var total = [124 , 48, 268];

var tip1 = tipCalc(total[0]);
var tip2 = tipCalc(total[1]);
var tip3 = tipCalc(total[2]);

var tips = [tip1, tip2, tip3];
var final = new Array ((tip1+total[0]), (tip2+total[1]), (tip3+total[2]) );

console.log(tips);
console.log(final);
