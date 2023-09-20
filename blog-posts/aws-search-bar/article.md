---
published: true
title: 'Search your AWS resources blazingly fast ⚡️'
cover_image: 'https://raw.githubusercontent.com/ChloeMouret/kumo-articles/master/blog-posts/aws-search-bar/assets/cover.png'
description: 'Use the AWS search bar to find directly any of your resources at a glance'
tags: aws, tutorial, serverless, webdev
series:
canonical_url:
---

## It's so annoying to find your resources in AWS ...

I don't know about you, but I find it really annoying to find my resources in AWS. I always have to click through the different services and then search for my resource.

If I need to find my `myLambda` function, I have to click on the `Lambda` service, then click on `Functions` and then search for my function.

![Find my lambda in Lambda service](./assets/find_lambda_in_lamdba_service.png 'Find my lambda in Lambda service')

In fact, there is a global search bar in the top left corner of the AWS console. But it's not really helpful. It only searches for services, not for resources. So if I search for `myLambda` in the search bar, I get a list of all the services that contain the word `myLambda`.

**🚀🚀 In this article, let me show you how to use this search bar to find your resources directly.🚀🚀**

## Use AWS Resource Explorer directly in the search bar

AWS Resource Explorer is a service that is used to efficiently search and discover your AWS resources across AWS Regions and accounts. It provides a single view of your resources and enables you to search and filter by resource type, region, tags, and other key attributes. You can also view resource details, including resource configuration, metadata, and related resources.

The best thing about it is that you can combine with the search bar and **it is free** !! 🤯

### Enable AWS Resource Explorer

To enable AWS Resource Explorer, you need to go to the [AWS Resource Explorer console](https://resource-explorer.console.aws.amazon.com/resource-explorer/home#/home) and click on `Turn on Resource Explorer`.

Then, you just have a small form to fill in. You just have to specify the Aggregator Index Region, a quick rule of thumb is to choose the region where you have the most resources.

![Turn on Resource Explorer](./assets/tuto_step3.png 'Turn on Resource Explorer')

Then click on `Turn on Resource Explorer` and you are done! 🎉 You will have to wait a few minutes for the service to be index all your resources in the background.

### Use AWS Resource Explorer in the search bar

From now on, it is so easy, just type the name of your resource in the search bar, scroll a little bit if needed and you will find your resource that match your input.

![Use AWS Resource Explorer in the search bar](./assets/tuto_step4.png 'Use AWS Resource Explorer in the search bar')

What is so powerful with that is that you can find associated resources like log groups and IAM roles.

### Last trick 🌟

Filter only your resources in the search bar by typing `/resources` before your resource name. This will filter only your resources and not the AWS services.

![Quick trick for your AWS search bar](./assets/trick.png 'Quick trick for your AWS search bar')

Also, if you want to be blazingly faster, you can use `OPT + S` for Mac or `ALT + S` for Windows to focus directly on the search bar.

{% cta https://twitter.com/ChloeMrt1 %} Follow me on twitter 🚀 {% endcta %}
