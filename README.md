# Jokely 
## A machine intelligent enough to create humanlike jokes
[[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1naor0BgRj4Q9x0NKPjBT7kqBqK3aKOuS?usp=sharing)]
A machine learning model that generates amazingly intelligent jokes
## How big is the training dataset
Eventually the training dataset is 200,000 jokes
## How did I make it work?
Last day I opened my computer and saw a weird thing. it said how a computer was able to generate precisely context-based jokes from just using a transformer model, then I knocked my head and said "what the hell was that it looks like a human said it", then I remembered GPT-2(the master of lies) and said for my self "If a raw transformer can create jokes then a GPT-2(again, trained with 40GB of human knowledge) can be more intelligently humourous while creating jokes, it's obvious that it could do so because well GPT-2 already knows a lot of grammar and human representation of things. So, I went and asked where could I get such dataset and just went with a google search ( jokes database GitHub ) funny but it worked... here's the result https://github.com/taivop/joke-dataset, I used the reddit_jokes.json file. Then got into a google search again (Google Colab GPT-2 pypl) then opened the Google Colab made a new copy on my repo (https://colab.research.google.com/drive/1naor0BgRj4Q9x0NKPjBT7kqBqK3aKOuS?usp=sharing). then joined the title and body as a one-liner attached by "||" then just made a list of them as lines and saved it in a file. then I went on training the model. here's the result

![Results](https://preview.redd.it/7gl16qfb0jh51.png?width=967&format=png&auto=webp&s=c0656c69c247e08930e8c4983f71f68ce433fff2)

So, here's what I think happened.

The transformer model pretty much used its first knowledge of transforming and aligning and even contextualizing raw list of BPE's and used it on the jokes while being trained, that allowed it to create human-like jokes that are pretty.

Here's some evidence

    I asked my girlfriend if she knew what sex was like || she said that you can kiss her and she'll think you're a queer.

You can see this sentence and understand that the sentence before "||" is like a question and all the jokes in the prepared to train jokes are like this so the machine understood that changing the sentence before "||" is much of underscored so I just got my computer and searched "I asked my girlfriend if she knew what sex was like" on the list of sentences. amazing it's there but "she said that you can kiss her and she'll think you're a queer" was never there even searched from the half that means the ML model generated the best fit for the question, interesting! huh.

What about using prefixes

    Why does the teacher have her own car? || She's a car company for Santa.

I used a prefix for the GPT-2 model which says "the teacher have a car" and so it got this. it's amazing how it could even generate a humourous answer for an unknown question because well it didn't overfit and the amazing part was the temperature was just set to 0.6. but even with this humour I still got to a problem of understanding what "She's" meant. because it could change everything if it meant she has it would be much funnier than "she is", uh! bias in the training data.

My conclusion

I think I just prove that Machine learning is being more humourous and contextual and that's very good.

Anyone who wants to give ideas feel free to do so. I am happy to learn.
