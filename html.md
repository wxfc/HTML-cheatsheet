# HTML Cheatsheet

1.  `<!-- -->`

To write notes within your code

2.  `<!DOCTYPE html>`

Every html text file has to begin with this declaration, which lets the browser know that this begins a HTML page. It is technically not a HTML tag, but rather an instruction given to the browser about the version of HTML being used.

3.  `<a>`

This tag is for hyperlinks and stands for 'anchor'. Anchor can be used to link to many kinds of resources, such as email, files, and other content elsewhere on the same page.
**Attributes**

- **href**: is the main attribute, which specifies what one is linking to. Can be either an absolute(will have a URL address as the content beginning with http:// or https:// (the second version is the more secure version of the same URL)) or relative link (will specify the path to be followed from the page’s location in the browser directory to the file it is referencing).
- **download**: is added if the link is to explicitly download the content. Adding this attribute after the path name will direct the browser to download the file.
- **hreflang**: is an attribute that explicitly names the language of the document being linked to.
- **media**: tells the browser what target device the site has been designed for, in order to produce an optimal experience. eg.
  `media="all"`
  would mean that the content renders well on all displays and devices. Specifications for multiple devices can be used by using these logical operators:
  - and
  - not
  - , (a comma is used as the logical operator that means or)

The following can be used as the values for the media attribute:

- **aural**: speech synthesizers
- **braille**: braille devices
- **projection**: projectors
- **print**: print for pages and preview
- **screens**: screens
- **tty**: teletypes
- **tv**: lower resoluton televisions

There are more properties that are used for more fine-tuned media targeting.

- **ping**: can be used to send an HTML POST request to a designated web server if the link is clicked on. This provides one way of tracking user behaviour on site, so that if the link is clicked, the site creator is notified.
- **rel**: in this context specifies the nature of the relationship between the document with the link and the resource being linked to. The possible relationships (which are values to he **rel** attribute) that can be named between the link and its resource are:

  - **alternative**: gives an alternative URL for the link
  - **author**: gives a link to the author page
  - **coursemark**: is used for creating coursemarks
  - **external**: indicates that the link is to help resource
  - **license**: provides a link to a licensing reference
  - **next**: links to the next document if it is part of a sequence of pages
  - **nofollow**: asks web spiders not to follow you as you on the web as you activate the link
  - **noreferrer**: asks the browser not to send HTTP referrer information
  - **noopener**: is a security value that requires the next page not to have any window openers active, which might exploit a vulnerability
  - **prev**: specifies a link to a web page that is the previous on in a sequence
  - **search**: indicates a link to a futre search feature
  - **tag**: gives a keyword for the webpage

- **target**: it speficies how the link should be opened in the browser. It's values are:

  - **\_blank**: opens the page in a new tab
  - **\_parent**: opens the page in the parent browsing context
  - **\_self**: opens the page in the current browser frame
  - **\_top**: the top-most context for browsing

- **type**: is used to designate what are called Media Types. A typical use is to descibe the kind of text file being linked to. For instance, when linking to a stylesheet one will designate the media type as:
  `type="text/css"`
  More can be found at http://bit.ly/mediaTypes

4. `<abbr>`

Is used for definging acronyms or abbreviatons. This tag can be helpful for the machine reading of websites, so that scripts get at the meaning inside of letters that form an abbreviation. eg.
`<p><abbr title="Prisoner of War>POW</abbr></p>`

5. `<address>`

This tag designates contact information for the content of its nearest parent element. If placed inside of the `<article>` tag, it represents the author of the article, while if it is located in the `<body>` tag, it refers to the contact information of the whole document. It usually renders by default in italics.

6. `<area>`

Is used inside of a `<map>` tag to create clickable areas known as 'hotspots' inside of an image. When we click on these areas, we activate a link that produces some kind of change in the browser.

7. `<article>`

Is used for areas of self-contained content hat hypothetically could be distributed on their own separately from the website.

8. `<aside>`

Is content related to but separated from someother content it is associated with. For example, information in a paragraph or article might be highlighted for additional emphasis, such as with a sidebar, is an aside.

9. `<audio>`

Is for playing audio content in the browser. Audio files are usually compressed for more efficient playback, since smaller files will stream more quickly than larger files. Audio files should be included, using the self-closing `<source>` tags. It takes type as attribute which has a value of either `audio/mpeg`, `audio/wav` or `audio/ogg`. Audio tag takes the following attributes:

- **autoplay**: will set the audio to play when it has been loaded into the browser
- **loop**: will set the audio to play a loop, repeating every time it finishes
- **muted**: will mute the audio output, perhaps to be unmuted later through JavaScript interaction
- **preload**: has three possible calue settings: **auto**, **metadata** and **none**. These values are for shaping the overall user experience
- **auto**: is used for loading the entire audio file when the page loads
- **metadata**: loads only the metadata associated with the audio file when the page loads
- **none**: instructs the browser not to load the audio file on page load
- **src**: gives the URL source information for locating the sound file

10. `<bold>`

Is the bold tag. The issue with bold as a tag concept is that it has no semantic meaning.

11. `<base>`

Is placed in the `<head>` to describe a root URL, relative to which subsequent URLs placed as values to href attributes will read like relative paths.

12. `<bdi>`

This tag's name stands for "bi-directional isolation" and provides a way for treating text that might be inserted dynamically, by JavaScript, into an HTML document which might be written in a different direction. Such insertions might involve the use of other languages such as Arabic, that are read right-to-left.
