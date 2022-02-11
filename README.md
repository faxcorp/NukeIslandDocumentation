# NukeIslandDocumentation
Nuke Island Project Unreal Marketplace Docs

To fix any Virtual Texture glitches (flickering and stuff) be sure to edit your engines "BaseEngine.ini" Virtual Texture parameters to enlarge the memory pool:

![image](https://user-images.githubusercontent.com/37246339/153584612-80383bf9-90bd-4e24-b1e4-997ba90f9d66.png)


To merge Nuke Island project to an existing project do following steps:

![defaultengine](https://user-images.githubusercontent.com/37246339/152350199-2402eac2-141f-459a-bcf1-820f3db28a87.jpg)
1. Edit DefaultEngine to have this line 
```r.Streaming.PoolSize=2048```
or you can make it 1024, it means your game will have 1gb minimum video card ram requirement





![projectsettings](https://user-images.githubusercontent.com/37246339/152350202-a528493e-0257-40fe-b755-d7cf071e7976.jpg)
2. Enable virtual texture support in project settings 







![plugins](https://user-images.githubusercontent.com/37246339/152350204-626f51af-610d-4b3b-add2-085cb2b05814.jpg)
3. Enable Virtual Heighfield Mesh plugin


4. Copy "NukeIsland" folder to your game projects "Content" folder
