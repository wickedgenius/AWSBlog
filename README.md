# AWSBlog

Blog built entirely for use in Amazon S3 without any server side code.

## Motivation

Having recently completed an AWS course I decided that a blog on my use of AWS would be a nice further learning experience, and where better to put it than into S3! Unfortunately I couldn't find any server-less blogs that I liked and decided to put something together using just client side technologies.

## Installation

The following settings can be set in the js/AWSBlogSettings.js file:

* BlogTitle: The title of your blog, this is the title shown at the top of every page and in the browser title.
* PostsOnPage: This sets the number of posts found on each page of the main posts listing.

For each blog post you want to make there are two things to do:

1. Add an entry to the BlogPosts array in articles.json file that looks like this:
	```JSON
	{
		"PostTitle": "Welcome!",
		"CreatedDate": "May 05, 2017 23:17:00",
		"Author": "Aaron",
		"Path": "articles/welcome.html"
	}
	```
2. Create an html file at the location you've pointed the path above to, it doesn't need any special markup just needs to be a document that can use HTML for styling, here's an example:
	```HTML
	<p>Welcome to my Blog!</p>
	
	<p>I can have all sorts of content:<br />
	<b>bold</b>
	<i>Italic</i>
	<ul>
		<li>lists</li>
		<li>stuff</li>
	</ul>
	and more!</p>
	```

## Contributors

At present this is solely maintained by myself but if you would like to assist then drop me a message.

## License

This project is made available under the MIT license.