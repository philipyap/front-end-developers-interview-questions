# HTNL Questions

1. What does a doctype do ? 
    - It is important to add `DOCTYPE` declaration because it makes sure the document will be parsed the same way by different browsers.

2. How do you serve a page with content in multiple languanges ?
    - Always use a language attribute on the `html` element. This is inherited by all other elements, and so will set a default language for the text in the document head element.

3. What kind of things must you be wary of when designing or developing for multilingual sites ?
    [answer](https://fedev.tech/topic/html/5b188f91b4327d001452788c/)
    - Use lang attribute in your HTML.
    - Directing users to their native language - Allow a user to change his country/language easily without hassle.
    - Text in images is not a scalable approach - Placing text in an image is still a popular way to get good-looking, non-system fonts to display on any computer. However, to translate image text, each string of text will need to have it's a separate image created for each language. Anything more than a handful of replacements like this can quickly get out of control.
    - Restrictive words/sentence length - Some content can be longer when written in another language. Be wary of layout or overflow issues in the design. It's best to avoid designing where the amount of text would make or break a design. Character counts come into play with things like headlines, labels, and buttons. They are less of an issue with free-flowing text such as body text or comments.
    - Be mindful of how colors are perceived - Colors are perceived differently across languages and cultures. The design should use color appropriately.
    - Formatting dates and currencies - Calendar dates are sometimes presented in different ways. Eg. "May 31, 2012" in the U.S. vs. "31 May 2012" in parts of Europe.
    - Do not concatenate translated strings - Do not do anything like "The date today is " + date. It will break in languages with different word order. Use a template string with parameters substitution for each language instead. For example, look at the following two sentences in English and Chinese respectively: I will travel on {% date %} and {% date %} 我会出发. Note that the position of the variable is different due to grammar rules of the language.
    - Language reading direction - In English, we read from left-to-right, top-to-bottom, in traditional Japanese, text is read up-to-down, right-to-left.