<h1>Markov's Muse: Using N-Gram Markov Chains to Generate Emotion Based Lyrics</h1>
Hannah Shu - hshu100@stanford.edu

<h3>Abstract</h3>
With Spotify's AI detection systems becoming increasingly popular as a source of music listening, curated playlists based on our emotions are gaining traction. Songs have always had the power to capture the emotions of their writers and convey those feelings to their listeners. Large Language Models, such as ChatGPT, generate responses using techniques like n-grams, which predict the next word in a sequence given the previous words. This process, though probabilistic, can be refined using Markov matrices often associated with n-gram models. By combining these two concepts, we can develop a program that writes songs based on specified emotions, creating a more personalized and emotionally resonant music experience.

<h3>Data Collection</h3>
Web Scraping Lyrics from Artists: With a plethora of different artists that were recommended by Jerry and my friends, I was able to web scrape 11 different artists and their full song lists. From this, I scraped the lyrics of each individual song using BeautifulSoup and added them in dataframes based on the artist. 

Emotion Lexicon: For this project, I used an emotion lexicon, specifically the NRC Emotion Lexicon, which is a list of words associated with eight basic emotions: anger, fear, anticipation, trust, surprise, sadness, joy, and disgust. Each word in the lexicon is tagged with one or more of these emotions, indicating an association between the word and the corresponding emotion. Using the lexicon, I was able to influence the word selection process during the generation of lyrics by appending words that are associated with emotion. 

<h3>Probabilistic Model</h3>
Can be found in my write up

<h3>User Interface</h3>
I used Visual Studio Code and Jupyter Notebook to train my model and generate lyrics. Users can input various parameters, including changing the n value for the n-grams, selecting the desired emotion for the lyrics, and specifying the artist. I have loaded datasets for 11 artists into the notebook. Additionally, users can specify the section of the song they want to generate, such as the Chorus, Intro, and so on.

<h3>Future Work</h3>
I would like to explore the differences between human and computer-generated lyrics and develop a system to evaluate how "fake" the computer-generated lyrics appear, focusing on the linguistic aspects. Additionally, I aim to ensure that emotions are more prominently highlighted in the generated lyrics. Although my models could randomly select words that the artist wrote, which were also in the lexicon, the occurrence was still very low. To improve this, I am considering finding a lexicon that determines the emotion of a word based on its intensity or strength.

<h3>Acknowledgements/Inspirations</h3>
I would like to acknowledge that this project was inspired by an assignment I completed in a previous class (DATASCI 112), where we learned how to create unigram and bigram models. I decided to take the skills I acquired from that class, particularly in unigram/bigram modeling and web scraping, and apply them to this project. Additionally, I was inspired by ChatGPT and how it uses N-Gram Markov Chains to create its Large Language Models (LLMs).

<h3>Sources</h3>
Emotion Lexicon: https://www.saifmohammad.com/WebPages/NRC-Emotion-Lexicon.htm 
N-Gram Chat GBT: https://livecode.com/chatgpt-language-models-101/ 
Lyrics: https://lyrics.az/kendrick-lamar/allsongs.html, https://lyrics.az/luke-combs/allsongs.html, https://lyrics.az/olivia-rodrigo/allsongs.html, https://lyrics.az/ed-sheeran/allsongs.html, https://lyrics.az/mitski/allsongs.html, https://lyrics.az/joji/allsongs.html, https://lyrics.az/the-beatles/allsongs.html, https://lyrics.az/seal/allsongs.html, https://lyrics.az/taylor-swifts/allsongs.html, https://lyrics.az/billie-eilish/allsongs.html, https://lyrics.az/hozier/allsongs.html

