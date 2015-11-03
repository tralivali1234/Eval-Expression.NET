---
layout: post
---

<html lang="en">
	<head>
		<meta charset="utf-8">
		<meta name="viewport" content="width=device-width, initial-scale=1">
		<meta http-equiv="x-ua-compatible" content="ie=edge">
		<meta name="description" content="Evaluate, Compile and Execute code and expression at runtime">
		<meta name="keywords" content="NET, CSharp, VB, Eval, Evaluate, Compile, Execute">
		<title>Evaluate, Compile and Execute code and expression at runtime</title>
		<link rel="stylesheet" type="text/css" href="https://cdn.rawgit.com/twbs/bootstrap/v4-dev/dist/css/bootstrap.min.css">
		<link rel="stylesheet" type="text/css" href="https://maxcdn.bootstrapcdn.com/font-awesome/4.4.0/css/font-awesome.min.css">
		<link rel="stylesheet" type="text/css" href="/css/github.css">
	</head>
	<body>
  
	<a id="download" href="#"></a>
	<a id="github" href="#"></a>
	<div id="top-header">
		<div class="container">
			<div class="row">
				<div class="col-sm-12 text-right">
					<a href="mailto:sales@zzzprojects.com"><i class="fa fa-envelope"></i>&nbsp;sales@zzzprojects.com</a>
					<a href="https://www.facebook.com/zzzprojects" target="_blank"><i class="fa fa-facebook"></i></a>
					<a href="https://twitter.com/zzzprojects" target="_blank"><i class="fa fa-twitter"></i></a>
					<a href="https://plus.google.com/+Zzzprojects_NetSQL/posts" target="_blank"><i class="fa fa-google-plus"></i></a>
					<a href="http://zzzprojects.us9.list-manage.com/subscribe?u=cecbc4775cf67bf1ff82018af&id=4765ffa5f8" target="_blank" class="hidden-sm-down"><i class="fa fa-newspaper-o"></i></a>
				</div>
			</div>
		</div>
	</div>
	<header>
		<div class="container">
			<div class="row">
				<div class="col-lg-6">
					<div class="jumbotron">
						<h1 class="display-3">Eval.NET</h1>
						<h3>Evaluate, Compile and Execute code and expression at runtime</h3>
						<hr class="m-y-md" />
						<div class="lead">
							<a href="https://www.nuget.org/packages/Z.Expressions.Eval/" class="btn btn-success btn-lg" role="button"><span><i class="fa fa-cloud-download fa-2x"></i>&nbsp;<span>Download</span></span></a>
							<a href="https://github.com/zzzprojects/Z.Expressions.Eval" class="btn btn-primary btn-lg" role="button"><span><i class="fa fa-github fa-2x"></i>&nbsp;<span>GitHub</span></span></a>
							<p class="text-muted">* FREE up to 50 characters</p>
							<p style="display: none">
								<a href="https://www.nuget.org/packages/Z.Expressions.Eval/" target="_blank" alt="download nuget"><img src="https://img.shields.io/nuget/v/Z.Expressions.Eval.svg" /></a>
								<a href="https://www.nuget.org/packages/Z.Expressions.Eval/" target="_blank" alt="download nuget"><img src="https://img.shields.io/nuget/dt/Z.Expressions.Eval.svg" /></a>
							</p>							
						</div>
					</div>
				</div>
				<div class="col-lg-6">
					<div id="carousel" class="carousel slide" data-ride="carousel" data-interval="2000">
						<ol class="carousel-indicators">
							<li data-target="#carousel" data-slide-to="0" class="active"></li>
							<li data-target="#carousel" data-slide-to="1" class=""></li>
							<li data-target="#carousel" data-slide-to="2" class=""></li>
						</ol>
						<div class="carousel-inner" role="listbox">
							<div class="carousel-item active">
								<div class="carousel-item-container">
{% highlight csharp %}
int result = Eval.Execute<int>("x + y", new { x = 1, y = 2})
{% endhighlight %}
								</div>
								<div class="carousel-caption">
									<h3>From simple expression...</h3>
								</div>
							</div>
							<div class="carousel-item">
								<div class="carousel-item-container">
{% highlight csharp %}
int result = Eval.Execute<int>(@"x + y", new { x = 1, y = 2})
{% endhighlight %}
								</div>
								<div class="carousel-caption">
									<h3>to complex code...</h3>
								</div>
							</div>
							<div class="carousel-item">
								<div class="carousel-item-container">
{% highlight csharp %}
int result = Eval.Execute<int>(@"x + y", new { x = 1, y = 2})
{% endhighlight %}
								</div>
								<div class="carousel-caption">
									<h3>with an easy to use API</h3>
								</div>
							</div>
						</div>
					</div>
				</div>
			</div>
		</div>
	</header>
	
	<div id="feature">
		<div class="container">
			<div class="row">
				<div class="col-lg-6">
					<a id="execute" href="#"></a>
					<h2>Eval.Execute</h2>
					<hr class="m-y-md" />
					<p>Evaluate and execute a code or expression</p>
					<h3>Using Anonymous Class</h3>
{% highlight csharp %}
int result = Eval.Execute<int>("x + y", new { x = 1, y = 2})
{% endhighlight %}
					<h3>Using Ordinal Position</h3>
{% highlight csharp %}
int result = Eval.Execute<int>("{0} + {1}", x, y)
{% endhighlight %}
					<h3>Using Extension Methods</h3>
{% highlight csharp %}
string s = "x + y";
int result = s.Eval<int>(new { x = 1, y = 2 });
{% endhighlight %}
					<div class="text-center"><a class="btn btn-primary btn-lg" href="#" role="button">Learn More&nbsp;<i class="fa fa-hand-o-right"></i></a></div>
				</div>
				<div class="col-lg-6">
					<a id="compile" href="#"></a>
					<h2>Eval.Compile</h2>
					<hr class="m-y-md" />
					<p>Compile a code or expression and return a delegate to execute</p>
					<h3>Using custom Delegate</h3>
{% highlight csharp %}
Func<int> compiled = Eval.Compile<Func<int>>("x + y", new { x = 1, y = 2})
int result = compiled(1);
{% endhighlight %}
					<h3>Using Extension Methods</h3>
{% highlight csharp %}
string code = "x + y";
var compiled = code.Compile<Func<int, int>>("x", "y");
foreach(var item in list)
{
}
{% endhighlight %}
					<div class="text-center"><a class="btn btn-primary btn-lg" href="#" role="button">Learn More&nbsp;<i class="fa fa-hand-o-right"></i></a></div>
				</div>
			</div>
		</div>
	</div>
	
	<div id="pricing">
		<div class="container">
			<div class="row">
				<div class="col-lg-6">
					<h2>Pricing</h2>
					<p>Become a <span class="text-bold text-green">PRO</span> now and save time and money.</p>
					<p>Thousands of <span class="text-bold">development hours</span>, thousands of <span class="text-bold">unit test</span> to make Eval.NET the best and robust expression evaluator for .NET language.</p>
					<p>PRO License starting at $299</p>
					<p class="text-muted">Each additional developer seat at $100</p>
				</div>
				<div class="col-lg-6">
					<table class="table">
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
					
					<form>
						<fieldset class="form-group">
							<select class="form-control" id="exampleSelect1">
								<option>Eval.NET $299 (1 seat)</option>
								<option>Eval.NET $399 (2 seats)</option>
								<option>Eval.NET $499 (3 seats)</option>
								<option>Eval.NET $599 (4 seats)</option>
								<option>Eval.NET $699 (5-9 seats)</option>
								<option>Eval.NET $899 (10-14 seats)</option>
								<option>Eval.NET - 15+ seats - Contact Us</option>
							</select>
						</fieldset>
						<div class="checkbox">
							<label>
								<input type="checkbox">I have read and agree to the <a href="" target="http://www.zzzprojects.com/license-agreement/">License Agreement</a>.
							</label>
						</div>
						<a href="https://www.nuget.org/packages/Z.Expressions.Eval/" class="btn btn-success btn-lg" role="button"><span><i class="fa fa-shopping-cart"></i>&nbsp;<span>BUY NOW</span></span></a>
					</form>
					
				</div>
			</div>
		</div>
	</div>
	
	<a id="support" href="#"></a>
	<div id="support">
		<div class="container">
			<h2>Test our Outstanding Support</h2>
			<p>We usually answer within the next business day, hour, or minutes!</p>
			<div class="row">
				<hr class="hidden-sm-up" />
				<div class="col-sm-6 col-lg-3">
					<div class="card">
						<div class="card-block">
							<h4 class="card-title">Documentation</h4>
						</div>
						<a href="/docs/" target="_blank"><i class="fa fa-folder-open fa-5x"></i></a>
						<div class="card-block">
							<p class="card-text">Consult and print our complete documentation to help you get started</p>
							<a href="/docs/" target="_blank">Documentation</a>
						</div>
					</div>
				</div>
				<hr class="hidden-sm-up" />
				<div class="col-sm-6 col-lg-3">
					<div class="card">
						<div class="card-block">
							<h4 class="card-title">Contact Us</h4>
						</div>
						<a href="mailto:sales@zzzprojects.com"><i class="fa fa-users fa-5x"></i></a>
						<div class="card-block">
							<p class="card-text">Email our team for any type of questions</p>
							<a href="mailto:sales@zzzprojects.com">sales@zzzprojects.com</a>
						</div>
					</div>
				</div>
				<hr class="hidden-sm-up" />
				<div class="col-sm-6 col-lg-3">
					<div class="card">
						<div class="card-block">
							<h4 class="card-title">Forum</h4>
						</div>
						<a href="mailto:sales@zzzprojects.com"><i class="fa fa-weixin fa-5x"></i></a>
						<div class="card-block">
							<p class="card-text">Consult the forum to propose a new feature or to discuss about the library</p>
							<a href="https://zzzprojects.uservoice.com/forums/327759-eval-expression-net" target="_blank">Forum</a>
						</div>
					</div>
				</div>
				<hr class="hidden-sm-up" />
				<div class="col-sm-6 col-lg-3">
					<div class="card">
						<div class="card-block">
							<h4 class="card-title">Open Source</h4>
						</div>
						<a href="https://github.com/zzzprojects/Z.Expressions.Eval" target="_blank"><i class="fa fa-github fa-5x"></i></a>
						<div class="card-block">
							<p class="card-text">Look at the latest release notes to know what’s new with the version you are using</p>
							<a href="https://github.com/zzzprojects/Z.Expressions.Eval" target="_blank">GitHub</a>
						</div>
					</div>
				</div>
			</div>
		</div>
	</div>
	
	<footer>
		<div class="container">
			<div class="row">
				<div class="col-lg-6 text-center-md-down">
					Copyright © 2015 <a href="http://www.zzzprojects.com/" target="_blank">ZZZ Projects Inc.</a>
					<div class="hidden-lg-up"></div>All rights reserved
				</div>
				<hr class="hidden-lg-up" />
				<div class="col-lg-6 text-right text-center-md-down social">
					<a href="https://www.facebook.com/zzzprojects" target="_blank"><i class="fa fa-facebook"></i></a>
					<a href="https://twitter.com/zzzprojects" target="_blank"><i class="fa fa-twitter"></i></a>
					<a href="https://plus.google.com/+Zzzprojects_NetSQL/posts" target="_blank"><i class="fa fa-google-plus"></i></a>
					<a href="http://zzzprojects.us9.list-manage.com/subscribe?u=cecbc4775cf67bf1ff82018af&id=4765ffa5f8" target="_blank"><i class="fa fa-newspaper-o"></i></a>
				</div>
			</div>
		</div>
	</footer>

    <script type="text/javascript" src="https://ajax.googleapis.com/ajax/libs/jquery/2.1.4/jquery.min.js"></script>
    <script type="text/javascript" src="https://cdn.rawgit.com/twbs/bootstrap/v4-dev/dist/js/bootstrap.min.js"></script>
	<script type="text/javascript">
	  (function(i,s,o,g,r,a,m){i['GoogleAnalyticsObject']=r;i[r]=i[r]||function(){
	  (i[r].q=i[r].q||[]).push(arguments)},i[r].l=1*new Date();a=s.createElement(o),
	  m=s.getElementsByTagName(o)[0];a.async=1;a.src=g;m.parentNode.insertBefore(a,m)
	  })(window,document,'script','//www.google-analytics.com/analytics.js','ga');

	  ga('create', 'UA-55584370-3', 'auto');
	  ga('send', 'pageview');
	</script>
  </body>
</html>

<style>
/* general */
* {
	 font-family: "Bitter",Georgia,"Times New Roman",serif;
}
.text-bold {
	font-weight: 700;
}
.text-green {
	color: rgb(68, 157, 68);
}
@media (max-width: 61em) {
  .text-center-md-down {
    text-align: center;
  }
}

/* section general */
#top-header {
    background: -moz-linear-gradient(top, #111, #222);
    background: -webkit-linear-gradient(top, #111, #222);
    background: -ms-linear-gradient(top, #111, #222);
    background: -o-linear-gradient(top, #111, #222);
    background: linear-gradient(top, #111, #222);
	border-bottom: 1px solid #111;
	font-size: 14px;
	padding-top: 5px;
	padding-bottom: 5px;
}
header {
	background: -moz-linear-gradient(top, #222, #333);
    background: -webkit-linear-gradient(top, #222, #333);
    background: -ms-linear-gradient(top, #222, #333);
    background: -o-linear-gradient(top, #222, #333);
    background: linear-gradient(top, #222, #333);
	border-bottom: 1px solid #111;
	border-top: 1px solid #333;
}
#feature {
    background: -moz-linear-gradient(top, #ddd, #f2f2f2);
    background: -webkit-linear-gradient(top, #ddd, #f2f2f2);
    background: -ms-linear-gradient(top, #ddd, #f2f2f2);
    background: -o-linear-gradient(top, #ddd, #f2f2f2);
    background: linear-gradient(top, #ddd, #f2f2f2);
    border-top: 1px solid #eee;
	padding-bottom: 60px;
}
#pricing {
	padding-top: 60px;
	padding-bottom: 60px;
}
#support {
	background: -moz-linear-gradient(top, #eee, #bbb);
    background: -webkit-linear-gradient(top, #eee, #bbb);
    background: -ms-linear-gradient(top, #eee, #bbb);
    background: -o-linear-gradient(top, #eee, #bbb);
    background: linear-gradient(top, #eee, #bbb);
	padding-top: 60px;
	padding-bottom: 60px;
	border-bottom: 1px solid #aaa;
}
footer {
	background: -moz-linear-gradient(top, #333, #222);
    background: -webkit-linear-gradient(top, #333, #222);
    background: -ms-linear-gradient(top, #333, #222);
    background: -o-linear-gradient(top, #333, #222);
    background: linear-gradient(top, #333, #222);
	border-top: 1px solid #444;
	color: #666;
	padding-top: 5px;
	padding-bottom: 5px;
}

/* top-header */
#top-header a {
	color: #f1f1f1;
	padding-left: 10px;
	padding-right: 10px;
	text-decoration: none;
} 
#top-header a:hover {
	opacity: 0.7;
    transition: all 0.4s ease-in-out 0s;
}

/* header */
header .jumbotron {
	background-color: transparent;
	color: #f1f1f1;
	margin-bottom: 0px;
	padding-top: 20px;
}
header .jumbotron hr {
	border-color: initial;
}
header .jumbotron .lead .btn {
	width: 175px;
	margin-right: 20px;
}
header .jumbotron .lead .btn span {
	display: inline-block;
	height: 40px;
}
header .jumbotron .lead .btn span span {
	vertical-align : middle;
}

header .jumbotron .lead .text-muted {
	font-size: 14px;
}
header #carousel {
	background-color: #f1f1f1;
	border: 2px solid #444;
	color: #000;
	margin-top: 64px;
	margin-bottom: 64px;
}
header .carousel-item {
	height:300px;
}
header .carousel-caption,
header .carousel-control {
	color: #000;
	text-shadow: none;
}
header .carousel-indicators li {
	border: 1px solid #000;
}
header .carousel-indicators .active {
	background-color: #000;
}
header #carousel .highlight,
header #carousel .highlight pre {
	background-color: transparent;
	border: none;
}
@media (max-width: 33em) {
	header .jumbotron h1.display-2{
		font-size: 4.5rem;
	}
	header .jumbotron .lead .btn {
		margin-bottom: 20px;
	}
}
@media (max-width: 61em) {
  header #carousel {
    margin-top: 0px;
  }
}

/* feature */
#feature h2 {
	font-size: 42px;
	letter-spacing: 4px;
	padding-top: 60px;
	text-align: center;
}
#feature h3 {
	letter-spacing: 2px;
	font-size: 16px;
	text-decoration: underline;
}
#feature .btn {
	margin-top: 40px;
}

@media (min-width: 62em) {
	#feature .row .col-lg-6:first-child {
		padding-right: 45px;
	}
	#feature .row .col-lg-6:last-child {
		padding-left: 45px;
	}
}


/* pricing */
#pricing h2 {
	padding-bottom: 20px;
}
#pricing .table thead th {
	text-align: center;
}
#pricing .table td {
	text-align: center;
}
#pricing .fa-times {
	color: #c9302c;
}
#pricing .fa-check-square-o {
	color: rgb(68, 157, 68);
}

/* support */
#support {
	text-align: center;
}
#support h2 {
	padding-bottom: 20px;
}
#support .card {
	border: 0.0625rem solid #ccc;
}
#support .card-text {
	min-height: 75px;
}
#support i {
	color: #0275d8;
	padding-bottom: 20px;
}

/* footer */
footer a {
	color: #666;
	text-decoration: none;
}
footer a:hover {
	color: #666;
	opacity: 0.7;
    transition: all 0.4s ease-in-out 0s;
	text-decoration: none;
}
footer .social a {
	font-size: 24px;
	padding-left: 10px;
	padding-right: 10px;
}
@media (max-width: 61em) {
  footer {
	padding: 20px 0;
  }
}
</style>
