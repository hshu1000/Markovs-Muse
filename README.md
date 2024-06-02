# Markovs Muse
 
<h1>Markov's Muse: Using N-Gram Markov Chains to Generate Emotion Based Lyrics</h1>
Hannah Shu - hshu100@stanford.edu

Abstract
With Spotify's AI detection systems becoming increasingly popular as a source of music listening, curated playlists based on our emotions are gaining traction. Songs have always had the power to capture the emotions of their writers and convey those feelings to their listeners. Large Language Models, such as ChatGPT, generate responses using techniques like n-grams, which predict the next word in a sequence given the previous words. This process, though probabilistic, can be refined using Markov matrices often associated with n-gram models. By combining these two concepts, we can develop a program that writes songs based on specified emotions, creating a more personalized and emotionally resonant music experience.

Data Collection
Web Scraping Lyrics from Artists: With a plethora of different artists that were recommended by Jerry and my friends, I was able to web scrape 11 different artists and their full song lists. From this, I scraped the lyrics of each individual song using BeautifulSoup and added them in dataframes based on the artist. 

Emotion Lexicon: For this project, I used an emotion lexicon, specifically the NRC Emotion Lexicon, which is a list of words associated with eight basic emotions: anger, fear, anticipation, trust, surprise, sadness, joy, and disgust. Each word in the lexicon is tagged with one or more of these emotions, indicating an association between the word and the corresponding emotion. Using the lexicon, I was able to influence the word selection process during the generation of lyrics by appending words that are associated with emotion. 
