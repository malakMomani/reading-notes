# Domain Modeling

> is the process of creating a conceptual model in code for a specific problem.

- model : describe the various entities , their attribute and behaviors
- entry : stores data in properties and encapsulates behaviors in methods is commonly referred to as an **Object-Oriented** model.

> A domain model that's articulated well can verify and validate the understanding of a specific problem among various stakeholders. As a communication tool, it defines a vocabulary that can be used within and between both technical and business teams.

Example :

| **Property**   |      **Data**      |  **Type** |
|----------|:-------------:|------:|
| epicRating | 1 to 10 | Number |
| hasAnimals |    `true` or `false`   |   Boolean |

Here's an implementation of the EpicFailVideo constructor function :

```
var EpicFailVideo = function(epicRating, hasAnimals) {
  this.epicRating = epicRating;
  this.hasAnimals = hasAnimals;
}

var parkourFail = new EpicFailVideo(7, false);
var corgiFail = new EpicFailVideo(4, true);

console.log(parkourFail);
console.log(corgiFail);
```
**two objects are instantiated with the new keyword and their properties are initialized by calling the EpicFailVideo constructor function**

***This is object-oriented programming in JavaScript at its most fundamental level***
1. The `new` keyword instantiates (i.e. creates) an object.
2. The constructor function initializes properties inside that object using the `this` variable.
3. The object is stored in a variable for later use.

### Generate random numbers
```
EpicFailVideo.prototype.generateRandom = function(min, max) {
  return Math.floor(Math.random() * (max - min + 1)) + min;
}
```

### Calculate daily Likes
- To calculate the number of viewers per day, generate a random number between 10 and 30 and then multiply it by the epic rating of that video :

| Random number   |      Epic rating      |  Viewers per day |
|----------|:-------------:|------:|
| 10 |  10 | 100 |
| 20 |    9   | 180 |
| 30 | 8 | 240 |

- The percentage of viewers who'll Like a video depends on whether or not the video contains animals: 

| Animals   |      Percentage      |
|----------|:-------------:|
| Yes |  75% |
| No |   40%   |

```
EpicFailVideo.prototype.dailyLikes = function() {
  var viewers, percentage;

  viewers = this.generateRandom(10, 30) * this.epicRating;

  if (this.hasAnimals) {
    percentage = 0.75;
  } else {
    percentage = 0.40;
  }

  return Math.round(viewers * percentage);
}
```

### Calculate weekly Likes
 ```
 
EpicFailVideo.prototype.weeklyLikes = function() {
  var total = 0;

  for (var i = 0; i < 7; i++) {
    total += this.dailyLikes();
  }

  return total;
}
 ```

 **Domain modeling is the process of creating a conceptual model for a specific problem. And a domain model that's articulated well can verify and validate your understanding of that problem.**


 -----------------------------------------------------------------------------------------

 # Chapter 6 : Tables

**What's A Table ?**
> A table represents information in a grid format.

- < table> : is used to create a table.
- < tr> : indicate the start of each row (stands for table row).
- < td> : stands for table data
- < th> : is used like <td> but its purpose is to represent the heading for either a column or a row (stands for table heading).
- Example :

```
< table>
    < tr>
        < th></ th>
        < th scope="col">Saturday</ th>
        < th scope="col">Sunday</ th>
    </ tr>
    < tr>
        < th scope="row">Tickets sold:</ th>
        < td>120</ td>
        < td>135</ td>
    </ tr>
    < tr>
        < th scope="row">Total sales:</th>
        < td>$600</td>
        < td>$675</td>
    </ tr>
</ table>
```
