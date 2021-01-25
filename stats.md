<h4> Question  ##1: <br/>
A market has 3 doors. Entries from the doors to the market per hour respectively &lambda; 1 = 110, &lambda; 2 = 90 and &lambda; 3=160 creates a poisson process with customer. <br/>

30% of all customers are male. <br/>

The probability of any man buying from the market is 80%, for any woman 10%. An average ali-veris is 67.5 TL. <br/> </h4>

a) What is the expected amount of shopping in a 10-hour working day?


</div>
<details>
  <summary><b>Click here for the solution</b></summary>
<br>
<div id="q1" class="collapse">

Customers entering through all doors create independent poisson processes. <br/> 
&lambda; 1 + &lambda; 2 + &lambda; 3 = &lambda; <br/>
&lambda; = 110 + 90 + 160 = 360 customers / hour creates a fast composite poisson process. <br/>

---
Since 30% of all customers are men, separating this total process, 
the speed of the process created by male customers <br/> 
&lambda; Male = 360 * 0.30 = 108 customers / hour, <br/> 
the process created by female customers is <br/>
&lambda; Female = 360 * 0.70 = 252 customers / hour. <br/>

These two poisson processes are independent of each other. <br/>

---
If we distinguish the male fast poisson process again with similar thinking as "shopping" and "non-shopping" male customers: <br/>

- Speed ​​of male customers shopping: <br/>
&lambda; Male, S = 108 * 0.80 = 86.4 customers / hour <br/>

- Speed ​​of male customers who do not shopping: <br/>
&lambda; 1 Male, S'= 108 * 0.20 = 21.6 customer / hour. <br/>

- Speed ​​of female customers shopping: <br/>
&lambda; Female, S = 252 * 0.10 = 25.2 customers / hour <br/>

- Speed ​​of female customers who do not shopping: <br/>
&lambda; 1 Female, S'= 252 * 0.90 = 226.8 customer / hour. <br/>

---

So on a 10-hour workday <br/>

E [Z <sub> t </sub>] = E [N <sub> t </sub> <sup> Male, S </sup> + N <sub> t </sub> <sup> Female, S </sup>] = E [N <sub> t </sub> <sup> Male, S </sup>] + E [N <sub> t </sub> <sup> Female, S </sup> ] = & lambda; <sub>t</sub> <sup> Male, S </sup> + & lambda; <sub>t</sub> <sup> Female, S </sup> = 86.4 * 10 + 25.2 * 10 = 1116 customer / hour and <br/>

Expected amount of shopping in a 10-hour working day as the average basket is 67.5 TL: <br/>

1116 * 67.5 TL = **75 330 TL.**

</div>
</details>



b) What is the likelihood that the third woman who does shopping comes to the market within the first 15 minutes?

</div>
<details>
  <summary><b>Click here for the solution</b></summary>
<br>
<div id="q1" class="collapse">
  
<img src="https://latex.codecogs.com/gif.latex?p(T_3&space;\leq&space;15_(mins))&space;=&space;p(T_3&space;\leq&space;1/4_(hours))&space;=&space;1-&space;\sum_{k=0}^{2}\frac{e^{-\lambda(Female,&space;S)^t}\lambda_((Female,S)^t)^{Female}}{Female_k!}" title="p(T_3 \leq 15_(mins)) = p(T_3 \leq 1/4_(hours)) = 1- \sum_{k=0}^{2}\frac{e^{-\lambda(Female, S)^t}\lambda_((Female,S)^t)^{Female}}{Female_k!}" />




</div>
</details>

