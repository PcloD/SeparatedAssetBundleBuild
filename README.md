# SeparatedAssetBundleBuild
Workaround for long time to build many AssetBundles.

## �������Ă�����ɂ���
Unity 5.5�ɂāA�r���h�Ώۂ�AssetBundle����������Α�����قǁA�r���h���Ԃ��w���I�ɒ����Ȃ�Ƃ�����肪�N���Ă��܂��B<br />

�}1.AssetBundle���ƃr���h���Ԃ̊֌W<br />

![Alt text](/doc/img/AssetBundleBuildTime.png)

Issue Tracker:<br />
https://issuetracker.unity3d.com/issues/drastically-longer-asset-bundle-building-time-when-building-multiple-small-asset-bundles<br />

## ���̃v���W�F�N�g�ɂ���
���̃v���W�F�N�g�́A"BuildPipeline.BuildAssetBundles"���\�Ȍ��蕪�����ČĂяo�����Ńr���h���Ԃ�Z�k���邽�߂̃v���W�F�N�g�ł��B

### �g�p���@
1). SeparatedAssetBundleBuild.unitypackage ���C���|�[�g���܂��B<br />
2). �v���W�F�N�g���ɂ��� "BuildPipeline.BuildAssetBundles" �� "UTJ.SeparatedAssetBundleBuild.BuildAssetBundles" �ɒu�������Ă��������B<br />


### �T���v���ɂ���
�e�X�g�p�ɃT���v����p�ӂ��܂����B<br />
Menu��"Sample/SampleWindow"���Ăяo���Ă��������B<br />

![Alt text](/doc/img/AssetBundleBuildTime.png) <br />
<br />
1).�e�X�g�Ɏg�p����A�Z�b�g�o���h�������Z�b�g���܂��B<br />
2).�e�X�g�p�̃f�[�^���쐬���܂��B<br />
3).�]���̂�����AssetBundle���쐬���܂��B<br />
4).����p�ӂ������@�ŁAAssetBundle���쐬���܂��B<br />


