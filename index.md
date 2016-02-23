---
layout: post
---

<html lang="en">
	<head>
		<meta charset="utf-8">
		<meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
		<meta http-equiv="x-ua-compatible" content="ie=edge">
		<meta name="msvalidate.01" content="89359D9C492A475C0061398008D105FB" />
		
		<!-- seo !-->
		<meta name="description" content="Evaluate, Compile and Execute dynamic C# code and expression at runtime">
		<meta name="keywords" content="Eval, Evaluate, Compile, Execute, Expression, Dynamic, Runtime, .NET, dotnet, C#, CSharp, VB">
		<title>C# Eval Function | C# Expression Evaluator to Evaluate, Compile and Execute dynamic C# code and expression at runtime.</title>
		
		<!-- icon/css !-->
		<link rel="icon" type="image/png" href="http://entityframework-plus.net/images/logo.png">
		<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0-alpha.2/css/bootstrap.min.css" integrity="sha384-y3tfxAZXuh4HwSYylfB+J125MxIs6mR5FOHamPBG064zB+AFeWH94NdvaCBm8qnd" crossorigin="anonymous">
		<link rel="stylesheet" type="text/css" href="https://maxcdn.bootstrapcdn.com/font-awesome/4.4.0/css/font-awesome.min.css">
		<link rel="stylesheet" type="text/css" href="http://entityframework-plus.net/css/github2.css">
		<link rel="stylesheet" type="text/css" href="http://entityframework-plus.net/css/default.css">
	</head>
	
	<body>
  
		<!-- top-header !-->
		<div id="top-header">
			<div class="container">
				<div class="text-right">
					<a href="mailto:info@zzzprojects.com"><i class="fa fa-envelope"></i>&nbsp;&nbsp;info@zzzprojects.com</a>
					<a href="https://www.facebook.com/zzzprojects" target="_blank"><i class="fa fa-facebook"></i></a>
					<a href="https://twitter.com/zzzprojects" target="_blank"><i class="fa fa-twitter"></i></a>
					<a href="https://plus.google.com/+Zzzprojects_NetSQL" target="_blank"><i class="fa fa-google-plus"></i></a>
					<a href="http://zzzprojects.us9.list-manage.com/subscribe?u=cecbc4775cf67bf1ff82018af&id=4765ffa5f8" target="_blank" class="hidden-xs-down"><i class="fa fa-newspaper-o"></i></a>
				</div>
			</div>
		</div>
		
		<!-- header !-->
		<header>
			<div class="container">
				<div class="row">
					<div class="col-lg-6">
						<div class="card">
							<div class="card-block">
								<h3 class="card-title">Eval Expression.NET</h3>
								<hr class="m-y-md" />
								<h1>Evaluate, Compile and Execute dynamic C# code and expression at runtime</h1>
								<hr class="m-y-md" />
								<div class="lead">
									<a href="https://www.nuget.org/packages/Z.Expressions.Eval/" target="_blank" class="btn btn-success btn-lg btn-left" role="button"><span><i class="fa fa-cloud-download fa-2x"></i>&nbsp;<span>Download</span></span></a>
									<a href="https://github.com/zzzprojects/Eval-Expression.NET" target="_blank" class="btn btn-primary btn-lg btn-right" role="button"><span><i class="fa fa-github fa-2x"></i>&nbsp;<span>GitHub</span></span></a>
									<p class="text-muted">* FREE Version limited to 50 characters</p>		
								</div>
							</div>
						</div>
					</div>
					<div class="col-lg-6">
						<div class="card">
							<div class="card-block card-code">
{% highlight csharp %}
// From simple expression...
int result = Eval.Execute<int>("X + Y", new { X = 1, Y = 2})

// To complex code.
int result = Eval.Execute<int>(@"
	var list = new List<int>() { 1..100 };
	var filter = list.Where(x => x < 3);
	return result.Sum(x => x);");
	
// Support full C# Syntax including:
// - Anonymous Type
// - Extension Methods
// - Generic Type
{% endhighlight %}	
							</div>
						</div>
					</div>
				</div>
			</div>
		</header>
		
		<!-- featured !-->
		<div id="featured">
			<div class="container">
			
				<!-- C# Eval Function like JavaScript !-->
				<h2>C# Eval Function like JavaScript</h2>
				<div class="row">
					<div class="col-lg-5">
						<p class="featured-tagline">Use <span class="text-font-red">flexibility</span> of an Eval function in C# to build great dynamic application. C# developer doesn't have any more to be jealous of JavaScript Eval!</p>
						<ul class="featured-list-sm">
							<li>Anonymous Type</li>
							<li>Extension Methods</li>
							<li>Generic Type</li>
							<li>Lambda Expression</li>
							<li>LINQ</li>
							<li>And more...</li>
						</ul>
					</div>
					<div class="col-lg-7">
{% highlight csharp %}
int result = Eval.Execute<int>(@"
var list = new List<int>() { 1, 2, 3, 4, 5 };
return list.Where(x => x > X).Take(Y).Count();
{% endhighlight %}
					</div>
				</div>
			</div>
		</div>
		
		<!-- testimonials !-->
		<div id="testimonials">
			<div class="container">
				<h2>Amazing <span class="text-bold-red">performance</span>, outstanding <span class="text-bold-red">support</span>!</h2>
				<ul>
					<li>- "We were very, very pleased with the customer support. There was no question, problem or wish, that was not answered AND solved within days! We think that’s very unique!" Klemens Stelzmüller, <a href="http://www.beka-software.at/" target="_blank">Beka-software</a></li>
					<li>- "I’d definitely recommend it, as it is a great product with a great performance and reliability." Eric Rey, <a href="http://www.transturcarrental.com/" target="_blank">Transtur</a></li>
				</ul>
				<p><span class="text-bold-red">Share</span> your experience, we love to hear from you: <a href="mailto:info@zzzprojects.com">info@zzzprojects.com</a></p>
			</div>
		</div>
		
		<!-- features !-->
		<div id="feature">
			<div class="container">
				<!-- Evaluate dynamic arithmetic/math expression !-->
				<a id="evaluate-dynamic-arithmetic-math-expression" href="#"></a>
				<h2>Evaluate dynamic arithmetic/math expression</h2>
				<div class="row">
					<div class="col-lg-5">
						<p class="feature-tagline">Use a <span class="text-bold-red">complete</span> and <span class="text-bold-red">fast</span> compiler which support nearly everything.</p>
						<ul>
							<li>Operator Precedence</li>
							<li>Parenthesis</li>
							<li>Pow Operator (2^^3 = 8)</li>
						</ul>
					</div>
					<div class="col-lg-7">
{% highlight csharp %}
// Anonymous Type
int result = Eval.Execute<int>("X + Y", new { X = 1, Y = 2} );

// Class Member
dynamic expandoObject = new ExpandoObject();
expandoObject.X = 1;
expandoObject.Y = 2;
int result = Eval.Execute<int>("X + Y", expandoObject);

// Dictionary Key
var values = new Dictionary<string, object>() { {"X", 1}, {"Y", 2} };
int result = Eval.Execute<int>("X + Y", values);

// Argument Position
int result = Eval.Execute<int>("{0} + {1}", 1, 2);
{% endhighlight %}
					</div>
				</div>

				<hr class="m-y-md" />
				
				<!-- Execute dynamic string code !-->
				<a id="execute-dynamic-string-code" href="#"></a>
				<h2>Execute dynamic string code</h2>
				<div class="row">
					<div class="col-lg-5">
						<p class="feature-tagline">Improve your applications <span class="text-bold-red">flexibility</span> by executing code using the same C# Syntax.</p>
						<ul>
							<li>Evaluate stored formula</li>
							<li>Perform LINQ operations with string</li>
						</ul>
					</div>
					<div class="col-lg-7">
{% highlight csharp %}
int result = Eval.Execute<int>(@"
var list = new List<int>() { 1, 2, 3, 4, 5 };
return list.Where(x => x > X).Take(Y).Count();
{% endhighlight %}	
					</div>
				</div>

				<hr class="m-y-md" />
				
				<!-- Compile fast property getter/setter !-->
				<a id="compile-fast-property-getter-setter" href="#"></a>
				<h2>Compile fast property getter/setter</h2>
				<div class="row">
					<div class="col-lg-5">
						<p class="feature-tagline">Improve your code <span class="text-bold-red">readability</span> and <span class="text-bold-red">maintainability</span> with an easy-to-use and easy-to-understand API.</p>
						<ul>
							<li>Access internal and private property</li>
							<li>Avoid using slow reflection</li>
							<li>Avoid making complex lambda expression</li>
						</ul>						
					</div>
					<div class="col-lg-7">
{% highlight csharp %}
var customer = new Customer() { Name = "ZZZ" };

var nameGetter = Eval.Compile<Func<Customer, string>>("x.Name", "x");
var name = nameGetter(customer);
{% endhighlight %}	
					</div>
				</div>	
			</div>
		</div>
		
		<!-- support !-->
		<a id="supports" href="#"></a>
		<div id="support">
			<div class="container">
				<h2>Test our outstanding Support</h2>
				<h3>We usually answer within the next business day, hour, or minutes!</h3>
				<div class="row">
					<hr class="hidden-sm-up" />
					<div class="col-sm-6 col-lg-3">
						<div class="card">
							<div class="card-block">
								<h4 class="card-title">Contact Us</h4>
							</div>
							<a href="mailto:info@zzzprojects.com"><i class="fa fa-users fa-5x"></i></a>
							<div class="card-block">
								<p class="card-text">Email our team for any type of questions. We love to hear from you!</p>
								<a href="mailto:info@zzzprojects.com">info@zzzprojects.com</a>
							</div>
						</div>
					</div>
					<hr class="hidden-sm-up" />
					<div class="col-sm-6 col-lg-3">
						<div class="card">
							<div class="card-block">
								<h4 class="card-title">Documentation</h4>
							</div>
							<a href="https://github.com/zzzprojects/Eval-Expression.NET/wiki" target="_blank"><i class="fa fa-folder-open fa-5x"></i></a>
							<div class="card-block">
								<p class="card-text">Consult our complete documentation to help you getting started.</p>
								<a href="https://github.com/zzzprojects/Eval-Expression.NET/wiki" target="_blank">Documentation</a>
							</div>
						</div>
					</div>
					<hr class="hidden-sm-up" />
					<div class="col-sm-6 col-lg-3">
						<div class="card">
							<div class="card-block">
								<h4 class="card-title">Forum</h4>
							</div>
							<a href="https://github.com/zzzprojects/Eval-Expression.NET/issues" target="_blank"><i class="fa fa-weixin fa-5x"></i></a>
							<div class="card-block">
								<p class="card-text">Visit the forum to propose new features or to discuss about the library.</p>
								<a href="https://github.com/zzzprojects/Eval-Expression.NET/issues" target="_blank">Forum</a>
							</div>
						</div>
					</div>
					<hr class="hidden-sm-up" />
					<div class="col-sm-6 col-lg-3">
						<div class="card">
							<div class="card-block">
								<h4 class="card-title">Open Source</h4>
							</div>
							<a href="https://github.com/zzzprojects/Eval-Expression.NET" target="_blank"><i class="fa fa-github fa-5x"></i></a>
							<div class="card-block">
								<p class="card-text">Access the source of the library you're using to understand better its logic.</p>
								<a href="https://github.com/zzzprojects/Eval-Expression.NET" target="_blank">GitHub</a>
							</div>
						</div>
					</div>
				</div>
			</div>
		</div>
		
		<!-- pricing !-->
		<a id="pro" href="#"></a>
		<div id="pricing">
			<div class="container">
				<div class="row">
					<div class="col-lg-6">
						<h2>Pricing</h2>
						<hr class="m-y-md" />
						<p class="pricing-tagline">Use a well-coded and well-tested compiler to evaluate and execute your dynamic code and expressions.</p>
						<ul>
							<li>Add flexibility to your application</li>
							<li>Increase readability over reflection/expression</li>
							<li>Reduce development cost and time with a working library</li>
						</ul>
						<p class="pricing-tagline">C# developer are waited so long to get an Eval function, it's now possible and easy to make incredible dynamic library.</p>
						<hr class="m-y-md" />
						<p class="pricing-tagline">Want to evaluate C# code directly in SQL Server? <a href="http://eval-sql.net/">Eval-SQL.NET</a></p>
						<hr class="m-y-md" />
						<p>Every month, a <a href="https://www.nuget.org/packages/Z.Expressions.Eval/" target="_blank">FREE trial</a> of the PRO version is available to let you evaluate all its features without limitations.</p>						
					</div>
					<div class="col-lg-6">
						<table class="table table-hover table-bordered">
							<thead class="thead-inverse">
								<tr>
									<th></th>
									<th>FREE</th>
									<th>PRO</th>
								</tr>
							</thead>
							<tbody>
								<tr>
									<th>Maximum Characters</th>
									<td>50</td>
									<td>Unlimited</td>
								</tr>
								<tr>
									<th>Commercial License</th>
									<td><i class="fa fa-times fa-2x"></i></td>
									<td><i class="fa fa-check-square-o fa-2x"></i></td>
								</tr>
								<tr>
									<th>Royalty-Free</th>
									<td><i class="fa fa-times fa-2x"></i></td>
									<td><i class="fa fa-check-square-o fa-2x"></i></td>
								</tr>
								<tr>
									<th>Support & Upgrades (1 year)</th>
									<td><i class="fa fa-times fa-2x"></i></td>
									<td><i class="fa fa-check-square-o fa-2x"></i></td>
								</tr>
							</tbody>
						</table>
						
						<form action="https://www.paypal.com/cgi-bin/webscr" method="post" target="_top" onsubmit="return purchase_validate()">
							<input type="hidden" name="cmd" value="_s-xclick">
							<input type="hidden" name="hosted_button_id" value="PW79CTHBQFBZC">
							<input type="hidden" name="currency_code" value="USD">
							<fieldset class="form-group">
								<input type="hidden" name="on0" value="Seats">
								<select name="os0" class="form-control">
									<option value="1 seat">Eval Expression.NET $599 (1 seat)</option>
									<option value="2-4 seats" selected>Eval Expression.NET $799 (2-4 seats)</option>
									<option value="5-9 seats">Eval Expression.NET $999 (5-9 seats)</option>
									<option value="10-14 seats">Eval Expression.NET $1199 (10-14 seats)</option>
									<option value="15-19 seats">Eval Expression.NET $1399 (15-19 seats)</option>
								</select> 
							</fieldset>
							<div class="checkbox">
								<label>
									<input id="agree_agreement" type="checkbox">I have read and agree to the <a href="http://www.zzzprojects.com/license-agreement/" target="_blank">License Agreement</a>.
								</label>
							</div>
							<button type="submit" class="btn btn-success btn-lg"><span><i class="fa fa-shopping-cart"></i>&nbsp;<span>BUY NOW</span></span></button>
							<div><br />* Contact us for invoice or payment method alternative.</div>
						</form>	
					</div>
				</div>
			</div>
			
			<!-- validation !-->
			<div id="error_validation" class="modal fade" tabindex="-1" role="dialog" aria-labelledby="modal_agreement" aria-hidden="true">
				<div class="modal-dialog" role="document">
					<div class="modal-content">
						<div class="modal-header">
							<h4 class="modal-title" id="modal_agreement">License Agreement</h4>
						</div>
						<div class="modal-body bg-danger">
							You must read and agree to the License Agreement.
						</div>
						<div class="modal-footer">
							<button type="button" class="btn btn-secondary" data-dismiss="modal">Close</button>
						</div>
					</div>
				</div>
			</div>
		</div>

		<!-- other product !-->
		<div id="product">
			<div class="container">
				<div class="row">
					<div class="col-lg-3">
						<h3>Entity Framework</h3>
						<ul>
							<li><a href="http://entityframework-extensions.net/" target="_blank">Entity Framework Extensions</a></li>
							<li><a href="http://entityframework-plus.net/" target="_blank">Entity Framework Plus (EF+)</a></li>
						</ul>
					</div>
					<div class="col-lg-3">
						<h3>Bulk Operations</h3>
						<ul>
							<li><a href="http://bulk-operations.net/" target="_blank">Bulk Operations</a></li>
						</ul>
					</div>
					<div class="col-lg-3">
						<h3>Expression Evaluator</h3>
						<ul>
							<li><a href="http://eval-sql.net/" target="_blank">Eval SQL.NET</a></li>
							<li><a href="http://eval-expression.net/" target="_blank">Eval Expression.NET</a></li>
						</ul>
					</div>
					<div class="col-lg-3">
						<h3>Others</h3>
						<ul>
							<li><a href="https://github.com/zzzprojects/Z.ExtensionMethods" target="_blank">Extension Methods</a></li>
							<li><a href="https://github.com/zzzprojects/LINQ-Async" target="_blank">LINQ Async</a></li>
						</ul>
					</div>
				</div>
			</div>		
		</div>
		
		<!-- footer !-->
		<footer>
			<div class="container text-center-md-down">
				<div class="row">
					<div class="col-lg-6">
						Copyright © <a href="http://www.zzzprojects.com/" target="_blank" class="text-bold">ZZZ Projects Inc.</a> 2014 - 2016
						<div class="hidden-lg-up"></div>
						All rights reserved
					</div>
					<hr class="hidden-lg-up" />
					<div class="col-lg-6 text-right-lg-up social">
						<a href="https://www.facebook.com/zzzprojects" target="_blank"><i class="fa fa-facebook"></i></a>
						<a href="https://twitter.com/zzzprojects" target="_blank"><i class="fa fa-twitter"></i></a>
						<a href="https://plus.google.com/+Zzzprojects_NetSQL" target="_blank"><i class="fa fa-google-plus"></i></a>
						<a href="http://zzzprojects.us9.list-manage.com/subscribe?u=cecbc4775cf67bf1ff82018af&id=4765ffa5f8" target="_blank"><i class="fa fa-newspaper-o"></i></a>
					</div>
				</div>
			</div>
		</footer>

	<script type="text/javascript" src="https://ajax.googleapis.com/ajax/libs/jquery/2.1.4/jquery.min.js"></script>
	<script src="http://entityframework-plus.net/js/tether.min.js"></script>
	<script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0-alpha.2/js/bootstrap.min.js" integrity="sha384-vZ2WRJMwsjRMW/8U7i6PWi6AlO1L79snBrmgiDpgIWJ82z8eA5lenwvxbMV1PAh7" crossorigin="anonymous"></script>
	<script type="text/javascript">
	  (function(i,s,o,g,r,a,m){i['GoogleAnalyticsObject']=r;i[r]=i[r]||function(){
	  (i[r].q=i[r].q||[]).push(arguments)},i[r].l=1*new Date();a=s.createElement(o),
	  m=s.getElementsByTagName(o)[0];a.async=1;a.src=g;m.parentNode.insertBefore(a,m)
	  })(window,document,'script','//www.google-analytics.com/analytics.js','ga');

	  ga('create', 'UA-55584370-3', 'auto');
	  ga('send', 'pageview');
	  
	  function purchase_validate() {
		if($("#agree_agreement").prop('checked')) {
			return true;
		}
		
		$("#error_validation").modal('show')
		return false;
	  }
	</script>
	</body>
</html>
