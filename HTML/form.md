
noteId: "5a105bf002f511f093afeff3c7fba90f"
tags: []

# HTML Form
 - Html Forms are used to collect user input and send them to the server.
 - They are essential for creating interactive web applications.
 ## Basic structure
 ```
    <form action="/submit" method="POST">
        <label for="username">Username:</label>
        <input type="text" id="username" name="username">
        <label for="password">Password:</label>
        <input type="password" id="password" name="password">
        <input type="submit" value="Submit">
    </form>
```
## Explanation
    <form> - Container for all forms elements.
    action - the URL where data is submitted.
    method - HTTP method used to sent data (GET or POST).
    <label> - Associate text with input for accessibility.
    <input> - the field where users enter data.
    type - defines the kind of input field(text, password, email, tel, submit).
    name - identifier used to reference the form data on the server.

# Input types and examples
## 1.Textual Input
```
  <input type="text" name="fullname" placeholder="Full Name" required>

   <input type="email" name="email" placeholder="Email Address" required>

   <input type="password" name="password" placeholder="Password" required>

   <input type="number" name="age" min="1" max="100">
```

## 2. Checkboxes and radio 
```
<label><input type="checkbox" name="subscribe"> Subscribe to newsletter</label>
<label><input type="radio" name="gender" value="male"> Male</label>
<label><input type="radio" name="gender" value="female"> Female</label>
```

## 3. File upload and hidden fields
```
<input type="file" name="profile_picture" accept="image/*">
<input type="hidden" name="user_id" value="12345">
```

## 4. Tel and URL inputs
```
<input type="tel" name="phone" placeholder="123-456-7890">
<input type="url" name="website" placeholder="https://example.com">
```

## 5. Submit, reset and button
```
<input type="submit" value="Submit">
<input type="reset" value="Reset">
<button type="button" onclick="alert('Button Clicked!')">Click Me</button>
```

## 6. Select (Dropdown)
```
<label for="cars">Choose a car:</label>
<select name="cars" id="cars">
  <option value="volvo">Volvo</option>
  <option value="saab">Saab</option>
  <option value="mercedes">Mercedes</option>
  <option value="audi">Audi</option>
</select>
```

## 7. Datalist(AutoComplete)
```
<label for="browsers">Choose a browser:</label>
<input list="browsers" name="browser">
<datalist id="browsers">
  <option value="Chrome">
  <option value="Firefox">
  <option value="Safari">
  <option value="Edge">
  <option value="Opera">
</datalist>
```

# Accessibility
- Use ```<label>``` for every ```<input>``` for better accessibility.
- Add aria-label, aria-labelledby, or aria-describedby where needed.
- Ensure good contrast ratios between text and background.
- Use tabindex for keyboard navigation.
