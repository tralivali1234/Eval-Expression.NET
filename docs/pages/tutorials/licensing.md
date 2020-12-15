---
layout: default
title: Licensing
permalink: licensing
---

{% include template-h1.html %}

## Evaluation Period
You can evaluate our library for several months before purchasing it.

The trial period stops at the end of the month. When you receive a license expiration error, download the latest version which will automatically extend your trial period.

You can also purchase the library [here](http://eval-expression.net/#pro)

Upon purchase, you will receive a license name and a license key.

## Setup License from config file
The license name and key can be added directly in the app.config or web.config file in the appSettings section.

{% include template-example.html %} 
{% highlight csharp %}
<appSettings>
	<add key="Z_Expressions_Eval_LicenseName" value="[licenseName]"/>
	<add key="Z_Expressions_Eval_LicenseKey" value="[licenseKey]"/>
</appSettings>
{% endhighlight %}

## Setup License from code
You can also set the license name and key directly in the code.

{% include template-example.html %} 
{% highlight csharp %}
// using Z.Expressions; // Don't forget to include this.

string licenseName = //... PRO license name
string licenseKey = //... PRO license key

EvalManager.AddLicense(licenseName, licenseKey);
{% endhighlight %}

### Recommendation
- Use the config file to store your license name and license key.
- **Web App:** Use Application_Start in global.asax to activate your license.
- **WinForm App:** Use the main thread method to activate your license.
- **Win Service:** Use the OnStart method to activate your license

> The AddLicense must be set before the first call to the library. Otherwise, you will start the evaluation period

## How can I check if my license is valid?
The validate method allow you to know whether your license is valid or not.
{% include template-example.html %} 
{% highlight csharp %}
string licenseErrorMessage;
if (!Z.Expressions.EvalManager.ValidateLicense(out licenseErrorMessage))
{
    throw new Exception(licenseErrorMessage);
}
{% endhighlight %}
