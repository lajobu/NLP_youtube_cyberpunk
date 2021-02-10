# Sentiment analysis performed on the transcripts and titles of youtube videos related to the game Cyberpunk 2077

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) 

![Cyberpunk 2077](https://i.ytimg.com/vi/8X2kIfS6fb8/maxresdefault.jpg)

The purpose of this project is to apply `Natural Languague Techniques`, concretly, `sentiment analysis` to transcripts and description of several youtube videos. 

The choseen topic is the videogame `Cyberpunk 20177` and the data was scrapped from Youtube 6 days after the game was released.

## Technical details about thje project:

 :round_pushpin: **Programming language:** `Python`

 :round_pushpin: **Libraries:** `moviepy`, `speech_recognition`, `youtubesearchpython`, `librosa` and `nltk.sentiment.vader`
 
## Data scrapping process: 

1) Firstly several searches were performed in YouTube, such as: `cyberpunk 2077 review`, `cyberpunk 2077 recommended`, `cyberpunk 2077 problem`... There were made several of them as the package `SearchVideos` has a limit of videos for each search
2) The videos were downloaded as `mp4` format
3) The audio of each video was extracted as `wav` format
4) `Speech recognition` was performed for the first `3 minutes of each video`

- Result: `136 videos` with the following features:

-- `url`
-- `description`
-- `duration`
-- `views`
-- `transcript`
-- `rating`

:link: [Data extraction](https://github.com/lajobu/NLP_youtube_cyberpunk/blob/main/1.data_extraction.ipynb)

## Next steps: 

:link: [Data description](https://github.com/lajobu/NLP_youtube_cyberpunk/blob/main/2.data_description.ipynb)
:link: [Sentiment analysis on Transcript](https://github.com/lajobu/NLP_youtube_cyberpunk/blob/main/3.sentiment_analysis_transcript.ipynb)
:link: [Sentiment analysis on Description](https://github.com/lajobu/NLP_youtube_cyberpunk/blob/main/4.sentiment_analysis_title.ipynb)

## Some figures:

- Audio representation:
![alt text](https://github.com/lajobu/NLP_youtube_cyberpunk/blob/main/Figures/output_19_1.png)

- Density plot of rating feature:

![alt text](https://github.com/lajobu/NLP_youtube_cyberpunk/blob/main/Figures/rating_distribution.png)

- Wodcloud on Description, not liked group:

![alt text](https://github.com/lajobu/NLP_youtube_cyberpunk/blob/main/Figures/words1_nl.png)

- Wodcloud on Description, liked group:

![alt text](https://github.com/lajobu/NLP_youtube_cyberpunk/blob/main/Figures/words2_l.png)

## Results and conclusions:

### - `Sentiment analysis` applied to the `youtube platform` could be an `attractive analysis` for some companies. Many people before buying the products review related videos on this plattform
### - This kind of analysis could be also usefull for `content creators`, because they will be able to extract information about what the people like the most
### - In some analysis such as the presented, it is `enough to have the title of the video`, rather than a partial transcript, however this would `depend of the analysis`
### - The current analysis showed that `after the release of the game Cyberpunk 2077`, the `youtube users didn't like` videos related to `technical aspects` of the game, about the `plattforms` or `criticism` of the game. However, it `should be analysed deeper in the video comments` if the people didn't like the videos because they `agree with the content` of the video (the didn't like the game) or just because they `didn't agree with the video` (they like the game)
### - In my opinion the `people may have been curious about the game`, for this reason the group of `liked videos` are mostly related to `gameplays`, about `features` of the game (for example `cars`) or `speaking well about the game`. This was expected, as the `videos were extracted just 6 days after the release` of the game, and probably a lot of possible buyers were looking for more information about the game
