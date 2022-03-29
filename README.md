# Programming Exercise

Your task is to figure out how this code works.

* Come with a test input for the function.
* Trace the flow of the program with your test input **without running the code**, keeping track of all of the variables and transformations until you can determine the output.
* Keep coming up with new inputs until you're confident that you know how the function works.
* Write a summary of what the function does.

*SUMMARY*
1) The function takes an input of a person and a pet name. 
2) The function iterates on every item in the array of `person` and checks the `dog.name` against the entered `petName`.
3) If there is a match, the function returns `dog` object. 

```js
function (person, petName){
  for (let dog of person.dogs){
    if (dog.name === petName){
      return dog
    }
  }
}
```

Inputs and outputs should be valid JavaScript values!

| Input | Output |
| ----- | ------ |
| person.Kristofer{dog: "Winnie"}, "Winnie" | {name: "Winnie",...} | 
| person.Alycia{dog: "Remi"}, "Remi"      | {name: "Remi",...}   |  
| person.Joseph{dog: "Aubrey"}, "Aubrey"    | {name: "Aubrey",...} | 

<table>
  <tr>
    <th>What does this program do?</th>
    <td>The program matches the owner with their pet and retrieves the pet info.</td>
  </tr>
</table>

## Rubric

* Contains a plausible collection of test cases
* Outputs are accurately derived from inputs
* Summary is plausible
