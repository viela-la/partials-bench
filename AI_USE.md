# AI Usage Statement
## Acknowledgement
Claude AI was used to generate all code in the `index.html` for the app in this repository, as well as the information in the `README.md` file.
## Logs
### Week 2: October 8, 2026
"-Make an app that allows you to add frequencies and amplitudes by typing. Make sure you can see the waveform and hear the sound.
Play with it.
Add 'random' frequencies.
Add a frequency and its multiples e.g. 100, 200, 300,... For the waveform window, make sure that you can change the scale. See many seconds, 100 ms, etc."

In testing this code, I compared the resulting app to the app my mentor demonstrated during our meeting session. As I was still grasping foundational knowledge of sound, I took to face-value that the sounds were producing correctly. After confirming the app was comparable to my mentor's example, I deemed the resulting code as acceptable. Claude AI had also automated adding harmonics or random frequencies to the partials table. For the harmonics, I was able to choose the fundamental frequency, the number of harmonics to add on top of it, a flat amplitude scale, and an amplitude shape drop-down. For the randoms, I was able to choose the number of partials and the ranges of frequencies and amplitudes allowed. For both automations, I was able to check a box to allow the current table to be replaced with a new generated array of frequencies.

### Week 4: October 24, 2026
"for the partials bench can you add a microphone and an automatic way of synthesizing vowels"

To test the resulting changes to the app, I first ensured it could still perform the original functions (adding and scaling frequencies). Afterwards, I tested the microphone aspect. It was correctly capturing my voice and correctly reporting back the vowel sound I was making. For the vowel synthesis, Claude had mapped the vowels in a 2D space, with the formants on the axes, and a dropdown of 3 different voice choices to synthesize the vowels in. I played all 10 vowel sounds in all 3 voices to ensure they sounded as I'd expect. Claude had also added a "Sequence" aspect where I could type in vowels and they'd be synthesized in that set order.

### Week 5: October 25, 2026
"can you add a way to copy the fundamental frequency of the captured voice/vowel and synthesize the other vowels out of it"

First, like always, I made sure the previous functions still worked properly. Then, I used the microphone to capture my voice and its pitch. The app mapped the training sound to the correct vowel on the 2D map. I then cycled through each of the vowels, playing them in my own synthesized voice, and ensured they sounded like me.

### Week 5: October 28, 2026
"incorporate a filter the user can move around"

Claude added a filter checkbox to the spectrum box. It provided a dropdown of different filter options, which all resembled the ones shown by my mentor in his spectrogram demonstration in-class. They worked as I'd expected.

"can the filter be fully draggable -- so i can add peaks and valleys wherever by dragging the filter response"

Since my main concern was replicating my mentor's app, I had to make the filter fully draggable like his was. The result was finicky, as the filter would move up and down in unexpected ways, but the frequencies' amplitudes transformed as expected.

### Week 5: October 29, 2026
"how can i make a github repo for the partials bench app"

I've never used Claude before this quarter. I've yet to figure out how to connect my GitHub account to my Claude account. The day after I learned I needed a GitHub repository for my code to live, Claude was able to gather the necessary files for a repository -- also generating the `README.md` file and populating it with necessary setup, usage, and functionality information. I created the repository and uploaded the app's files.
