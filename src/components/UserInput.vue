<template>
    <div id="user-input">

        {{ calculateInvestment }}

        <div class="input-group">
            <p>
                <label>initial Investment</label>
                <input type="number" id="initialInvestment" name="initialInvestment" v-model="initialInvestment">
            </p>
            <p>
                <label>Annual Investment</label>
                <input type="number" id="annualInvestment" name="annualInvestment" v-model="annualInvestment">
            </p>
        </div>
        <div class="input-group">
            <p>
                <label>Expected Return </label>
                <input type="number" id="expecteReturn" name="expectedReturn" v-model="interest">
            </p>
            <p>
                <label>Duration</label>
                <input type="number" id="duration" name="duration" v-model="duration">
            </p>
        </div>
    </div>

    <table id="result">
        <thead>
            <tr>
                <th>Year</th>
                <th>Investement Value</th>
                <th>Interest (Year)</th>
                <th>Total Interest</th>
                <th>Invested Capital</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>1</td>
                <td>2</td>
                <td>3</td>
                <td>4</td>
                <td>5</td>
            </tr>
        </tbody>
    </table>
</template>

<script>
// import { calculateInvestmentResults } from '../util/investment.js' 
export default {
    name: 'UserInput',
    data() {
        return {
            initialInvestment: 10000,
            annualInvestment: 1200,
            interest: 6,
            duration: 10,
            calculateInvestment: []
        }
    },

    methods: {
        calculate(){
            // this.calculateInvestment = calculateInvestmentResults(this.initialInvestment, this.annualInvestment, this.interest, this.duration)
            let arr = [1,6,9]
            this.calculateInvestment = [...arr]
            console.log("Testing...", this.arr)
        }
    }
    
}
</script>

<style>
#user-input {
    padding: 1rem;
    max-width: 30rem;
    margin: 2rem auto;
    border-radius: 4px;
    background: linear-gradient(180deg, #307e6c, #2b996d);
}

.input-group {
    display: flex;
    justify-content: space-evenly;
    gap: 1.5rem;
}

#user-input label {
    display: block;
    margin-bottom: 0.25rem;
    font-family: 'Roboto Condensed', sans-serif;
    font-size: 0.5rem;
    font-weight: bold;
    text-transform: uppercase;
}

#user-input input {
    width: 100%;
    padding: 0.5rem;
    border: 1px solid #76c0ae;
    border-radius: 0.25rem;
    background-color: transparent;
    color: #c2e9e0;
    font-size: 1rem;
}

#result {
  max-width: 50rem;
  margin: 2rem auto;
  padding: 1rem;
  table-layout: fixed;
  border-spacing: 1rem;
  text-align: right;
}

#result thead {
  font-size: 0.7rem;
  color: #83e6c0;
}
</style>