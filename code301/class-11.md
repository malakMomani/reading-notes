## EJS : Embedded Template Engine

What is *EJS* :  a templating engine used by Node.js. Template engine helps to create an HTML template with minimal code. Also, it can inject data into HTML template at the client side and produce the final HTML.

- Install *EJS* package : `npm i ejs`
- Set *EJS* as templating engine : `app.set('view engine', 'ejs');`
- Render a page on a certain request by the user : 

```
app.get('/', (req, res)=>{
// This page should be in the views folder
// in the root directory.
res.render('home');
  
});
```
- if there are any templates in HTML page like :

```
<body>
    <center>
        This is our home page.<br/>
        Welcome <%=name%>, to our home page.
    </center>
</body>
```

you should render the request like :

```
app.get('/', (req, res)=>{

// We can pass multiple properties and values
// as an object, here we are passing the only name
res.render('home', {name:'Malak'});
  
});
```

- if there is a list of items you want to render the HTML should look like :

```
<body>
    Hobbies of <%=data.name%> are:<br/>
    <ul>
        < %  data.hobbies.forEach((item)=>{ % >
        <li>< % =item %></li> 
        <% }); %>
    </ul>
</body>
```

and your request should look like :

```
app.get('/', (req, res)=>{
var data = {name:'Malak',
    hobbies:['Programming', 'playing chess', 'Reading']}
  
res.render('home', {data:data});
});
```