---
layout: post
title: Code Logging
categories: [CLog]
tags: [template]
Author: Rowan Maddigen
thumbnail: jekyll
summary: Code logging examples
---

This blog is what I call a code log, a place to post bits and pieces of code I find around the net along with the instructions on how to use them. Code Logging must be done such a way as to provide meaningful information and examples of code and output for ease of use.

Thus, I am making this Code Logging template page, so that those who get confused about the format of my logs might have a reference.

### One | Front Matter

All Code Logging posts must have the following in the front matter ( Do note, the front matter is not exactly visible to readers )

categories: [CLog]
tags: [varies,depending,on,type]

The category will always remain the same, it should be CLog, short for Code Log, the tags, on the other hand, will vary depending on what type of code is in that log, so I might use the tags [html,css] for example, or [html,css,js] or even [php] or [c#] any number of things. It just really all depends.

### Two | Code Blocks

Code blocks are specially highlighted to set them apart from normal text, an example of this is below...

{% highlight ruby %}
def show
  @widget = Widget(params[:id])
  respond_to do |format|
    format.html # show.html.erb
    format.json { render json: @widget }
  end
end
{% endhighlight %}

and another example...

{% highlight html %}
<h1>Hello World</h1>
<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer at diam eu lacus pellentesque venenatis vel nec purus. Vivamus euismod, diam vel cursus condimentum, justo dolor vulputate ante, eget vulputate justo justo eget ipsum.</p>
{% endhighlight %}

I think you get the idea.
