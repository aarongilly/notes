---
created: 2021-05-22
tags:
  - math
  - science
  - article
aliases:
---
First off, what does “digital” mean?

Digital, as opposed to “analog”, refers to measurements or signals that have been _digitized_[^1]. Digitization is the process of converting a continuous function into a series of discrete elements of a given level of granularity at a given interval (the “sampling rate”). Graphically, that means something like this:

![https://lh3.googleusercontent.com/pw/ACtC-3dYisJvbfh3WbAMRJgKDM-lhrbhrrpPmRQbHa4iCxJgtoi0hv84ewd1wGjjg1TTQpOFWSyBqVTtXw6TRyoUZstHj44_19rv87zuDVxW6M6MRqhyzzEHoC65Gt-JAtBIOqLiQurmfwhKPBPgLzB5f6-ujQ=w1652-h982-no?authuser=0](https://lh3.googleusercontent.com/pw/ACtC-3dYisJvbfh3WbAMRJgKDM-lhrbhrrpPmRQbHa4iCxJgtoi0hv84ewd1wGjjg1TTQpOFWSyBqVTtXw6TRyoUZstHj44_19rv87zuDVxW6M6MRqhyzzEHoC65Gt-JAtBIOqLiQurmfwhKPBPgLzB5f6-ujQ=w1652-h982-no?authuser=0)

If that looks to you like the difference between “continuous” and “discrete” that’s because they are incredibly closely related concepts. Analog signals are continuous, digital are discrete. Analog and digital signals are all around us.

## Analog Things

- AM & FM radios
- Film cameras
- Typical Microscopes and Telescopes
- Mercury-in-glass thermometers
- Cutting a board, using that board to mark the line to cut on the next board
- The actual air pressure waves that cause sound we hear
- The actual frequency of light waves that hit our eyes
- The amount of water in a bucket

## Digital Things

- Internet radio
- Digital cameras
- Electron scanning microscopes and the Hubble Space Telescope
- One of those laser thermometers
- Measuring out 10 inches on a board you’ll be cutting
- MP3 files
- JPEG images
- A whole number of water bottles
- Almost everything else you can think of

# Why Go Digital?

Digital cameras have all but completely obsoleted analog cameras. The United States converted from analog over-the-air television to digital television within the past decade. Computers are digital. Why is everything going digital?

Well, there are a number of reasons.

## Digital is Storable

You can store analog signals, most definitely - but storing digital signals is so much cheaper, easier, and more durable in all sorts of ways.

If I asked you to memorize the curve on the left up there, turn off your computer, wait 90 minutes, then re-draw it from memory, you’d likely have a hard time. However, if we do the same thing and I ask you about the discrete signal on the right, you could simply memorize the sequence of discrete values, then reproduce the signal perfectly using those numbers.

Beyond that, we humans have gotten _really_ good at creating **tiny**transistors. These are the things that hold the “0”s and “1”s in your computer. So if your signal just so happens to be representable using a series of 0’s and 1’s (a.k.a. “if it’s digital”) we can put it into a storage drive alongside any other form of digital content. A digital storage device (e.g. your computer’s hard drive) can store _any_ kind of digital signal. You can’t just mix and match analog storage & transmission devices. Try recording your voice on a mercury thermometer. It doesn’t work.

## Digital is Durable

All signals are prone to noise. You have the signal, then you have all sorts of other junk on top of that signal. As you transmit, amplify, and/or make copies of the source signal, noise tends to accrue. For analog signals, that noise is _cumulative_. Eventually, the signal-to-noise ratio degrades the original material to the point where it no longer satisfies its purpose. If you watched an old VCR magnet cassette tape enough times, you’d realize one day the picture wasn’t as sharp as it used to be.

This doesn’t really happen in the digital world (except in extreme cases, which we’ll get to). Unlike in the world of analog, a digital signal is _discrete._ This allows for some level of error correction.

![https://lh3.googleusercontent.com/pw/ACtC-3f8bbf0-GWlDU814PDVSTudk-x1Ie6d0tU8CWegC9PV3-fqau3nqlrVdRAfSJsjpwVtE6q0awXQ0-uzS6AmXyZBG11g1Bv1oEhl3vEUceNSryg4erZR0AHpoLqyb6jETHd7PFZCDaBKax7nuBQHvlj1fw=w1182-h1512-no?authuser=0](https://lh3.googleusercontent.com/pw/ACtC-3f8bbf0-GWlDU814PDVSTudk-x1Ie6d0tU8CWegC9PV3-fqau3nqlrVdRAfSJsjpwVtE6q0awXQ0-uzS6AmXyZBG11g1Bv1oEhl3vEUceNSryg4erZR0AHpoLqyb6jETHd7PFZCDaBKax7nuBQHvlj1fw=w1182-h1512-no?authuser=0)

Because each middleman in a chain of senders and receivers can “correct” the errors they received from the sender that preceded them, the noise doesn’t accumulate over successive send/receive cycles.

### Metaphorical Example - a Weird Bucket-of-Water-Based Secret Transmission Scheme

If I were to try to transmit the secret number “5” to you by pouring five 20oz water bottles into a bucket, then sending you the bucket. If you knew my encoding scheme, and we agreed in advance that I’d be pouring a **whole** number of water bottles into the bucket, you could use the bucket to fill up a 20oz water bottle 5 times and decode the number 5.

If, however, the bucket spilled a few ounces of water, such that it only filled 4.7 water bottles, you’d _still_ be able to guess the number was “5”. Because 4.7 isn’t a valid number, you can make up for noise in the transmission. You could refill the bucket back up to 100oz before sending it to someone else. This process can be repeated thousands of times without losing the secret number.

If “just any” amount of water were valid, you’d lose a bit of water here and there as the bucket goes on this journey, and have no way to know how much you lost. Eventually, just like in the kids game “telephone”, the secret amount of water received at the end of the line could be drastically different than what was sent originally.

This only goes so far, though. If the level of noise is so bad that the digitization process incorrectly decodes the signal to the wrong value, then a “decoding error” has occurred. In the bucket of water metaphor, this would be like spilling 20+ fluid ounces of water. The receiver of the bucket would only be able to fill 4 bottles and incorrectly decode the secret number as “4”.

## Digital is Secure

Because digital signals can be, to use technical terms, “heavily bothered” without becoming unreadable, we can use some fancier varieties of “heavy bothering” to secure the content of that signal from being ready by 3rd parties in storage or transit. The numbers that a digital signal contains can be encrypted using any number of encryption algorithms, stored or sent securely, then decrypted by recipients with the proper knowledge. Some basic research tells me there isn’t _really_ a method for doing this in the analog realm[^2] (aside from digitizing the analog signal, then encrypting that).

Someday I should do an article on encryption.

# Digital Imperfections

So digital signals are advantageous in a number of ways, so why aren’t they used for _everything_?

Before we start to answer that, let’s cover a bit of vocabulary.

## Digital Vocabulary - Sampling Rate & Bit Depth

There are a bunch of engineering terms in this whole arena, but two of the most important ones are **Sampling Rate** and **Bit Depth**.

Sampling rate is literally the rate at which the analog signal is “sampled” (or _measured_, if you prefer).

Bit depth refers to how many different possible results each measurement is allowed to be. They call it “bit depth” because you use binary “bits” (ones and zeroes) to store the measurements, and you need more bits to hold a wider variety of numbers.

![https://lh3.googleusercontent.com/pw/ACtC-3csfp713LVSibXKRuwUBcvBmB0XQ2R2xMLowV6dqHIQXK2lAkzzoSILH3YXX_Dr63OGr3iPuTExCd8lOUfcrUXi4_izzBkqYj3SNt4_9BnqpyaOceoRcbTZcjpiFqmzo4BUlnyGr1nLbhDf0Qn1JUYcjA=w1756-h1065-no?authuser=0](https://lh3.googleusercontent.com/pw/ACtC-3csfp713LVSibXKRuwUBcvBmB0XQ2R2xMLowV6dqHIQXK2lAkzzoSILH3YXX_Dr63OGr3iPuTExCd8lOUfcrUXi4_izzBkqYj3SNt4_9BnqpyaOceoRcbTZcjpiFqmzo4BUlnyGr1nLbhDf0Qn1JUYcjA=w1756-h1065-no?authuser=0)

# Cons of Going Digital

## Quantization Error

Humans experience the world through analog signals. Digital signals are, at best, _approximations_ of analog signals. If you listen to a guitar being played live, you’re hearing the completely unadulterated analog audio signal, carried via pressure waves in the air. Once that audio signal is encoded into a digital format, you’re losing some level of fidelity.

![https://lh3.googleusercontent.com/pw/ACtC-3cGIrcWdJa_Vfk_AUu5D5OEIScM7ESpIiJZeBH9rnfegXKJ_LWS8RzlQgkwsO7J0oZNudXZ5wABQEOQWXEYiUguYpMg_FhtXlCL1yKqy9aKc3-WvQwMw3aGvRMBYSM-fAKl5ccwPdCvr_GwPApJMbQG-A=w1219-h1586-no?authuser=0](https://lh3.googleusercontent.com/pw/ACtC-3cGIrcWdJa_Vfk_AUu5D5OEIScM7ESpIiJZeBH9rnfegXKJ_LWS8RzlQgkwsO7J0oZNudXZ5wABQEOQWXEYiUguYpMg_FhtXlCL1yKqy9aKc3-WvQwMw3aGvRMBYSM-fAKl5ccwPdCvr_GwPApJMbQG-A=w1219-h1586-no?authuser=0)

The red shaded in area is the “quantization error” introduced when doing the analog-to-digital conversion. It’s an artifact of the digitization process, and is unavoidable.

When audiophiles insist on vinyl and other analog representations of their music, that loss of fidelity is what they’re trying to avoid.

### Buying Back Fidelity

You can minimize loss of fidelity from this effect by increasing the sampling rate and/or increasing the bit depth of the digitization process.

![https://lh3.googleusercontent.com/pw/ACtC-3crW6h5PxTwQUyiwpnFwDkFWjDDNhQFX5EzAtowkvaYxDNg74cbiUJS53R-tmJXYRAffYKKkKuGR5e9l61WhCrTo24EbJwt7RD9uBj87xJ2iNK3IBl44a7WnSklOigHExNVuMuzYcf4qEmECwbwOeX9gw=w1246-h1810-no?authuser=0](https://lh3.googleusercontent.com/pw/ACtC-3crW6h5PxTwQUyiwpnFwDkFWjDDNhQFX5EzAtowkvaYxDNg74cbiUJS53R-tmJXYRAffYKKkKuGR5e9l61WhCrTo24EbJwt7RD9uBj87xJ2iNK3IBl44a7WnSklOigHExNVuMuzYcf4qEmECwbwOeX9gw=w1246-h1810-no?authuser=0)

The higher the sampling rate and the higher the bit depth, the closer and closer the digitized line comes to approximate the analog signal. To dip my toe into calculus waters, the limit as both of those factors approaches infinity is a perfect copy of the analog signal itself.

But higher sampling rates and higher bit depths both come at the expense of losing a bit of the benefits that “going digital” buys you. The smaller the distance you have between the possible values on the Y dimension, the less likely you are to be able to correct for noisy signals. The higher the sampling rate, the larger the digital representation of the signal becomes. Combine high sampling rates with high bit depths and you get a very vibrant, detailed signal that takes a lot of storage capacity to save, bandwidth to send, and compute power to process. For example, the difference between the encoded signals on the bottom left and bottom right of the image above is:

`8,6,7,5,3,0,9` ← 7 samples, each 1 digit long = 7 digits to transmit

`8.0, 6.5, 6.0, 6.5, 7.0, 5.5, 4.5, 3.5, 2.0, 0.5, 0.0, 4.0, 9.0` ← 13 samples, each 2 digits long = 26 digits to transmit

Like most everything, the key is in finding the best balance of sampling rate and bit depth for whatever the situation needs.

## Aliasing & the Nyquist Rate

One last concept I’ll mention, because it’s a term you’ve probably seen before in the settings of your TV, is the concept of “aliasing”. Aliasing is what you’re seeing when a picture of a carpet or a computer monitor or something and it gets funny looking patterns all over it that aren’t there in real life. Like the bricks on the right:

![https://lh3.googleusercontent.com/pw/ACtC-3cbF34QP-VLP4O1WW6xldBD0bEBWg3wAQeHjVGzjNswIepc6U0tIdQtPUIbww5XZrJ85oxYavMZnUtpRl7A2VA0h5R3fLK6GAxxPQFu1FzMX8HpBSR_VIWH9S5lcztjR8AlgrQReNTzx8VHo61KdZWlOg=w1251-h806-no?authuser=0](https://lh3.googleusercontent.com/pw/ACtC-3cbF34QP-VLP4O1WW6xldBD0bEBWg3wAQeHjVGzjNswIepc6U0tIdQtPUIbww5XZrJ85oxYavMZnUtpRl7A2VA0h5R3fLK6GAxxPQFu1FzMX8HpBSR_VIWH9S5lcztjR8AlgrQReNTzx8VHo61KdZWlOg=w1251-h806-no?authuser=0)

Image derived from [Wikipedia](https://en.wikipedia.org/wiki/Aliasing)

Basically, what’s happening here is that the sampling rate of the digitization process is too low to capture the highest frequency components of the analog signal being captured. Any time the frequency of the input signal is over half that of the sampling rate, you’re going to have some form of aliasing. The rate at which a signal can be sampled without aliasing is x2 that of the highest frequency in the signal. This is called the “Nyquist Rate”.

![https://lh3.googleusercontent.com/pw/ACtC-3f-zGlnhmXShge2QXMeZs-AKn44BsqUQclQhS3Pkzbz4DXjsoHAAev2iqCLJ9hkqTYpp_dh7CwU-XsmUXk7HaEClG7H9SsWWuRkDvYKRsrCKR0Uhl1GgOXh_OTDYE0KPuvDOzJ3tnEwIZTBg-VnhjPDWQ=w1278-h947-no?authuser=0](https://lh3.googleusercontent.com/pw/ACtC-3f-zGlnhmXShge2QXMeZs-AKn44BsqUQclQhS3Pkzbz4DXjsoHAAev2iqCLJ9hkqTYpp_dh7CwU-XsmUXk7HaEClG7H9SsWWuRkDvYKRsrCKR0Uhl1GgOXh_OTDYE0KPuvDOzJ3tnEwIZTBg-VnhjPDWQ=w1278-h947-no?authuser=0)

Given only the signal on the right, you’d have no idea Jenny’s phone number has a zero in it.

# Conclusion

The difference between analog and digital signals is closely related to the difference between continuous and discrete functions in mathematics. Digital signals offer a lot of advantages over analog signals, but can also cause problems if you’re not sure of what you’re doing. Digitization is the process of converting analog signals to digital ones. Higher-fidelity digitization starts to lose you some of the benefits of going digital in the first place, but too low of a fidelity causes the original signal to be lost. Digital engineering is neat.

**Fun fact** - the etymology behind the term “digital” is from the Latin “_digitus_”, which refers to fingers or toes… because we use them to count. If you can’t count it, it’s not digital.

[^1]: Way to use a more esoteric term in the definition of a relatively simple term, Aaron)

[^2]: I love it when I Google something and find that the only relevant results are academic papers.