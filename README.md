Version
-------
1.0.4 released. Check out https://rubygems.org/gems/dq-readability

* competing structure for fighting invalid characters
* Wikipedia image case resolved

Install
-------
Command line:

    (sudo) gem install dq-readability

Bundler:

    gem "dq-readability"
Example
-------
    require 'rubygems'
    require 'dq-readability'
    source = "http://www.personal.kent.edu/~rmuhamma/Algorithms/MyAlgorithms/Sorting/radixSort.htm"
    puts DQReadability::Document.new(source,:tags=>%w[div pre p h1 h2 h3 h4 td table tr b a img br li ul ol center br hr blockquote em strong sub sup font tbody tt span dl dd t code figure fieldset legend dir noscript],:attributes=>%w[href src align width color height]).content
