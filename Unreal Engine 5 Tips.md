Doing UE5.0 preview developmental testing, valued discord user mindframes#3572, unveiled various UE5 caviats concerning rendering issues as follows:


1. If you run in VR, in some configurations you may notice all water surfaces seemingly flickering -- check to see if the left eye is rendering differently from the right eye. If they are showing different things, [turn off Instanced Stereo](https://forums.unrealengine.com/t/4-26-water-system-in-vr-havent-gotten-it-to-work-properly-yet/155231/3).

2. For Unreal Engine 5 setup, the changes to BaseEngine.ini are different from those in UE 4.27.
In BaseEngine.ini, in the section [/Script/Engine.VirtualTexturePoolConfig]:
```[/Script/Engine.VirtualTexturePoolConfig]
; SizeInMegabyte from 64-256 have been tested and work. 64 may cause some visible texture loads. Numbers above 3000 will cause severe problems in rendering the landscape or even make it invisible, even on an Nvidia 3090.
+Pools=(SizeInMegabyte=256, bAllowSizeScale=False, bEnableResidencyMipMapBias=True)```
