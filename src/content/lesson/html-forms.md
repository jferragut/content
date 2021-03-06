---
title: "HTML Forms"
subtitle: "Forms are really easy to understand, and they are the ONLY way to make interactive websites without AJAX.

These very basic concepts represent 90% of everything you will ever need to know about forms."
time: "3 minutes"
date: "2018-01-11"
tags: ["fale"]
---

# **HTML Forms**
***

This lesson is very easy to understand – but it is essential in that in this new knowledge, all of the interactivity of the internet will be relayed.  There are a few additional HTML tags that we need to discuss before finishing the Pre-Work: they are the first possible ways of interaction that were introduced in HTML: The Inputs and Forms.

Like always, let’s compare our website with an MS Word document…At some point scientists needed to create forms just like the ones we fill out when we pay our taxes: with blank spaces available for the user to fill with their Name, Last Name, Date of Birth, etc.

![forms](https://ucarecdn.com/9148fbd4-338b-4f0c-aada-9024ed4d6f85/)

The elements that the user fills in a form are called `<inputs>` and they always have to be wrapped inside of a `<form>` tag.  You can also use all the other HTML tags we learned in the previous lessons without any problems.

Here is an example of a simple form in HTML:

<iframe width="100%" height="300" src="//jsfiddle.net/BreatheCode/xmg974pn/embedded/html,css,result/" allowfullscreen="allowfullscreen" allowpaymentrequest frameborder="0"></iframe>

The following is a list of all the possible elements we can use to receive any input from the user:

|**Name**   |**Declaration**   |**Description**   |
|:----------|:-----------------|:-----------------|
|Text       |`<input type=”text”>`   |The text input is meant to receive any small string of characters such as: Username, Name, Last Name, Date of birth, etc.<br>`<input type="text" name="Name" />name="comments"><textarea/>`   |
|Textarea   |`<textarea>`   |The textarea is ideal for long text inputs.  Its main difference from the text input is its ability to allow for multiple lines.<br>`<textarea name="comments"><textarea/>`   |
|Password   |`<input type="password" />`   |This is just like an input type="text" but with the only difference that the characters are hidden like bullets – the user cannot see what  they are typing.<br>`<input type="password" name="password" />`   |
|Radiobutton   |`<input type=”radio”>`   |Allows the user to select only one of all the inputs with the same name.<br>`<input type="radio" name="color" value="red" />` <br> `<input type="radio" name="color" value="green" />`   |
|Checkbox   |`<input type=”check”>`   |You have to use brackets in the name of the input to allow the user to select multiple options at the same time.<br>`<input type="check" name="color[]" value="green" />`<br> `<input type="check" name="color[]" value="blue" />`   |
|File   |`<input type="file">`   |This is the only way to work with files.  Eg: It’s what websites use when they ask you to upload a picture.<br>`<input type="file" name="photo" value="" />`   |
|Submit Button   |`<input type="submit">`   |When the form is ready to be sent, the user presses this “submit” button and everything is then sent to the server for processing.<br>`<input type="submit" value="Send Form" />`   |
|Select   |`<select>`   |Asks the user to pick one or more elements from a list of options.<br>`<select name="color" /> <option value="red">Red </option> <option value="yellow">Yellow</option> <select />`   |

# **Input Attributes**
***

Just like any other HTML tag, the input tags have several attributes that can be set to describe their behavior in more specific ways:

VALUE:  You can specify a default value that the input should have before it starts getting filled by the user:

```html
<input type="text" name="firstname" value="John">
```
READ ONLY:  Determines if the user is allowed to change the value of the input.

```html
<input type="text" name="firstname" value="John" readonly>
```

DISABLED:  Determines if the input is going to be gray and read-only.  The disabled inputs are not sent to the backend – they act as if they never existed.

```html
<input type="text" name="firstname" value="John" disabled>
```

SIZE:  The maximum number of characters allowed for that input.

```html
<input type="text" name="firstname" value="John" size="40">
```

# The forms METHOD and ACTION
***


The two most important attributes that need to be set into the `<form>` tag are action and method:

Action: Is the URL where the data collected from the form is going to be sent.

Method: Can be either “POST” or “GET” – the main differences will be: (1) How the collected data is going to be sent to the destination page once we arrive there and (2) How the form data is submitted to the server.

|**Using method GET**   |**Using method POST**   |
|:----------------------|:-----------------------|
|All form data is encoded into the URL.  This means that it will append all the information of the form to the end of the destination URL like this:http://www.mydestinationurl.com?input_name1=value1&input_name2&value2…..   |The data will be hidden from the end-user.  The URL will remain as it was defined in the "action" attribute and only a developer will be able to request the form information.   |

[[warning]]
| :point_up:If you are going to use the `<input type=”file”>` the only method supported is POST.

# Welcome to the Web 2.0
***

You now know all the basics to create your first interactive website.  Now, if only you knew any backend language to process the data that is being collected from your forms!  In the meantime, you can try this free service to start the modjo! https://formspree.io/






  		


