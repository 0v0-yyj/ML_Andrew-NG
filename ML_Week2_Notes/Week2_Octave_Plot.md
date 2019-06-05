## Plotting Data

1. * __plot (x,y)__  :point_right: _plot y versus x_
2. *  __hold on__
   *  __plot(X,Y)__ :point_right: _hold current plot (x,y) and plot new curve (X,Y) with different color in the sampleplot._
3. * __xlabel('')__
   * __ylabel('')__ :point_right: _give labels to x and y axises_
   * __legend('','',...)__ :point_right: _repectively add legend to each curve_
   * __title('')__
4. * __print -dpng 'filename.png'__ :point_right: _save png file in current directory_
5. * __close__ :point_right: _close current figure_
6. * __figure 1; plot(x,y1)__
   * __figure 2; plot(x,y2)__ :point_right: _figure 1 and figure 2 windows simutaneouly popup instead in one figure_
7. * __subplot(1,2,1)__ :point_right: _devide plot a 1x2 grid, access 1st element_
   * __plot(x,y1)__ :point_right: _fill this plot into 1st place_
   * __subplot(1,2,2)__ :point_right: _devide plot a 1x2 grid, access 2nd element_
   * __plot(x,y2)__ :point_right: _fill this plot into 2nd place_
   * __axis([0.5 1 -1 1])__ :point_right: _set plot(x,y2) x-axis range 0.5to1, and y-axis range -1to1 :fire: __used to set closer plot axises ranges__
8. * __clf__ :point_right: _clear the current figure window_
9. * __imagesc(A)__ :point_right: _plot a matrix row x col grid of color, differetn color represent different values_
   * __imagesc(A), colorbar, colormap gray__ :point_right: _plot a matrix in image and colorbar in colormap grey_
10. * __a=1,b=2,c=3__ :point_right: _comma chaining of commands/function calls %excute three commands at the same time, print 3 results_ 
    * __a=1;b=2;c=3__ :point_right: _multiple commands on the same line_
