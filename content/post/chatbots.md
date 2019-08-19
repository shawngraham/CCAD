---
title: "Why Chatbots?"
date: "2019-08-19"
tags: ["chatbots","engagement","mirror"]
---

I've made a number of twitterbots, and one or two facebook messenger bots. In my [lesson on making twitterbots for the Programming Historian](https://programminghistorian.org/en/lessons/intro-to-twitterbots) I wrote:

> _I believe also that there is space in digital history and the digital humanities more generally for creative, expressive, artistic work. I belive that there is space for programming historians to use the affordances of digital media to create things that could not otherwise exist to move us, to inspire us, to challenge us. There is room for satire; there is room for comment. With Mark Sample, I believe that there is a need for ‘[bots of conviction](https://medium.com/@samplereality/a-protest-bot-is-a-bot-so-specific-you-cant-mistake-it-for-bullshit-90fe10b7fbaa)’._

Angeliki Tzouganatou reviews some heritage bots in a recent edition of [_Advances in Archaeological Practice_](https://www.cambridge.org/core/journals/advances-in-archaeological-practice/article/can-heritage-bots-thrive-toward-future-engagement-in-cultural-heritage/0B1894A640F167BC25CCE47FB82840E8/core-reader) and ultimately concludes that the full potential of bots for understanding the past is not being met:

> _The majority of those in development and currently available online right now are closed and didactic in nature. The next step is to craft them into genuine mechanisms of chat, inviting users to actively interact and participate in the conversational experience_

Sara Perry's team has been trying a slightly different approach, and is using bots as a way of prompting reflective discussion (amongst the humans). Indeed, in Roussou et al 2019 they go so far as to call the bot they've designed a 'provocation', drawing on Sample's 'bots of conviction' framework.

Their bot is a rules-based bot, but allows for an emergent dialogue amongst the humans.

![](https://deliveryimages.acm.org/10.1145/3310000/3300857/images/chi2019-627-fig2.jpg)

Allison Parrish has a notebook demonstrating a chatbot trained on the Cornell Movie Dialogue database, which then uses semantic similarity to pick appropriate responses to the user's input according to how similar that input is to the query part of dialogue pairs in the database ([more here](notebooks/semantic-similarity-chatbot/)).

At present, I want to move beyond these kind of rules-based or replacement-grammar type bots towards a generative bot more along the lines of what Parrish has done. I want to train a chatbot on archaeological knowledge so that it can be queried _but the responses will be generated on the spot_. That is, I want it to understand something of the structured language of archaeology, and from that structure, divine new insights from its training.

While it's not quite the state-of-the-art for neural network approaches to text, Karpathy's [the unreasonable effectiveness of recurrent neural networks](https://karpathy.github.io/2015/05/21/rnn-effectiveness/) gives us a vector for considering one way of creating a bot that might do something along those lines. But what would the result actually _tell_ us about the archaeology on which it is trained? My instinct is that what would emerge from such a dialogue would be a kind of mirror effect, a bit like the original [ELIZA](https://www.masswerk.at/elizabot/eliza.html) that enables us to pick apart ourselves apart.

And so I am currently playing with [https://github.com/pender/chatbot-rnn](https://github.com/pender/chatbot-rnn) which builds from Karpathy's work but also includes a feature called 'relevance':

> _Two models are run in parallel: the primary model and the mask model. The mask model is scaled by the relevance value, and then the probabilities of the primary model are combined according to equation 9 in Li, Jiwei, et al. "A diversity-promoting objective function for neural conversation models." arXiv preprint arXiv:1510.03055 (2015)._

Stay tuned.

[Video of chatbot in action](https://screencast-o-matic.com/watch/cqjbF3tfNz)

Karpathy, Andrej. (2015). The Unreasonable Effectiveness of Recurrent Neural Networks. https://karpathy.github.io/2015/05/21/rnn-effectiveness/

Roussou, M., Perry, S., Katifori, A., Vassos, S., Tzouganatou, A., McKinney, S. (2019) Transformation through Provocation? Designing a ‘Bot of Conviction’ to Challenge Conceptions and Evoke Critical Reflection. In CHI ’19 Proceedings of the 2019 CHI Conference on Human Factors in Computing Systems, Glasgow, Scotland, 4-9 May. New York: ACM. [Paper No. 627](https://dl.acm.org/citation.cfm?doid=3290605.3300857).

Tzouganatou, A. (2018). Can Heritage Bots Thrive? Toward Future Engagement in Cultural Heritage. Advances in Archaeological Practice, 6(4), 377-383. doi:10.1017/aap.2018.32
