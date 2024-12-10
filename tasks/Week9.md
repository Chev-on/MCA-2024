[<kbd> <br> Home <br> </kbd>](../README.md) [<kbd> <br> Week 2 <br> </kbd>](Week2.md) [<kbd> <br> Week 3 <br> </kbd>](Week3.md) [<kbd> <br> Week 4 <br> </kbd>](Week4.md)  [<kbd> <br> Week 5 <br> </kbd>](Week5.md) [<kbd> <br> Week 7 <br> </kbd>](Week7.md) [<kbd> <br> Week 8 <br> </kbd>](Week8.md) [<kbd> <br> Week 9 <br> </kbd>](Week9.md) [<kbd> <br> Week 10 <br> </kbd>](Week10.md) 


# Week 9 

<html>
<h2>Task 1 - Extract Features <h2><br>

	
		<p>For Week 9's task, we were asked to identify 3 tracks related to out portfolio theme and present a Spectrogram, Mel Frequency Cepstral Coefficients, and a Chromagram alongside the orignal waveform. 
		For the purposes of this weeks task, I will reuse the tracks I analysed in Week 8.</p><br>
		
        <br>
      		
      		<h3 class="h3w8">Movement 1 - Allegro Non Molto</h3><br>
      		
      		<img src="../week9/mv1/mv1.png" alt="Allegro Non Molto" style="display: block;margin-left:auto;margin-right:auto;width:900px;height:650px;"><br>
      				
      		<h3 class="h3w8">Movement 2 - Adagio e Piano</h3><br>
      		
      		<img src="../" alt="Tremor Analysis Features" style="display: block;margin-left:auto;margin-right:auto;width:900x;height:650px;"><br>
      		
      		<h3 class="h3w8">Aftershock & LCXCPR - Party Like a Rockstar</h3><br>
      		
      		<img src="../images/rockstarw9.png" alt="Party Like A Rockstar Analysis Features" style="display: block;margin-left:auto;margin-right:auto;width:900x;height:650px;"><br><hr>
      		
      		<h2>Computing and Visualising Histograms</h2><br>
      		<br>
      		<h3>Computed Spectrograms to Histograms</h3>
      		<br>
      		
      		
    <table class="content-table">
        <thead>
          <tr>
            <th>Virtual Self - Duvet (LLFA Edit)</th>
            <th>Virtual Self - Tremor (Devon Remake)</th>
            <th>Aftershock & LXCPR - Party Like A Rockstar</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td><img src="../images/duvetspectrogram.png" style="width:100%;"></td>
            <td><img src="../images/tremorspectrogram.png" style="width:100%;"></td>
            <td><img src="../images/rockstarspectrogram.png" style="width:100%;"></td>
          </tr>
        </tbody>
      </table><br>
      
            <h3>Computed MFCC's to Histograms</h3>
      		<br>
      
         <table class="content-table">
        <thead>
          <tr>
            <th>Virtual Self - Duvet (LLFA Edit)</th>
            <th>Virtual Self - Tremor (Devon Remake)</th>
            <th>Aftershock & LXCPR - Party Like A Rockstar</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td><img src="../images/duvetmfcc.png" style="width:100%;"></td>
            <td><img src="../images/tremormfcc.png" style="width:100%;"></td>
            <td><img src="../images/rockstarmfcc.png" style="width:100%;"></td>
          </tr>
        </tbody>
      </table><br>
      
            <h3>Computed Chromagrams to Histograms</h3>
      		<br>
      
         <table class="content-table">
        <thead>
          <tr>
            <th>Virtual Self - Duvet (LLFA Edit)</th>
            <th>Virtual Self - Tremor (Devon Remake)</th>
            <th>Aftershock & LXCPR - Party Like A Rockstar</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td><img src="../images/duvetchromagram.png" style="width:100%;"></td>
            <td><img src="../images/tremorchromagram.png" style="width:100%;"></td>
            <td><img src="../images/rockstarchromagram.png" style="width:100%;"></td>
          </tr>
        </tbody>
      </table><br>
      
      <h3>Analysis</h3><br>
      
      <p>As someone that doesn't come from a music theory based background, I found that the histograms were helpful at figuring out significant differences between the tracks. For example,
      as all 3 are dance songs - a genre largely defined by melody and drums, I found prior to the task that there would be similarities. However, I decided to pick 3 tracks from 
      different subgenres of dance music. "Duvet" being a techno / trance track with a big melody and standard drums, where as "Tremor" has more of industrial influence with big drum parts. "Party Like a Rockstar" comes from Hardstyle
      where the melody is big as well as having a loud bassy kick. <br>
      <br>
      For this task, I've decided to analyse the MFCC Histograms. As all 3 tracks are from a similar genre, I expect to find some similarities in sound and frequency. As Duvet and Tremor were 
      originally produced by the same artists - Virtual Self, some of the features are very alike, such as the synth sounds. The MFCC graphs reflect that, being that they are similar in frequency - albeit, Tremor is a little more noise heavy
      due to the intensity of the track. As Party Like A Rockstar is very kick heavy, where most of the "peak" sounds would come from, I would expect that the sound would be a sharp drop, which the histograms above reflect.</p>
      		
		</section>
	</body>
	
</html>