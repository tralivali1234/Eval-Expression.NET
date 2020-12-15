---
layout: default
title: LINQ Dynamic - Take
description: C# Dynamic LINQ Take examples using an Expression Evaluator.
permalink: linq-dynamic-take-examples
---

{% include template-h1.html %}

## LINQ Dynamic Take Examples
{{ page.description }}

- [Take - Simple](#take---simple)
- [Take - Nested](#take---nested)

## Take - Simple
This C# example uses the LINQ Take method with a dynamic expression to get only the first 3 elements of the array.

### LINQ
{% highlight csharp %}
private void uiTake_Simple_LINQ_Click(object sender, EventArgs e)
{
	int[] numbers = {5, 4, 1, 3, 9, 8, 6, 7, 2, 0};

	var first3Numbers = numbers.Take(3);

	var sb = new StringBuilder();
	sb.AppendLine("First 3 numbers:");

		foreach (var n in first3Numbers)
		{
			sb.AppendLine(n.ToString());
		}

	My.Result.Show(My.LinqResultType.Linq, uiResult, sb);
}
{% endhighlight %}

### LINQ Execute
{% highlight csharp %}
private void uiTake_Simple_LINQ_Execute_Click(object sender, EventArgs e)
{
	int[] numbers = {5, 4, 1, 3, 9, 8, 6, 7, 2, 0};

	var first3Numbers = numbers.Execute<IEnumerable<int>>("Take(3)");

	var sb = new StringBuilder();
	sb.AppendLine("First 3 numbers:");

		foreach (var n in first3Numbers)
		{
			sb.AppendLine(n.ToString());
		}

	My.Result.Show(My.LinqResultType.Linq, uiResult, sb);
}
{% endhighlight %}

### Result
{% highlight text %}
LINQ Execute Test
------------------------------
First 3 numbers: 
5 
4 
1

{% endhighlight %}

## Take - Nested
This C# example uses the LINQ Take method with a dynamic expression to get the first 3 orders from customers in Washington.

### LINQ
{% highlight csharp %}
// todo
{% endhighlight %}

### LINQ Dynamic
{% highlight csharp %}
// todo
{% endhighlight %}

### LINQ Execute
{% highlight csharp %}
// todo
{% endhighlight %}

### Result
{% highlight text %}
LINQ Execute Test
------------------------------
First 3 orders in WA: 
CustomerID=LAZYK OrderID=10482 OrderDate=3/21/1997 
CustomerID=LAZYK OrderID=10545 OrderDate=5/22/1997 
CustomerID=TRAIH OrderID=10574 OrderDate=6/19/1997

{% endhighlight %}
