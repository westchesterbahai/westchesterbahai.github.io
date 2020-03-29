---
title: Contact
layout: post
permalink: /contact/
---


<style>
.contact-li {
    list-style: none;
}

.contact-input {
    border:none;
    border-bottom: 1px solid #eee;
    width: 12em;
}

.contact-input:focus {
    outline:none;
    border-bottom: 1px solid #ea6111;
}

.contact-label {
    display: block;
}

ul.contact-ul {
    margin: 0;
    padding: 10px;
}

#submit {
    border:none;
    background-color: #ea6111;
    padding: 5px 15px;
    color: #eee;
    opacity: 0.8;
}

#submit:hover {
    opacity: 1;
    cursor: pointer;
}


#contact-form {
    border: 1px solid #aaa;
    display: inline-flex;
    margin-bottom: 1em;
}

</style>

This is a placeholder for a "contact us." I'd prefer to direct people to actual activities, but this is immediate. The 1-800-22-UNITE is also a good option.

<form id="contact-form" class="form" action="https://getsimpleform.com/messages?form_api_token={{site.api-token}}" method="POST" enctype="multipart/form-data">
        <ul class="contact-ul">
            <li class="contact-li">
                <label class="contact-label" for="name">Name:</label>
                <input type="text" placeholder="Your name" id="name" class="contact-input" name="name" tabindex="1"/>
            </li>
            <li class="contact-li">
                <label class="contact-label" for="email">Email:</label>
                <input type="email" placeholder="Your email" id="email" class="contact-input" name="email" tabindex="2"/>
            </li>
            <li class="contact-li">
                <label class="contact-label" for="message">Message:</label>
                <textarea class="contact-textarea" placeholder="Your message" class="contact-input" rows="4" id="message" name="message" tabindex="3"></textarea>
            </li>
            
        </ul>
        <input type="submit" value="Send" id="submit"/>
        
</form>

This form is setup using [SimpleForm](https://getsimpleform.com){: target="_blank" rel="nofollow"}. You can get your own API token and update it in the **_config.yml** file.

The styles for the form is included in this page. I haven't included it in the main css because the form has at least 25 lines of css and it is used only on this page. So including it in main css file doesn't make sense.
