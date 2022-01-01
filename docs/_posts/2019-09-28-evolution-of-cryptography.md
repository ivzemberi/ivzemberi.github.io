---
layout: post
title: "Evolution of Cryptography"
image: /blog_assets/cryptography-unsplash.jpg
hero_image: /blog_assets/cryptography-unsplash.jpg
hero_darken: true
---

>The art of writing and solving codes was a necessary skill even in ancient times. Even though that was the time where 
most of the population was still illiterate, powerful leaders could not risk their tactics being revealed to the enemy.

The solution to that problem was coming up with a cypher to encode the messages. That way they were sure their tactics, 
hidden in the messages, would not fall into the wrong hands.

That being said, we can assume that the cypher that Caesar used when he was a powerful leader, is not very secure 
nowadays. The main reason he got away with it, was that the illiteracy was common in his time.

##### The Caesar Cypher

*The Caesar Cypher* is a classical substitution and historically the oldest cypher. It is based on shifting each letter 
of the Latin alphabet by a predetermined number.

Example:

The message we want to send is: “ATTACK AT DAWN”, and the predetermined number is 3.

<figure align="center">
    <img src="/blog_assets/shifted-alphabet-3.png">
    <figcaption align="center">Shifting the alphabet when the predetermined number is 3</figcaption>
</figure>

“ATTACK AT DAWN” → “DWWDFN DW GDZQ”

There are a few problems with this cypher. First of all, there is a limited number of keys to use. One could try them 
all in a day and decode the message. Secondly, with the letter frequency analysis, the key can be found even faster. 
Also, the word constraints are making it easier to find the key. But again, this cypher was used in the time illiteracy 
was common.

##### The Polybius Square

Similarly to *Caesar’s Cypher*, there is *The Polybius Square* which uses a 5x5 grid that shows the coordinates of the 
letters. Due to the Latin alphabet having 26 numbers, “I” and “J” are on the same coordinates.

Example:

We want to send the same message, “ATTACK AT DAWN”, but using this cypher:

<figure align="center">
    <img src="/blog_assets/polybius-square.png">
    <figcaption align="center">The Polybius Square</figcaption>
</figure>

“ATTACK AT DAWN” → “1144111325 1144 14115233”, but to make it a bit harder to decode it is better to remove the spaces, 
so the message should look like this: “1144111325114414115233”.

Of course, this cypher also has its problems. Considering that each number is numbered from 1 to 5, the antagonist can 
easily conclude that the cypher is based on some kind of grid. Once he/she sees that, decoding becomes trivial. Today, 
a modern computer could do it in a millisecond.

Some cyphers are used purely for fun, for example, *The Pigpen Cypher, FonCode, ROT13*, etc. Even though each is 
different from the next, they are mostly used for fun, by kids in school or on Internet forums.

All these cyphers I mentioned before have one thing in common. They are easily breakable. Opposed to that, there is 
***The Vigenere Cypher***.

##### The Vigenere Cypher

*The Vigenere Cypher* is best described as many Caesar shift cyphers combined at once. The timing of the shifts is 
usually determined by a keyword, and the user of a Vigenere Cypher usually carries on him a cypher wheel or a Vigenere square.

Example: *Encoding “ATTACK AT DAWN” using The Vigenere Cypher*

Plaintext: ATTACKATDAWN

Key: MEDIUM

Keystream: MEDIUMMEDIUM

Cyphertext: MXWIWWMXGIQY

<figure align="center">
    <img src="/blog_assets/vigenere-square.png">
    <figcaption align="center">The Vigenere Square</figcaption>
</figure>

To understand the encryption it is important to know:

- All involved must agree upon a key to use, and the key is typically one, easy to remember word.
- The keystream is as long as the text we want to encode. That is why our keystream is long 12 letters, “mediummedium”.
- The upper alphabet signifies the letters from plaintext, and the one on the left signifies the letters from the 
keystream. Marked red, are the coordinates of the letters that are used in the cyphertext.

##### Conclusion

Due to the increase in the level of education, and of course, the advancement of technology, it is logical that 
cryptography is constantly evolving. Today we have a lot of encryption methods and algorithms that are used in coding 
to secure sensitive data.

The thing about these particular cyphers is that they all share some similarities. Each cypher I described is at least 
a few centuries old. Moreover, they also show the process of evolution, from Caesar’s Cypher being the easiest to break,
Polybius Square which is a tad more difficult, and finally, the Vigenere Cypher which is almost impossible to break 
without having the key.