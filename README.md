## Metro station locations and Capital Bikeshare ridership

Click [here](https://github.com/dandtaylor/MetroShare/blob/master/Analysis_metro_bikeshare_commuters.ipynb) to download my analysis notebook where all of my code is shown

the new [map of the redline stations used in analysis](map_red.html)!

<div style="text-align:center"><img src ="weekday_v_weekend.png" /></div>


![Weekday vs weekend ridership](weekday_v_weekend.png)

<a href="metro_nearbikes_map.html
" target="_blank"><img align="middle" src="metro_nearbikes_map_image.PNG" 
alt="Map!" width="346" height="269" border="10" /></a>

```python
fig, ax = plt.subplots(figsize=[6, 4])
ax.set_ylabel('Average number of rides per hour per day')
ax.set_title('Capital Bikeshare Weekend Ridership')
(bikeshare_weekend.groupby('Hour')['Hour'].count() / weekend_days).plot(kind='bar',alpha=0.5, color='r', ax=ax)
plt.show()
```
#### Complete analysis
Click [here](https://github.com/dandtaylor/MetroShare/blob/master/Analysis_metro_bikeshare_commuters.ipynb) to view my jupyter notebook with my complete analysis

#### Data sources
[WMATA api](https://developer.wmata.com/docs/services/)  
[OpenDataDC](http://www.opendatadc.org/dataset/wmata-disruption-reports)  
[Capital Bikeshare](https://www.capitalbikeshare.com/system-data)  


Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/dandtaylor/MetroDelayBikeShare/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
