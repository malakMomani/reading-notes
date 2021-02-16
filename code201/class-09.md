# Chapter 7 : FORMS

**Form Controls** :
- **Adding text** : 
  - Text Input : single line of text.
  - Password input : single line but masks the characters entered.
  - Text area : long texts.
- **Making Choices** : 
  - Radio buttons : select option (only one).
  - Checkboxes : select onr or more option.
  - Drop-down boxes : pick option from list.

**How forms work** : 
user fill the form -> press button to submit the information to server -> each control inside form with value off user -> server process it using one of programming language .

- each form control has a name and tke its value from the user.

**Form Structure**
```
<form action="http://www.example.com/subscribe.php"
  method="get">
  <p>This is where the form controls will appear.
    </p>
</form>
```
- < form> : carry action attribure and method.
- < action> : have the url for the page on server that will recieve the info.
- < method> : `get` or `post`.

**Text Input** : 
using `< input>` tag.
- `type = "text"`.
- `name` : name of the text field.
- `maxlength` : limit of number of charcter a user may enter. 
inside `form` tag :

```
<p>Username:
  <input type="text" name="username" maxlength="30" />
</p>
```

**password Input** : 
using `< input>` tag
- `type = "password"`.
- `name` : name of the password text field.
- `maxlength` : limit of number of charcter a user may enter. 
inside `form` tag :

```
<p>Password:
  <input type="password" name="password" maxlength="30" />
</p>
```
 
**Text Area** : element by itself
inside `form` tag
```
<textarea name="comments" cols="20" rows="4">Enter
 your comments...</textarea>
```

**Radio Button** :
using `< input>` tag
- `type = "radio"`.
- `name` : name of the radio button
- `value` : the value radio button
- `checked` : can use to indicate which value should be checked by default.
inside `form` tag :
```
<p>Enter your gender
 <input type="radio" name="gender" value="male"
 checked="checked" /> Male
 <input type="radio" name="gender" value="female" />
 Female
</p>
```

**CheckBox** :
using `< input>` tag
- `type = "checkbox"`.
- `name` : name of the checkbox
- `value` : the value checkbox
- `checked` : can use to indicate which value should be checked by default.
inside `form` tag :
```
<p>Enter your hobbies
 <input type="checkbox" name="hobby" value="swimming"
 checked="checked" /> Swimming
 <input type="checkbox" name="hobby" value="reading" /> Reading
</p>
```

**Drop Down List Box**:
using `< select>` and `option` tag.
- `name` : name of the drop down list
- `value` : the value drop down list
- `selected` : can use to indicate which value should be selected by default.

inside `< form>` tag:


```
<p>What programming language you love?</p>
<select name="PL">
 <option value="c++">C++</option>
 <option value="html">HTML</option>
 <option value="android">Android</option>
 </select>
```
**File Input Box**
using `< input>` tag
- `type="file"`

**Submit button**
using `< input>` tag
- `type="submit"`
- `name` : name of the button
- `value` : the value button

**Image button**
using `< input>` tag
- `type="image"`
- `name` : name of the button

-----------------------------------------------------
# Chapter 14 
