---
layout: default
title: Overview
permalink: overview
---

{% include template-h1.html %}

## What's C# Eval Expression library?

Our library is a lightweight expression evaluator that support nearly everything. You can evaluate or compile almost all possible C# expression including:

- Anonymous Type
- Extension Method
- Lambda Expression
- LINQ
- Method Overloads

It supports:

- NET40+
- NET Standard 1.3

It’s easy to use, and easy to customize.

{% include template-example.html %} 

{% highlight csharp %}
int result = Eval.Execute<int>("X + Y", new { X = 1, Y = 2});

int result = Eval.Execute<int>(@"
    var list = new List<int>() { 1, 2, 3, 4, 5 };
    var filter = list.Where(x => x < 4);
    return filter.Sum(x => x);");
{% endhighlight %}

### Is it that simple?

Yes,

You add a valid expression and execute it.

That’s why people feel in love so quickly with our library.

### Who use it?

Already **hundreds** of companies of all sizes and kinds use it:

- From start-up company with one developer
- To fortune 100 companies with hundreds of developers

Are you still not using it? Give it one try, and you will understand why they choose our library.
