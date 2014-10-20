---
title: Get acquainted
published: true
---

# Get into computer sphere with some cat help

![This is how we do binis]({{site.baseurl}}/img/codecatz/blinkoncomp.jpg)

Image [CC-BY-SA](https://creativecommons.org/licenses/by-sa/2.0/) by [iAlja](http://instagram.com/ialja) on Flickr.

During this course you will learn the theoretical and technical parts by 
creating your own online portfolio
![Applause](http://media.giphy.com/media/Hc8PMCBjo9BXa/giphy.gif)

## First of, join the CodeCatz properly
You thought we are interesting enough, that you visited us and hopefuly we did not turn you away,
by the heaps of chocolade we offered you.

Now is time for you to tell the whole wold you are now a CodeCat and that is why
we want you to put your lovely
little face on the front page of this course.

For this you'll need an account with [Github](https://github.com/).
If you don't have one, now is the best time to create one. Go ahead and then come back.

This course is built using [GitHub Pages](https://pages.github.com/).

To be presented as a proper CodeCat you'll need, to know a bit about git. 

OK, you will need to know quite a lot about git, but hey no worries, we are 
here to get you started. For now you'll just need to know how to fork repository
, how to add your lovely picture to this course and how to send a pull request, 
so we can publish it. Then we party!


<a class="btn btn-primary" href="https://github.com/ercchy/get-codecatz-smart/fork" target="_blank"><i class="fa fa-code-fork"></i> Fork this repository</a>

Some of the technical things may be challenging or frustrating, but by tackling 
it bit by bit and asking your peers for help, you’ll soon be an expert 
and helping other people. We promise!

### Tweak a few items. 
In your Github space there is a repository called "get-codecatz-smart". Click on it
and don't get intimidated by all the items you see inside. You do not need to 
know what they are just yet.

Find this file{% highlight yaml %}_data/course.yml{% endhighlight %}

On the top right you will see a button ![Little Pencil]({{site.baseurl}}/img/codecatz/little_pencil.png), by cliking on it you are able to edit
this file.

Where it says "signups" add your own data. Careful, data has to be in the same format as
all of the other is already. That means you have to watch out for the whitespaces,
they are important.

Example:
{% highlight yaml %}
 - name: Blink TheCat
  image: http://path/to/the/image
  twitter: blink
  github_username: blink
{% endhighlight %}

After you are done adding you info you will need to commit this change. 
That is just a fancy way of saying you are saving the change you made.

On the bottom of the editor, there is a space, where you describe what your
change is about. The description does not need to be very long, but it is a good
practice to put something descriptive.

![Your first commit]({{site.baseurl}}/img/codecatz/commit.png)

### Send your first pull request. 

Now this is the change that you did in your own repository, which is only a 
clone of the main CodeCatz repository. The change you made is reflected on
your repository, but the main one does not know anything about your changes
(how rude, but hey that is life...).

So we have to tell the main repository you have made something new and you
think it could be interesting for it. To let the main repository see the changes 
you made, we will need to send a pull request. That means we will request that
the main repository pulls our changes into itself and display your lovely image.

First press this button on the right side ![Pull Request Button]({{site.baseurl}}/img/codecatz/little_pull_request.png)

The page for the pull requests opens up and there is a new button that you'll need 
to press.

![Create new pull request]({{site.baseurl}}/img/codecatz/create_new_pull_request.png)

Now you can review the changes you made. The green lines is everything you added
and the red ones are everything you deleted or changed.

![Review the changes]({{site.baseurl}}/img/codecatz/review_changes.png)

After we reviewed all the changes we have made we are going to have to press the green
"Create pull request" button yet again. Yeah it takes a lot of convincing, we know.

![Create Pull Request Yet Again]({{site.baseurl}}/img/codecatz/create_pullrequest_after_review.png)

You will see that the description of your commit is automaticaly set into the 
title input box, and you can leave it as it is, or you can change it if there is 
something else you would like to say to the people who will look at your pull request.
We will leave it as it is now, because it is descriptive enough.
And will yet again press the big green button. This is the last time, promise!

![Send Pull Request]({{site.baseurl}}/img/codecatz/send_pullrequest.png)

Now we see the summary of our pull request.

![Pull Request summary]({{site.baseurl}}/img/codecatz/summary_of_pullrequest.png)

Bravo! You've send your first pull request. have yourself a treat.

![I regret nothing]({{site.baseurl}}/img/codecatz/iregretnothing.jpeg)

### What now?

Now we have to sit around and wait for the people who are maintainers of the main
repository look at our pull request and merge it.

After they will do that:

####Ta-da

![Who Else Is Here]({{site.baseurl}}/img/codecatz/who_else.png)

## Recap

You have just sent your first pull request. This means that now you need to start
learning for real.

