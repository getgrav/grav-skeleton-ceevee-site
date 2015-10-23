---
title: Contact Form
menu: Contact
lead: Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo. Nemo enim ipsam voluptatem quia voluptas sit aspernatur aut odit aut fugit.
widgets:
    - title: Address and Phone
      content:
        - line: Jonathan Doe
        - line: 1600 Amphitheatre Parkway
        - line: Mountain View, CA 94043 US
        - line: (123) 456-7890

form:
    name: my-nice-form
    fields:
        - name: name
          label: Name
          placeholder: Enter your name
          autofocus: on
          autocomplete: on
          type: text
          validate:
            required: true

        - name: email
          label: Email
          placeholder: Enter your email address
          type: text
          validate:
            rule: email
            required: true

        - name: message
          label: Message
          size: long
          placeholder: Enter your message
          type: textarea
          validate:
            required: true

    buttons:
        - type: submit
          value: Submit

    process:
        - email:
            from: "{{ config.plugins.email.from }}"
            to:
              - "{{ config.plugins.email.from }}"
              - "{{ form.value.email }}"
            subject: "[Feedback] {{ form.value.name|e }}"
            body: "{% include 'forms/data.html.twig' %}"
        - save:
            fileprefix: feedback-
            dateformat: Ymd-His-u
            extension: txt
            body: "{% include 'forms/data.txt.twig' %}"
        - message: Thank you for your feedback!
        - display: thankyou
---

Morbi leo risus, porta ac consectetur ac, vestibulum at eros. Integer posuere erat a ante venenatis dapibus posuere velit aliquet. Cras justo odio, dapibus ac facilisis in, egestas eget quam. Morbi leo risus, porta ac consectetur ac, vestibulum at eros.
