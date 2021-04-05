## Sending form data

**Client/server architecture**
![client-server](https://developer.mozilla.org/en-US/docs/Learn/Forms/Sending_and_retrieving_form_data/client-server.png)
The client send a request whe he submit the form to the server (HTTP request). then the server response for that request.

- In the form there is attribute called `action` , it specified **where** the data well send , other mean it define the end point or valid URL

- The `method` attribute , it define **how** data is sent.

  - GET method : this method send data to server appended with URL.
  - POST method : send data to server appended to the body of HTTP request.

- you can see the HTTP request inside network tap in the inspector.

- On the server side: retrieving the data

  - after you send HTTP request you can access this list depends on the development paltform , for example : `Raw PHP` , `Python`
  - `PHP` offers ome global objects to access the data :

  ```
  <? php
  // The global $_POST variable allows you to access the data sent with the POST method by name
  // To access the data sent with the GET method, you can use $_GET
  $say = htmlspecialchars($_POST['say']);
  $to  = htmlspecialchars($_POST['to']);

  echo  $say, ' ', $to;
  ?>
  ```

  - `Python`:

  ```
  from flask import Flask, render_template, request
  app = Flask(**name**)

  @app.route('/', methods=['GET', 'POST'])
  def form():
  return render_template('form.html')

  @app.route('/hello', methods=['GET', 'POST'])
  def hello():
  return render_template('greeting.html', say=request.form['say'], to=request.form['to'])

  if **name** == "**main**":
  app.run() 
  ```

- A special case: sending files : 
  - method attribute should be POST because file content can't be put inside URL parameters.
  - Set  the value of enctype to multipart/form-data because the data will be split into multiple parts.
  - Include one or more `<input type="file">` controls to allow your users to select the file(s) that will be uploaded 
  - Example :
  
  ```
  <form method="post" action="https://www.foo.com" enctype="multipart/form-data">
  <div>
    <label for="file">Choose a file</label>
    <input type="file" id="file" name="myFile">
  </div>
  <div>
    <button>Send the file</button>
  </div>
  </form>
  ```