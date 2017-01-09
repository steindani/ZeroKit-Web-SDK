[![Build Status](https://travis-ci.org/tresorit/ZeroKit-Web-SDK.svg?branch=master)](https://travis-ci.org/tresorit/ZeroKit-Web-SDK)
# ZeroKit Web SDK
This SDK helps you implement **secure authentication** and **end-to-end encryption** in your web application, utilizing only iframes loaded from a tenant server. These iframes deal with password inputs and run all the code handling encryption keys, protecting you from accindental leaks and most XSS attacks.

![](https://raw.githubusercontent.com/wiki/tresorit/ZeroKit-Web-SDK/images/zerokit_pattern.png)

The ZeroKit SDK for Web is currently under development and accessible as a preview. We continuously improve the SDK and fix bugs. The project is developed in TypeScript and available as a compiled JavaScript file from the tenant server. Loading from there is the recommended way of use.

## Usage
The SDK compiles into a bundle, inserting the zkit_sdk object into the global namespace. Calling the `setup` method of this object initializes the SDK. This should be done during the pageload – optionally along with a `whoAmI` call that initializes the lazy loading. After that your application can use the exposed `login`, `register`, and alike methods.

For a detailed documentation, please visit the [tenant management portal](https://manage.tresorit.io).

## Requirements
First, to use the SDK you need a tenant server (basically a subscription to ZeroKit). You can get one for free at the ZeroKit [tenant management portal](https://manage.tresorit.io), where you can also find a detailed documentation and sample apps for many platforms. You can also take a look at the relevant example at our [ZeroKit simple example GitHub repo](https://github.com/tresorit/ZeroKit-simple-example).
