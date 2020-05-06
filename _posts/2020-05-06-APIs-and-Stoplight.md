---
layout: post
title:  "My journey with APIs and Stoplight"
date: 2020-05-06 13:45:00 +0300
tags: [blog, APIs, open source, Stoplight, prism]
author: Serafin
---

# My journey with APIs
So, lately I have been doing a lot of work related to APIs.
Agree on JSON responses, query parameters, etc.

And I try to follow the OpenAPI initiative as much as possible.
Take a look [here](https://www.openapis.org/).

The main point was to use a repository to hold the definitions and keep track of those changes.
And a tool to make it easier to build those API definitions.

And I found [Stoplight](https://stoplight.io/).

Two amazing products from these guys:

[Stoplight Studio](https://stoplight.io/studio/)

[Prism](https://stoplight.io/open-source/prism/)


**Studio** has a clean UI, and gives a nice and easy way to build APIs.

As it comes with a mockup server included, you can check the responses without leaving the tool, apply changes and keep building those definitions.
In addition, if you add format to your YAML definitions, the server will fake data.

You may also add "x-faker" tags to fully control such fake data.
More details [here](https://github.com/Marak/faker.js)

For example, as I wanted to fake some ids, you may add:
```yaml
id:
    type: string
    x-faker: random.uuid
```

These lines will add something like "c21beeaa-c81d-40f0-b8aa-abc1ce4c9d05".

If you want to control further the id length, for example:
```yaml
id:
    type: string
    format: uuid
    minLength: 5
    maxLength: 8
```

The result: "1bc0236c".

And, as commented, everything under a repository, so later I can pull the latest and update the prism server configuration so that the tools consuming those APIs get fake data every time.

Keep you posted and enjoy!