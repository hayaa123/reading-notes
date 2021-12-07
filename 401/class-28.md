# Working with forms

- An HTML Form is a group of one or more fields/widgets on a web page, which can be used to collect information from users for submission to a server

## Django form handling process

![](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Forms/form_handling_-_standard.png)

- Display the default form the first time it is requested by the user.

- Receive data from a submit request and bind it to the form.

- Clean and validate the data.

- If any data is invalid, re-display the form, this time with any user populated values and error messages for the problem fields.

- If all data is valid, perform required actions 

- Once all actions are complete, redirect the user to another page.


## Declaring a Form

1- ```
    from django import forms

    class RenewBookForm(forms.Form):
        renewal_date = forms.DateField(help_text="Enter a date between now and 4 weeks (default 3).")```


resorses 

[Working with forms](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Forms)