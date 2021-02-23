# What Google Learned From Its Quest to Build the Perfect Team

**Julia Rozovsky Story : she had worked at a consulting firm , she wasn't know what he want to do in her life , after that she applied to business school , he works with a group , they was gathering between classes or after dinner to discuss homework assignment and they worked hard , she had a real benefit from work within her teamates**

**THE WORK ISSUE: REIMAGINING THE OFFICE**
1. How to Build a Perfect Team
2. The War on Meetings
3. The Case for Blind Hiring
4. Failure to Lunch
5. The 'Good Jobs' Gamble
6. Rethinking the Work-Life Equation
7. The Rise of White-Collar Automation
8. The Post-Cubicle Office
9. The New Dream Jobs

- One study, said `the time spent by managers and employees in collaborative activities has ballooned by 50 percent or more`

- The bulk of modern work is more and more team-based.

- **Groups** 
  - tend to innovate faster.
  - see mistakes more quickly.
  - find better solution to problems.
  - tend to acheive better result.
  - report higher job satisfaction.
  - *Google* became focused on building the perfect team.

![Illustration by James Graham](https://static01.nyt.com/images/2016/02/28/magazine/28mag-teams2/28mag-teams2-superJumbo.jpg?quality=90&auto=webp)
Illustration by James Graham

- Understanding and influencing group norms were the keys to improving Google’s teams.

- **Good Teams**
  - had high average social sensitivity

`We had lots of data, but there was nothing showing that a mix of specific personality types or skills or backgrounds made any difference. The ‘‘who’’ part of the equation didn’t seem to matter`

`As long as everyone got a chance to talk, the team did well. But if only one person or a small group spoke all the time, the collective intelligence declined.`


-----------------------------------------------------

# CSS & HTML

### `transform ` property 

- Has 2d settings or 3d settings.

- 
```
div {
  -webkit-transform: scale(1.5);
     -moz-transform: scale(1.5);
       -o-transform: scale(1.5);
          transform: scale(1.5);
}

```

- **2D Transforms**:
  - `x` and `y` axes
  - 2D Rotate:
    - `transform: rotate(10deg)`
  - 2D Scale :
    - `transform: scale(.75);`
  - 2D Translate:
    - `transform: translate(-10px, 25%);`
  - 2D Skew:
    - `transform: skew(5deg, -20deg);`
  - Transform Origin:
    - ` transform: skewX(20deg);`
      ` transform-origin: top left;`
  - Perspective:
    - `transform: perspective(200px) rotateX(45deg);`
  - Perspective Origin: 
    - `perspective-origin: 75% 75%;`

- **3D Transforms**:
  - `x` , `y` and `z` axes
  - 3D Rotate:
    - `transform: perspective(200px) rotateZ(45deg);`
  - 3D Scale: 
    - `transform: perspective(200px) scaleZ(.25) rotateX(45deg);`
  - 3D Translate:
    - `transform: perspective(200px) translateZ(50px);`
  - *Skew* can't be transformed on a three-dimensional scale.
  - Backface Visibility:
    - `backface-visibility: hidden;`
       `transform: rotateY(180deg);`


### Transition & Animation :

- **Transition** :

```
.box {
  background: #2db34a;
  transition-property: background;
  transition-duration: 1s;
  transition-timing-function: linear;
}
.box:hover {
  background: #ff7b29;
}

```

  - Transitional Property: `transition-property: background, border-radius;`
  - Transition Duration : `transition-duration: .2s, 1s;`
  - Transition Timing: `transition-timing-function: linear, ease-in;`
  - Transition Delay : `transition-delay: 0s, 1s;`


- **Animation**:
  *The @keyframes rule must be vendor prefixed, just like all of the other transition and animation properties.*

  *@-moz-keyframes@-o-keyframes@-webkit-keyframes*


    
