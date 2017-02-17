# SeparatedAssetBundleBuild
Workaround for long time to build many AssetBundles.

Read this in other languages: English, [日本語](README.ja.md)<br />
日本語版はコチラを参照してください。

## about Issue
At Unity 5.5 , the build time of AssetBundle is increasing exponentially by the number of AssetBundle.<br />

Graph1.releation between the number of AssetBundles and building time<br />

Issue Tracker:<br />
https://issuetracker.unity3d.com/issues/drastically-longer-asset-bundle-building-time-when-building-multiple-small-asset-bundles<br />

## about this
This is a workaround project.<br />

To make the build time shorter, it is effective way to separate calling "BuildPipeline.BuildAssetBundles".

Graph2.this workaround
![Alt text](/doc/img/AssetBundleBuildTime.png)


### How to use this
1). Import the "SeparatedAssetBundleBuild.unitypackage".<br />
2). Replace "BuildPipeline.BuildAssetBundles" to "UTJ.SeparatedAssetBundleBuild.BuildAssetBundles".<br />


### About sample 
We prepared test case.<br />
Call "Sample/SampleWindow" from menu.<br />

![Alt text](/doc/img/SampleWindow.png) <br />
<br />
1)The number of datas.<br />
2).Create test datas.<br />
3).Build assetBundle without this workaround.<br />
4).Build assetBundle with this workaround.<br />

