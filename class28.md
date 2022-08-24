# Django Forms 

Forms are useful because they can provide a secure way to share data with the server, and let us send data through `POST` requests. Django provides and easier way to programmatically to generate the form HTML code and work with the user interaction. 

## Django form handling process

1. Displays default form the first time it is requested by the user

2. receives data from the submit requests and binds it to the form 

3. Validates the data

4. If data is invalid it will re-display the form with error messages and for the problem fields. 

5. Once data is valid it moves on to performing required actions 

6. When actions are complete it redirects user to another page. 

## declaring a form 

To create a `Form` you have to import the forms library from the forms class and declare forms field. See example below: 

`from django import forms`

`class RenewBookForm(forms.Form):`
    `renewal_date = forms.DateField(help_text="Enter a date between` `now and 4 weeks (default 3).")`

Here are arguments for most fields 

- required 

- label

- label suffix 

- initial 

- Widget 

- help text 

- error messages 

- localize 

- disabled 

## Things I want to know more about 

I would like to see how the Django form is implemented in real time. 