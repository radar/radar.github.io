--- 
wordpress_id: 186
layout: post
title: Which Came First?
wordpress_url: http://frozenplague.net/?p=186
---
Today a question was asked by the work experience kid that made me think what in Ruby gets called first, a local variable or a method. The answer can be explained by this short irb example (thanks to Yuji Yukoo, a work mate of mine):

<pre lang='rails'>
irb(main):001:0> a = "b"
=> "b"
irb(main):002:0> def a
irb(main):003:1> "a"
irb(main):004:1> end
=> nil
irb(main):005:0> a
=> "b"
irb(main):006:0> a()
=> "a"
</pre>

Firstly we define a local variable called a, and then a method called a, and then we type a and press enter, and the local variable is outputted rather than the method. Next we call a() which outputs "a", the code defined within the method a. It's just one of those interesting things of note.
