const salary = document.getElementById("salary");
const benefits = document.getElementById("benefits");
const form = document.getElementById("salary-form");
const results = document.getElementById("results");
const clear = document.getElementById("clear");

form.addEventListener("submit", function (e) {
  e.preventDefault();
  const salaryValue = +salary.value;
  const benefitsValue = +benefits.value;
  const grossPay = salaryValue + benefitsValue;
  const NHIF = 1100;
  const NSSF = 1060;
  const paye = grossPay * 0.3;
  console.log(salaryValue, benefitsValue, paye);
  const netPay = grossPay - (paye + NHIF + NSSF);
  results.innerHTML = `
  <p>Your gross pay is ${grossPay}</p>
  <p>Your paye is ${paye}</p>
  <p>Your net pay is ${netPay}</p>
  `;
});

clear.addEventListener("click", function () {
  salary.value = "";
  benefits.value = "";
  results.innerHTML = "";
});
