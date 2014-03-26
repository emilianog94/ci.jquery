# jQuery CI Validator

jQuery plugin to validate Uruguayan Identity Documents (Cedula de
Identidad Uruguaya).

This plugin will validate a text input's content as a Uruguayan CI
number. It will add 'valid' or 'invalid' classes to an input.
Check out [example.html](example.html) to see how it works or see below:

## Usage:

```html
<style>
  input.valid{
    background: #9deb91;
  }
  input.invalid{
    background: #eb91ae;
  }
</style>

<input type="text" name="ci" id="ci"/>

<script type="text/javascript" src="https://code.jquery.com/jquery-1.11.0.min.js"></script>
<script type="text/javascript" src="./ci.jquery.js"></script>
<script type="text/javascript">
  $("#ci").keyup(function(){
    $("#ci").validate_ci(); // adds 'valid' or 'invalid' classes to the input on keyup
  });
</script>
```
