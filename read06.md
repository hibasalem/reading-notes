# Read: 06 - Design web pages with CSS

## Chapter 10: Introducing CSS

CSS allows controlling how the content of an element should appear. CSS works as if there is an invisible box around every HTML element.
***Block level elements*** look like they start on a new line &lt;h1> &lt;h6>, <&lt;p> and &lt;div> elements.
***Inline elements*** flow within the text and do not start on a new line. Examples include &lt;b>, &lt;i>, &lt;img>,&lt;em> and &lt;span>.
A ***CSS rule*** contains two parts: a ***selector*** (which element the rule applies to) and a ***declaration*** (how the elements referred to in the selector should be styled and it split into two parts (a property and a value)).

CSS rules usually appear in a separate document, although they may appear within an HTML page.
##### Using External CSS
The <link> element can be used in an HTML document to tell the browser where to find the CSS and it lives inside the <head> element.It should use three attributes:href type rel
##### Using Internal CSS 
we can also include CSS rules within an HTML page by placing them inside a <style> element,
which usually sits inside the <head> element of the page.
The <style> element should use the type attribute to indicate that the styles are specified 

## Chapter 11: Color

The colour property allows us to specify the colour of text inside an element. we can specify any colour in CSS in one of three ways: RBG value hex codes colour names.

It is important to ensure that there is enough contrast between any text and the background colour (otherwise people will not be able to read the content).

examples : ***Background Color*** background-color ***Opacity*** opacity, rgba ( we add a number at the end for the opacity value 0.5 for example).
CSS3 also allows you to specify colours as HSL values, with an optional opacity value. It is known as HSLA.
