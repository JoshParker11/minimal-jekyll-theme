---
layout: post
title: how to use Jekyll
date: 2015-05-28 13:20:50 +0100
author: Desired Persona
categories:
  - minimal
---

You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `bundle exec jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

{% highlight cpp %}
class Job
{
public:
    Job() = default;
    Job(void(*jobFunction)(Job&), Job* parent = nullptr);

    void run();
    bool finished() const;

private:
    void(*_jobFunction)(Job&);
    Job* _parent;
    std::atomic_size_t _unfinishedJobs;

    void finish();
};
{% endhighlight %}

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: http://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
