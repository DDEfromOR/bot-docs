---
title: Designing for the first interaction | Microsoft Docs
description: Learn best practices for designing for the first interaction between user and bot. 
keywords: Bot Framework, Bot design, core principles
author: matvelloso
manager: rstand

# the ms.topic should be the section of the IA that the article is in, with the suffix -article. Some examples:
# get-started article, sdk-reference-article
ms.topic: design-ui-and-ux-article

ms.prod: botframework

# The ms.service should be the Bot Framework technology area covered by the article, e.g., Bot Builder, LUIS, Azure Bot Service
ms.service: Bot Builder

# Date the article was updated
ms.date: 02/16/2017

# Alias of the document reviewer. Change to the appropriate person.
ms.reviewer: rstand

# Include the following line commented out
#ROBOTS: Index
---
# Designing for the first interaction

## First impressions matter

The first interaction between the user and bot is critical to the user experience. 
When designing your bot, keep in mind that there is more to that first message than just saying "hi." 
When you build an app, you design the first screen to provide important navigation cues: 
users should intuitively understand things such as 
where the menu is located and how it works, where to go for help, what the privacy policy is, and so on.
When you design a bot, the user's first interaction with the bot should provide that same type of information. 
In other words, just saying "hi" won’t be enough.

## Language versus menus 

Consider the following two designs:

Design 1

![bot](media/designing-bots/core/hello1.png)


Design 2

![bot](media/designing-bots/core/hello2.png)

Starting the bot with an open-ended question such as "How can I help you?" is usually a bad idea. 
If your bot has a hundred different things it can do, chances are users won’t be able to guess the vast majority of them. 
Your bot didn’t tell them what it can do, so how can they possibly know?

Menus provide a simple solution to that problem. 
First, by listing the available options, your bot is conveying its capabilities to the user. 
Second, menus spare the user from having to type too much -- they can simply click, which is always faster than typing. 
Finally, the use of menus can significantly simplify your natural language models (by narrowing the scope of input that the bot could receive from the user). 

> [!TIP]
> Menus are a valuable tool when designing bots for a great user experience. 
> Don’t dismiss them as not being “smart enough”.

> [!NOTE]
> You might choose design your bot to use menus while still supporting free form input. 
> That is, if a user responds to the initial menu by typing rather than by selecting a menu option, your bot could attempt to parse the user's text input. 

## Other considerations

In addition to providing an intuitive and easily navigated first interaction, 
a well-designed bot provides the user with access to information about its privacy policy and terms of use. 

> [!TIP]
> If your bot collects personal data from the user, it's important to convey that and to describe what will be done with the data.

## Next steps

Now that you're familiar with some basic principles for designing the first interaction between user and bot, 
learn more about [designing the flow of conversation](bot-framework-design-core-dialogs.md).