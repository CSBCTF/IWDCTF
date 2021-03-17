Challenge: See,not hear

Message: Find the flag

Value: 100

<img src="https://github.com/CSBCTF/IWDCTF/blob/08077b858d9836de6668299bdaf7ea0d67ce4a80/forensics/See,%20not%20hear/files/Capture.PNG">
<br>

When the audio files is open. We can hear a morse code like sounds. From the title we need to see it. So let's open an audio editor, Audicity.

<img src="https://github.com/CSBCTF/IWDCTF/blob/08077b858d9836de6668299bdaf7ea0d67ce4a80/forensics/See,%20not%20hear/files/Capture1.PNG">


Opening the audio file in Audacity.

<img src="https://github.com/CSBCTF/IWDCTF/blob/405761b7757e5740f1645aec706cdf45bf38a741/forensics/See,%20not%20hear/files/Capture2.PNG">

There is nothing much we could see. Lets open the spectogram

<img src="https://github.com/CSBCTF/IWDCTF/blob/405761b7757e5740f1645aec706cdf45bf38a741/forensics/See,%20not%20hear/files/Capture3.PNG">

From above, we can see the flag is hidden in the spectogram.

<img src="https://github.com/CSBCTF/IWDCTF/blob/405761b7757e5740f1645aec706cdf45bf38a741/forensics/See,%20not%20hear/files/Capture4.PNG">

You could edit the spectogram setting to see better. Editing the range and the gain would makes it more visible.

Flag: IWDCTF{you_c@n_s33_@udio_2}
