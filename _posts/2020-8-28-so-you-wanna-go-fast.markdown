---
layout: post
title:  "Welcome to Jekyll!"
date:   2017-11-10 15:15:15 -0500
categories: jekyll update
---
Why overclock? So you wanna go fast, huh? This is documentation of my journey of overclocking my i5 4690k.

[so you wanna go fast gif]

Again, please note this is a journal following my overclocking journey. It is not advice, and overclocking has inherent risks, including possibly frying your CPU completely (though this is unlikely unless you really push it to the limit^tm). I will also document what worked for me, though YMMV depending on your silicon lottery^{footnote}.

# What is clockrate?
# Clockrate and Voltage

Generally, the strategy you should be taking is as follows:
	(1) Try target clockrate (a quick google helps a lot). For the i5 4690k, 4.5Ghz is a good benchmark.
	(2) Update CPU voltage accordingly. This is composed of ring voltage and ___.
	(3) Run stability tests.
	(4) Repeat above, adjusting according to your stability test. If unstable at low temp, try going up. If unstable at high temp, reduce clockrate. Remember, pushing more than *X* volts through your chip is reaching dangerzone territory. I recommend staying below 1.3v. The marginal benefit of pushing it past is really not worth it, as you might actually fry your chip, while performance increases will be on the order of single percentage digits.

You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
