# Optimizing CLS

## Using DevTools to view CLS score

Using devtools in chrome, we can view the CLS score by 

`DevTools > Lighthouse`

We need to select `Performance` as our metric.

After the report is generated, we can filter for all the elements which are contributing to CLS. And if we want to know in detail, we can use `View Original Trace` button.

Under the `View Original Trace` section, we have to select the checkbox for `Web Vitals` and `Screenshots`. After doing this, we can look for Layout Shifts in the `Experience` part and view the screenshots to see what is causing LS.


![Screenshot 1](/screenshots/1.png)
![Screenshot 2](/screenshots/2.png)