---
title: "Part 3 - Setting Up our RDS Database"
date: 2018-07-24T21:19:40+01:00
draft: true
desc: "In this tutorial, we are going to be creating an RDS database instance which will store things such as our blog posts."
author: "Elliot Forbes"
tags: ["vuejs", "javascript"]
image: "vuejs.png"
weight: 3
series: [ "vuejsawsblog" ]
twitter: "https://twitter.com/Elliot_F"
---

## Introduction

Welcome back to part 3 of my course on building a blog with Vue.JS on AWS. In this part of the course, we are going to be setting up an RDS instance which will store all of our blog's articles and posts. 

Once we have our database instance set up and our schema defined, we can then move on to building Lambda functions that will query this database and return the results to our frontend.

These Functions will do as follows:

* Return all blog posts - This will return a paginated JSON list of all of the blog posts within our database
* Return single blog post - This will return a JSON object containing one particular blog post
* Create a blog post - This will allow authenticated users of the site to create new blog posts and upload them to our site
* Update a blog post - This will allow authenticated users who created a post the ability to update their posts
* Delete a blog post - this will allow authenticated users the ability to delete a blog post

This represents a fairly standard set of endpoints that will allow give us *most* of the basic functionality our blog will need in order to work.

## Amazon Aurora

For the purposes of this tutorial series, we'll be creating an Amazon Aurora DB instance which will be MySQL 5.6 compatible. This will cost roughly $30/month to run in a single-node configuration.

Now, the lower cost option for spinning up a database could be to run an EC2 t2.micro instance and run MySQL on top of that. However, you then have to worry about things such as resiliency, automatic failover, monitoring and more. By buying into these managed services, we effectively trade our money for peace-of-mind. 

If our blog happens to go viral for any reason, Amazon Aurora will be able to handle the massive surge in traffic.

## Under Construction



## Conclusion



