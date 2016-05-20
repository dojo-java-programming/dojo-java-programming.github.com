---
layout: post
title: Continuous Integration with [Travis-CI](travis-ci.org)
---

## Action Plan

- Create the Travis-CI configuration file `.travis.yml`

__Oracle Java 1.7 Project__

file `.travis.yml`
{% highlight java %}
language: java
{% endhighlight %}


__Oracle Java 1.8 Project__

file `.travis.yml`
{% highlight java %}
language: java
 
jdk:
  - oraclejdk8
 
addons:
  apt:
    packages:
      - oracle-java8-installer
{% endhighlight %}

- Add, Commit and Push the configuration file to GitHub repository
![_config.yml]({{ site.baseurl }}/images/sign-in-with-github.png)
- Open your account on https://travis-ci.org with your GitHub identity 
- Add the GitHub repository to the Travis-CI dashboard
- Add the build status of Travis-CI as an link to the projects `README.md`
