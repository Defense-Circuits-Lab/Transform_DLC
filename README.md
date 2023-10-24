# Easy transformation and scaling of DeepLabCut Data
DeepLabCut is a widely used markerless pose estimation toolbox in behavioral science. The output of DeepLabCut is coordinates in pixels for each frame for each marker. However, in most cases the coordinates first need to be translated (i.e. adapted to the coordinate-space of the behavioral maze) and scaled (e.g. to cm) to enable meaningful behavioral quantification. Notably, the code in this repository is basic and an implementation of translation as well as scaling as an optional function in the DeepLabCut toolbox itself would be a better solution then running yet another modul in data preprocessing.

The Transform_DLC repository takes care of this specific task: It takes DeepLabCut dataframes as the input and outputs transformed and scaled DeepLabCut dataframes. Requirements for this transformation and scaling are that the behavioral maze or a reference has to be rectangular and its corners have to be tracked with DeepLabCut.

Parameters of Transform_DLC are the names of the origin, horizontal and vertical basis vector markers, as well as the minimal needed likelihood for those markers to be included in the position estimation. If scaling is desired, horizontal and vertical scaling factors have to be specified, too.



This is a [Defense Circuits Lab](https://www.defense-circuits-lab.com/) project written by Michael Schellenberger.
<table>
<td>
    <a href="https://www.defense-circuits-lab.com/"> 
        <img src="https://static.wixstatic.com/media/547baf_87ffe507a5004e29925dbeb65fe110bb~mv2.png/v1/fill/w_406,h_246,al_c,q_85,usm_0.66_1.00_0.01,enc_auto/LabLogo3black.png" alt="DefenseCircuitsLab" style="width: 250px;"/>
    </a>
</td>

</table>
