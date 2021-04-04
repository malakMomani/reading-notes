## EJS Partial

- *EJS Partial* used when you want to reuse the same HTML across multiple views. like functions
- for example the `footer` ,it's the same in all pages so you can create new ejs file called footer and inside it put :

```
<!-- views/partials/footer.ejs -->
    <footer class="footer">
        <p>© 90210 Lawyer Stuff.</p>
    </footer>
```

and by using ejs templating notation "`<% %>`" you include it in any page you want :

```
<%- include('partials/footer') %>
```
