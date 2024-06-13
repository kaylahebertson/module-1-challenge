# Module 1 Challenge

## Technology Used

| Technology Used         | Resource URL           | 
| ------------- |:-------------:| 
| HTML    | [https://developer.mozilla.org/en-US/docs/Web/HTML](https://developer.mozilla.org/en-US/docs/Web/HTML) | 
| CSS     | [https://developer.mozilla.org/en-US/docs/Web/CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)      |   
| Git | [https://git-scm.com/](https://git-scm.com/)     |  

## Description

[Visit the Deployed Site]()

In this project, a functional HTML and CSS were provided with instructions to make them more concise and accesible. Code refactoring allows the external function of code to remain the same while the internal structure is updated to be more organized and maintainable. 

## Code Refactor Example

To see this project, please click on the link in the description. Once at the deployed site, feel free to right click and choose inspect to see the code in function. Below are some examples of changes from the original to the updated code. 

```html
 <div class="benefits">
        <div class="benefit-lead">
            <h3>Lead Generation</h3>
            <img src="https://static.bc-edx.com/coding/full-stack/01-HTML-Git-CSS/assets/lead-generation.png" />
            <p>
                Inbound strategies for lead generation require less work for your business, bringing customers directly to your website.
            </p>
        </div>
        <div class="benefit-brand">
            <h3>Brand Awareness</h3>
            <img src="https://static.bc-edx.com/coding/full-stack/01-HTML-Git-CSS/assets/brand-awareness.png" />
            <p>
                Users find your business through paid and organic searches, increasing the search ranking and visibility for your business.
            </p>
        </div>
        <div class="benefit-cost">
            <h3>Cost Management</h3>
            <img src="https://static.bc-edx.com/coding/full-stack/01-HTML-Git-CSS/assets/cost-management.png" />
            <p>
                As the search ranking for your business increases, your advertising costs decrease, and you no longer need to advertise your page.
            </p>
        </div>
    </div>
```

Converting the above HTML with non-semantic div to more suitable [semantic elements](https://www.w3schools.com/html/html5_semantic_elements.asp). Adding [img alt attributes](https://www.w3schools.com/tags/att_img_alt.asp) to make HTML more accessible.

```html
    <aside>
        <section>
            <h3>Lead Generation</h3>
            <img src="https://static.bc-edx.com/coding/full-stack/01-HTML-Git-CSS/assets/lead-generation.png" alt="gear turning into money" />
            <p>
                Inbound strategies for lead generation require less work for your business, bringing customers directly to your website.
            </p>
        </section>
        <section>
            <h3>Brand Awareness</h3>
            <img src="https://static.bc-edx.com/coding/full-stack/01-HTML-Git-CSS/assets/brand-awareness.png" alt="lit up light bulb" />
            <p>
                Users find your business through paid and organic searches, increasing the search ranking and visibility for your business.
            </p>
        </section>
        <section>
            <h3>Cost Management</h3>
            <img src="https://static.bc-edx.com/coding/full-stack/01-HTML-Git-CSS/assets/cost-management.png" alt="gear surrounded by money" />
            <p>
                As the search ranking for your business increases, your advertising costs decrease, and you no longer need to advertise your page.
            </p>
        </section>
    </aside>
```

Changing the HTML required some changes to the CSS.

```css
.benefit-lead {
    margin-bottom: 32px;
    color: #ffffff;
}

.benefit-brand {
    margin-bottom: 32px;
    color: #ffffff;
}

.benefit-cost {
    margin-bottom: 32px;
    color: #ffffff;
}

.benefit-lead h3 {
    margin-bottom: 10px;
    text-align: center;
}

.benefit-brand h3 {
    margin-bottom: 10px;
    text-align: center;
}

.benefit-cost h3 {
    margin-bottom: 10px;
    text-align: center;
}

.benefit-lead img {
    display: block;
    margin: 10px auto;
    max-width: 150px;
}

.benefit-brand img {
    display: block;
    margin: 10px auto;
    max-width: 150px;
}

.benefit-cost img {
    display: block;
    margin: 10px auto;
    max-width: 150px;
}
```

The original targeted class of 'benefit' is no longer in use, rather the 'aside' element is being targeted as seen below. CSS code was also consolidated where possible.

```css
aside section {
    margin-bottom: 32px;
    color: #ffffff;
}

aside h3 {
    margin-bottom: 10px;
    text-align: center;
}

aside img {
    display: block;
    margin: 10px auto;
    max-width: 150px;
}
```

## Usage

This project is intended to be an aid for code refactoring. Simply examine the code to see how HTML and CSS work together. 

## Learning Points

This project helps teach the importance of using semantic elements to help clearly define what is going on in an HTML. I learned how to create a more readable code that helps the user see the layout more clearly. I also learned how to use a CSS to enhance the overall flow and design of the HTML. I learned how to target specific classes as well as elements as a whole.

## Author Info

```md
Kayla Hebertson

* [Github](https://github.com/kaylahebertson)
* [LinkedIn](www.linkedin.com/in/kayla-hebertson)
* [Portfolio](coming soon)

```


## Credits

Coding Bootcamp

## License

Please refer to the LICENSE in the repo.
