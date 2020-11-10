---
layout: post
title: What is Apple Silicon and Why Does It Matter?
date: 2020-11-10 15:30:00
author: Stefan
---

Tonight at [10 a.m. PST / 7 p.m. CET](https://www.timeanddate.com/worldclock/fixedtime.html?msg=Apple+Event&iso=20201110T1800), there will an Apple Event called "One more thing." It is heavily rumored and very likely that they will announce the first Apple Silicon Macs. But what is Apple Silicon and why does it matter?

## Apple Silicon?
{% include image.html src="2020-11-10/IMG_0013.jpg" width="300px" title="Funny screenshot from Reddit" %}

No, we're not talking about breast implants, but about SoCs (system on a chip). Up til now[^1], Apple has been using Intel CPUs for all they Mac computers, whether laptops or desktops. Intel, however, has not been able to fulfill their promises and deadlines about new processor development, therefore giving only slight improvements in recent years.

In Apple's other products, most notably iPhones and iPads, Apple has been using their in-house designs for SoCs.[^2] And Apple has shown that they are really good at chip design. Year over year, their chips deliver large improvements, and it has barely slowed down since they started. Because of this, Apple's mobile CPUs have surpassed the Intel CPUs they are using in Macs. The iPad Pro's A12X/A12Z[^3], which was first released in 2018, is faster than most of Apple's current MacBooks on the market. This year, they announced the A14 SoC in the new iPad Air and the iPhone 12 line. While it has less CPU cores than the A12X and is therefore still behind in multi-core processing, its single core scores have been very high, and it still beats a lot of the MacBooks Apple is selling. This means that the iPhone is now faster than many of Apple's MacBooks. That's sad.

For a few years already, there have been rumors about Apple introducing their in-house chip design for Macs. Finally, at this year's WWDC[^4] in June, they announced the transition from Intel to Apple Silicon. It is important that they announce it beforehand since Intel (as well as almost all laptop and desktop computers on the market) uses x86 chips, while mobile CPUs (including Apple's) use ARM chips. These are different instruction set architectures, and therefore, software built for one cannot run on the other. This means that developers need to prepare their software to run on the new chipsets.[^5] In addition to the transition, they announced a Developer Transition Kit (a Mac mini running on a A12X) that developers can register for and use to test their applications, as well as the release of the first Apple Silicon Macs to the public "at the end of 2020."

Well, we're almost at the end of 2020, therefore we can assume tonight's event will be about the Apple Silicon Macs.

## Why Is This Exciting?
As I already noted, Apple's mobile chips used in iPhones and iPads already surpassed most of the Intel chips used in MacBooks today. The yet-to-be-released A14X is rumored to be faster than **every** Intel MacBook on the market. This is exciting because the chips we're talking about here are passively cooled, run at a lower TDP[^6], and still deliver higher performance than Intel's chips.

If we now assume that Apple can adjust these chips to be actively cooled (i.e. with a fan), we can expect even higher performance. That combined with the fact that MacBooks have more space and more battery means that Apple Silicon Macs will beat the shit out of the current Intel MacBooks.

We don't know any specifics, but we can easily assume that Apple Silicon MacBooks will be much faster than current Intel  MacBooks.

An additional consideration is that using their in-house SoCs for Macs, it means that they have even more control over the hardware and it is possible that the software (in particular the operating system) can be optimized for these new chips. This could lead to additional performance improvements, power savings, or even new features like a low power mode.

## What Can We Expect Tonight?
Apple's current lineup of Intel MacBooks consists, basically, of three models:
- MacBook Air 13"
- MacBook Pro 13"
- MacBook Pro 16"

It is expected that they will introduce Apple Silicon chips in at least the first two of these models, maybe even for the 16".

For the Air, I can imagine them simply using the A14 that the iPad Air and the iPhone 12 line are using. For the lowest end CPUs, this would already be a big leap in performance and especially in power efficiency. However, I could also imagine that they will use an A14X in these. Not sure how good it looks if the MacBook Air is using the same chip as the iPhone.[^7]

For the Pros, it is likely that they use a variant of the A14 chip, like an A14X or something even more powerful. For the 13" MacBook Pros, this would be a big upgrade and will likely suffice both in terms of CPU and GPU performance. However, one thing to consider is that the 16" comes with a dedicated GPU, so if Apple announced an Apple Silicon 16" MacBook Pro, they would need to provide improvements in GPU performance compared to what's currently in their chips. It is very likely that they will replace the dedicated GPUs with integrated GPUs though. Even modern consoles (like the PlayStation 5 and the Xbox Series X/S) use SoCs with integrated GPUs, so it is certainly possible to have enough GPU power even with an integrated GPU.

Currently, there are no indicators that Apple will announce any desktop computers with Apple Silicon. However, since the Developer Transition Kit uses a modified Mac mini, one could think that it would be trivial to release something similar to the public. Also, it has been rumored that the iMac will also get Apple Silicon chips soon. What I'm thinking is that Apple's manufacturing capacities won't be enough to release all of these at once, hence staging the releases so that manufacturing can keep up. Or they are simply not ready yet.

---

I hope that this post was informative and not too technical. While I don't plan to buy an Apple Silicon MacBook immediately, I am considering upgrading my 2015 MacBook Pro next year. I might wait for the second generation of Apple Silicon Macs though.

Expect a summary of tonight's event in tomorrow's blog post!

[^1]: Since 2006 when Apple [transitioned from PowerPC to Intel](https://en.wikipedia.org/wiki/Mac_transition_to_Intel_processors).
[^2]: Ever since the iPhone 4 and the first iPad, with the [Apple A4 SoC](https://en.wikipedia.org/wiki/Apple_A4).
[^3]: The A12X was introduced in 2018 with the redesigned iPad Pro 11" and 12.9". The A12Z is a variant of the A12X with one more GPU core and was introduced in the 2020 iPad Pros earlier this year.
[^4]: World Wide Developer Conference
[^5]: This sounds more dramatic than it is, at least for most developers. If you are using a high-level programming language, especially Swift which is what is commonly used for Mac applications, recompiling your application for ARM should be fairly trivial and could be as easy as flipping as switch. However, for more complicated applications or applications that depend on old legacy code, this might be much harder.
[^6]: Thermal design power, i.e. how much power they consume and how much heat they dissipate.
[^7]: Additionally, people are still hoping for a new 12" MacBook which could then use the A14. There have been no rumors about this coming today though.
