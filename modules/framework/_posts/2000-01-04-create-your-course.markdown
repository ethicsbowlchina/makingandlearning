---
title: Create your course
---

## Taking your course out of the box

You're going to be building your course in GitHub. GitHub is web-based repository hosting service, which allows you to manage your code, and see revisions you've made via a good-looking, easy-to-use web interface. It's newbie-friendly, and a great collaboration tool, which is why we're using it for Course in a Box.

The flagship functionality of GitHub is “forking” – copying a repository from one users account to another. This is what we will do with this repository of content. By forking repository you will copy the Course in a Box content from our repository, and modify it under your own account and then publish with your own link to it.

Your course will live on GitHub (so you don't need to worry about hosting) and you'll do all the building work there, but you'll be able to view it as a web page.

### Let's get started:

When we asked you to fork this course you actually copied this course and started building your own!

This copy is where you will be working during the course. Some of the technical things may be challenging or frustrating, but by tackling it bit by bit and asking your peers for help, you’ll soon be an expert and helping other people!

<div id="ghUsername-intro">
Below we will be doing some proper work on GitHub. We hope you won't mind telling us your username, so we can prepare some links and make things much easier for you. Don't worry, we are not storing any information about you on our servers. If you have JavaScript disabled for some reason, you will need to replace 'your-github-username' with your GitHub username where you see links containing 'your-github-username'
</div>

[your-github-username](https://github.com/your-github-username-set/course-in-a-box/)

### Tweak a few items.
There are two updates that you need to make to your course to get it working. First, change

{% highlight yaml %}baseurl:{% endhighlight %}

to

{% highlight yaml %}baseurl: /course-in-a-box{% endhighlight %}

in the file [https://github.com/your-github-username/course-in-a-box/blob/gh-pages/_config.yml](https://github.com/your-github-username/course-in-a-box/blob/gh-pages/_config.yml)

Next, delete the file called CNAME [https://github.com/your-github-username/course-in-a-box/blob/gh-pages/CNAME](https://github.com/your-github-username/course-in-a-box/blob/gh-pages/CNAME)

Now that you have a space to work, lets put a draft framework in place for your course.

### Give your course a name.
To update the title of your course, go to [https://github.com/your-github-username/course-in-a-box/blog/gh-pages/_data/course.yml](https://github.com/your-github-username/course-in-a-box/edit/gh-pages/_data/course.yml) and edit the file called `_data/course.yml`. You will see the title for this course there, change that to the name you decided on. Don't worry too much if you don't have the perfect name, you now know how to change the title for your course and you can update it at any time!

{% highlight yaml %}title: "Course Title"{% endhighlight %}

### Who is the course for & what will they learn?
Will they be building something during the course. Put this basic information on the front page of the course to give a short overview of what to expect. To update the info on the front page, go to the file [https://github.com/your-github-username/course-in-a-box/blob/gh-pages/index.markdown](https://github.com/your-github-username/course-in-a-box/blob/gh-pages/index.markdown) and replace the text currently there to reflect what your course will be about. Once again, you can update it at any time and we will come back to this at a later stage.

### Lets have a look at your course!

You can view it by going to [https://your-github-username.github.io/course-in-a-box/](https://your-github-username.github.io/course-in-a-box/).
