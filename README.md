[![Build Status](https://travis-ci.org/tresorit/ZeroKit-Web-SDK.svg?branch=master)](https://travis-ci.org/tresorit/ZeroKit-Web-SDK)
# ZeroKit Web SDK
This SDK exposes methods to help implement secure authentication and end-to-end encryption in your web application.
It makes use of iframes loaded from a tenant server. These iframes deal with password inputs and run all the code that
handles encryption keys, protecting you from accindental leaks and most XSS attacks.

The ZeroKit SDK for Web is currently under development and is accessible as a preview. We continuously improve the SDK and fix bugs.

The project was written in typescript and is available compiled to javascript on the tenant server.
Loading from there is the recommended way of use.

## Usage
The sdk compiles into a bundle, which inserts the zkit_sdk object into the global namespace.
Calling the setup method of this object initializes the sdk and it is ready to use.
This should be done during the pageload optionally along with a whoAmI call that will initialize the lazy loading.
From there on your application can use the exposed login register etc. methods.

For a detailed documentation you should see the documentation available for download on the management portal.

## Requirements
First, to use the SDK you need a tenant server (basically a subscription to ZeroKit).
You can get one for free at the ZeroKit [tenant management portal](https://manage.tresorit.io),
where you can also find a detailed documantation and sample apps for many platforms. You can also get the relevant
example from [GitHub](https://github.com/tresorit/ZeroKit-simple-example).
