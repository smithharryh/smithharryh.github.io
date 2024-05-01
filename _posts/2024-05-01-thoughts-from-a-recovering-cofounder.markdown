---
layout: post
title:  "Thoughts from a recovering Co-Founder - Part I"
date:   2024-05-01
categories: blogging
permalink: /blog/:title

---

I started writing this with the intention of noting down some of the lessons I learnt running my own business from idea to acquisition with my co-founder. I thought a brief overview of the company history might be useful backstory, and that quickly turned into a 3000 word essay. So this is going to be Part I. More of a trip down memory lane in the future when I'm old and grey and want to remember the crazy adventure that it was. I've tried to stay as high level as possible, with very few specifics around the product or technical parts of running the business. This is more of a timeline of events. It is not concise, and it's not well written, but it was cathartic getting the past on paper. I'll come back and fill in the blanks at some point, but for now I'll focus on Part II which will serve my original aim of expressing some of my learnings.


## A not-so-brief backstory of Ecofit Homes

### Day 1, Hour Zero

In September 2022, my friend Tim came to me with an idea. He was keen to quit his job in carbon offsetting after he'd become disenchanted with the indutry, and I think he'd be the first to say he's a serial entrepreneur who doesn't fit well in the 9-5. He found there was an API for accessing EPC data. And at the time, that was it. That was the whole idea. So much as to say, there was no idea. We had found some interesting data but had no idea what to do with it. This was accompanied by a very long walk from my house in Islington to Vauxhall and back, where we chatted about UK housing stock, solar panels, and whether there was something we could do together.

This was the day before I started a new job, and a few months earlier I had fallen at the final hurdle for my dream job at Palantir, with the feedback being I needed more technical data analysis experience. So with this in mind, I was pretty excited by the idea of working on a project with Tim that might help me get the Palantir job in a year's time. 

### Week 1

So that week, after work in the evenings, I worked on creating a website where you could put in your address and find out all the information in your EPC. I had done so little research that I didn't even know you could do this on the gov.uk website. I was just focused on building something. 

The following weekend Tim and I got a big piece of paper and a book on how to build a company and started working through what our idea might be. The headline was that we had the least energy efficient housing stock in Europe, and we should do something about this. XX% (a high amount, can't remember the exact figure) houses built now would still be around in 2050, so we need to make them more efficient, improve insulation, install energy generation and storage solutions etc. I've got many more thought around this now, but at the time it was this simple. After about 30 minutes we threw away the book and decided we knew much more about building a start up than the book did (we definitely didn't), and settled on the idea of building what we called "an end-to-end retrofit platform". You could visit out platform, find your house, see what was recommended for you, and get it installed by us. We would do innovative financing schemes, novel after-care products etc etc etc. In other words, a terrible startup idea going against all conventional start up rules. But we were very excited.


### September - December 2022

From September until new year, Tim did all the company incorporation, legal work and admin duties, as well as applying for every grant imaginable. We also dabbled with trying to get angel funding or access to some sort of accelerator. But we had no product, no big finance/tech experience on our CVs and no clients, customers or growth. So grants from our old unis, the Prince's Trust and the Scottish government were the only money we could get our hands on. For a while we had none of this, so Tim and I would have to bootstrap any costs of the business. 

I worked on building our platform. It was the prettiest looking website I had ever built (a poorly contested accolade if I am being honest). I took a week to go to Tim's house in Scotland and officially launch our site. At this time it was just a more graphical way to look at your EPC, but we had some buttons now offering to join a waiting list to get a new EPC or a retrofit assessment or some other incarnation of Tim coming to look at your house for a few hours. This was the first of many pivots as we started to realise we might have bitten off a bit much with our original end-to-end idea...

![](../assets/launching_ecofit.JPG)
*Launching Ecofit at the bus stop in Kirkhill*

After our launch we went out to the pub to celebrate, thinking about the flock of users we were going to get to the least innovative website ever created. Instead, in total we got 1 user that we didn't personally know, a really lovely woman who I sat next to on the train and practically begged her to sign up. In hindsight, we had no reason at all to expect any signups, but we were pretty disheartened.


### Becoming the data player

I can't exactly remember when our next pivot actually happened, but it was by far the most significant. When working with the EPC data to build our platform 1.0, it became pretty clear that this raw data was terrible. The UK was disjointed so England and Wales, Scotland and NI were available from different sources. This also meant the same data was formatted differently for each nation, so was difficult to use in applications. On top of this there were some crazy outliers, and some categorical columns had 100s of different categories with typos, capitalisation and spelling errors all meaning the same thing. We also found a data source from MCS showing that the cost of renewable technology installs varied depending on location within the UK, and these costs were static in the EPC. So if the EPC was conducted in 2009, the cost of panels in 2009 would be quoted. This was obviously useless for actual use in applications. 

So we decided that we would pivot (again). The end to end retrofit platform would be out of our reach without funding, which wasn't forthcoming. Plus lots of other well-backed startups were popping up trying to use the raw EPC data to develop the same thing. So we decided we would be the data player. All these startups, along with utility companies, insurers, mortgage providers and more would need a high quality version of this data. We also had some exciting ideas for how we could build the product out in the future. 

So with this in mind, I started to build out our own data pipeline, taking raw EPC downloads and making the data useful and useable. We called this 'Operation Chestnut' - I still don't really know why.

### "Kill Week"

We knew we weren't getting funding, and our personal funds were running out. I still had a job to pay my bills but I wasn't saving anything, and I wanted to work on Ecofit full time instead of every evening and weekend. Tim had quit his job aboout 4 months before and had only sunk money into Ecofit in this time. 

We decided our best route was to get a client (actually we wanted 5 clients). We would find someone who would buy our data from us and we would scale up from there. Our time was running out, so we decided to hold what we referred to as a "kill week". We lined up phone calls with absolutely everyone who might potentially be a client for 1 week in February. I would take annual leave from my day job and attend every call and work on the product in between. At this point I still didn't see it as taking time off from work (my day job) to work (Ecofit) as I was so keen for it to succeed, but in hindsight using up so much holiday (I'd now used the majority of my holiday allowance to date on Ecofit) when we had no Ecofit wins up to this point was certainly questionable. 

We spoke to every utility company, online estate agent, bank and insurer to pitch our data to them. We didn't even have the pipeline or API in production yet, but we knew we could do it and we just wanted some traction. This was a mind bogglingly frustrating process. We had meetings where executives at energy company would pitch our product to us as what they wanted, then when we said thats exactly what we had, they would say they didn't want it. We had people not understand what we had at all. We had people who were rude. We even had one CTO of an energy company who didn't even know what an EPC was (queue eye-rolls from everyone else on this CTO's team).

But, there were diamonds in the rough. Some people got it straight away and saw what our vision was immediately. Some asked really probing questions about our flaws which was very helpful. Some offered really good advice for where to go next, what to do with the product and who to speak to in their org to progress further.

And standing on a platform in Edinburgh Waverley, Tim phoned me to say he'd just heard that one of these diamonds wanted to make a purchase...

### Utilita Time!

Utilita were one of the diamonds. We had met with some great people who were excited by where our data could fit in with their plans and what they were building. We were pitching 3 products: a data download (our data post-cleaning extracted as CSVs), an API priced per request and a GUI web platform. The pipeline was finished but needed a lot of human intervention for it to run successfully. I had written the code for the API version 0.1 but it wasnt deployed anywhere, and the web platform was "in development"... They said they were interested in a data download to assess the product's utility for them, potentially moving onto the API in future.

A lot was going on at this time for me both personally and across both jobs, so my memory of it is a bit messy. But I do remember sorting contractual negotiations took months not weeks. Then the process of moving the data itself was cumbersome as our two man startup was trying to integrate with a huge coroporation. But we got there, and the money came into our account. This was a massive high for the business and Tim and I went out to celebrate. 

This also started to snowball to a few more successes. We had a couple more people show interest and buy some data. Although these were on a smaller scale, they did show interest in the API and platform in future, so we thought we might be onto something. Plus we were genuinely excited that we had stumbled on an idea to build something great that could have a real world impact! The small amount of money accrued also meant I could quit my day job and work on Ecofit full time. I handed my notice in and had to wait until September 2023, before I could leave. It was frustrating not being able to get right into it when we had momentum, but looking back it's satisfying to have juggled two jobs for the whole year. Knowing I had to wait to start full time on Ecofit meant development and progress on the business took a major hit.

### A British SME abroad

Our traction slowed a little over the summer, and our enthusiasm for being able to make enough money to continue with the business indefinitely waned. While we were still excited by our idea, we just knew the funds weren't forthcoming. The laws of a startup were coming back to bite us. I remember clearly reading an article from YC saying not to go after big clients early on as they move too slowly for a startup - this was depressingly coming true for us. The reality looked like Ecofit was going to either need to morph into something else, or be shut down. We had 3 months runway to get us to Christmas so we did what any broke co-founder should do: pack up, go to Bali and learn to surf.

By this point, Tim had been out of the job market for just over a year, so was pretty keen to get back to a semblance of normal work/life balance. I'd been living back at home for the last ~4 months so was happy to be away, but we were definitely in different headspaces for what we wanted for Ecofit. I was keen to start on the next stage of API development (API 1.0 was by this stage in production). This was referred to as 'Operation Hazelnut' (Again, I don't know why), and focused on expanding on our retrofit recommndations offering to include information on how different technologies would impact energy usage and bills. This was a classic case of the CTO (me) getting excited by cool tech, and the CEO (Tim) seeing the realities of swimming against the tide. We spent a few days during the first couple of weeks in Bali diving deep into UK energy markets, trying to understand where the most impact was to electrify every home. I'll save the detail of our conclusion for another blog, but the short answer is we believed utility companies should transition to do more than provide energy, but also do energy management of renewable assets. This would be a huge industry and energy providers were in the best position to do it at the speed and scale required.

So, with a heavy heart and a beer overlooking the sunset, we decided to put Ecofit into dormancy mode. Utilita wouldn't answer our emails, we were paying to host software that we didn't currently have clients for, and we didn't have the backing to keep building what we thought would be our holy grail. We would look for other ideas to work on as hobby projects, and we could maybe use some of the tech we built for those, but our commercial visions were over.

![](../assets/toasting_ecofit.jpeg)
*Toasting Ecofit*

### Acquisition 1.0

The next day, one of our former clients reached out to us asking for a catch up call. Tim was reluctant to take it, but at this stage beggars couldn't be choosers, and maybe I was still a bit reluctant to actually say goodbye to what we had worked so hard on, so a day after we had ceremoniously killed off Ecofit, we were dusting down the laptops for one last call. Our client in this case was looking to create a Retrofit startup, where our data was essential for their web platform to operate. We had sold very small samples so they could built a POC to show to investors/new clients, but nothing major. On the call with them, they asked how we were getting on and what our plans were. We told them candidly that essentially our hand was forced and we couldn't afford to continue. They then suggested that if that was the case, would we be willing to be acquired, and if so what was our price? We were pretty shocked by this outcome but obviously delighted. We massively undervalued ourselves but given we had written off the business almost 24 hours before, we were just happy that all our hard work could live on! We agreed a few preliminary items about next steps and booked in a more in-detail product call for the following week.

What followed was a months stress and anxiety trying to get the acquistion through. We had multiple calls around negotiating payment, what our roles would be post-acquisiton/what our involvement would be, as well as technical due diligence calls. Outside of this I worked to ensure our code was ship shape and ready for an easy handover. Tim worked hard to provide commerical and contractual information to our potential buyer, and managed all legal and financial implications. Despite us and the people acquiring us being small startups, we took the acquisition seriously, which put us in good stead in the long run.

This period made me very reflective of the change in my technical ability from a year ago when we had started the company. I was much more comfortable problem solving, and while still a long way off being the best engineer, there weren't many technical problems that seemed hugely out of reach (thank you ChatGPT). This was most evident in my attitude to learning, and I was no longer intimidated by new tech I hadn't formally learnt at work or uni. This isn't a great reflection of me as a founder, but I can recall many times throughout the year where Tim would suggest something, I would say it's incredibly difficult, go and read one blog about it and then build it pretty quickly. My attitude radically changed on what was technically within reach, but I'll save more on this for Part II.

Ultimately though, despite the hard work, the acquisition fell through. Everything was due to be completed, but at the last minute the acquiring company's funding fell through, meaning they couldn't complete the purchase in the timelines of our agreement. There was a slim hope that other financing may become available, but I gave this around a 3% chance of happening. Both Tim and I were devastated. I stayed on to travel around Vietnam for 2 weeks, and Tim flew home. It felt like such an underwhelming end to an amazing journey with Ecofit, and we had spent a lot of time and money on this acquisition. Reluctantly, we would have to get jobs, and go back to working on our business ideas as hobbies. I came home pretty dejected, and Tim and I quickly organised a trip up to Scotland to bunker down and do some job applications, while mourning the end of our startup.


### We have some exciting news

Tim suggested one final push, to email all former clients/warm leads and say that we were open for an acquisition. I wasn't keen and pushed to not do it. In fact this is an understatement, I'm pretty sure I begged him not to do it. I can't remember if I eventually caved or he did it anyway, but with hindsight he was definitely right and I was wrong.. We had a couple of calls with prospective buyers which went really well, but our timing, once again, wasn't great. It was just before Christmas so lots of key decision makers weren't around, and all the companies we spoke to seemed to be in a funding round or something else which provided a barrier to acquisition. Maybe they weren't as positive as we thought. That was until Tim sent this email to a contact at Utilita...

```
We've got some news and would love to catch up. 

Would you be free on Monday anytime between 4 and 6pm? 
```

I remember chastising Tim for this. Utilita hadn't responded to our emails since the original sale, the email looked like a phishing attack, and definitely wouldn't work.

I was wrong. They replied 13 minutes later asking what the news was, and we informed them that we were having conversations re acquisitons. A week later they got in touch saying they would like to have a discussion around this and set up calls for us with senior executives who were the decision makers and we then went through the whole acquistion process a second time round. 

This was more formal but the content was the same, the tech DD was longer but the same format, the legal paperwork was more cumbersome and just as boring. This process took a lot longer, and there were more people who needed oversight of different parts of the deal. As this was all happening over Christmas and New Year obviously this slowed down parts as well.

But we got there in the end. The contract was signed on 8th March 2024, and all assets transfered to Procode Technology, the tech subsidary of Utilita.

![](../assets/acquisition2.0.jpeg)
*Toasting the signing of the contract... is there a running theme here?*



We were also moving to Procode to continue to build out the vision and integrate it into their products. Given that twice before we had our hand forced to wind down Ecofit before we were able to realise our overall vision, this felt amazing that we would be able to build what we planned and show the economic value which it has - and thats what we are doing now.


![](../assets/post_acquisition.jpeg)
*With the Procode MD post-acuisition*

___


There's a lot more I could write about all the different stages, but I have tried (and largely failed) to keep to a high level of detail, particularly around the product and tech. The second acquisition process could do with a second blog post, if not just for the comedic value. Maybe it has just been doing it with Tim, but running a company has been a much funnier experience that I would have thought. I might come back and add to this over time as I remember other details and get Tim's input. Sorry if I have misremembered any details!