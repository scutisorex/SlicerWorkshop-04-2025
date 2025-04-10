# Slicer modules: Visualization, segmentation, and exporting meshes

Let's look at some of the important modules in Slicer using one of the sample volume data sets we just opened. If you have your own volumetric data, you can also try importing it now, in whatever format you have (DICOM or image stack; save your surface scanned models until a little later!). You can also try importing and working on [this volume data](https://drive.google.com/file/d/1LLCsZEND9LMf83WInAXXjp7WM_6t5HRd/view?usp=sharing), which you may recognize from earlier today. Open your data set in each one of these modules and see what you can do with it. 
 
Some modules to check out:
- [Volume Rendering](https://github.com/SlicerMorph/Spr_2021/blob/main/Day_2/VolumeRendering/VolumeRendering.md): This is the basics of how to view and customize your volume.
- [Transforms](https://slicer.readthedocs.io/en/latest/user_guide/modules/transforms.html): It's often useful to be able to reposition your object in the scene. Maybe you want to arrange it so its anatomical axes are aligned with those of the scene, or move it closer to another object, or rotate it relative to a markup of some kind. Whatever! Try making and hardening some transforms.
- [Animation](https://github.com/SlicerMorph/Spr_2021/blob/main/Day_2/SlicerAnimator/SlicerAnimator.md): Fundamentals of how to make a little movie of your item.
- [Lighting](https://github.com/SlicerMorph/Spr_2021/blob/main/Day_2/Lighting/Lights.md): This is an additional tool to make your volumes look nice. It's in an extension called **Sandbox**. If you don't have it installed, this is a great opportunity to practice installing a new extension!

**HOT TIP!** To navigate to a module, you can use the search box or the drop-down menu in the box with the name of your current module. You can also hit **CTRL+F** and it will open the Module Finder. Directly to the right of the current module is another drop-down that will show you module history, so you can go back to recent modules. The green arrows to the right of that are like the back and forward buttons on a browser; e.g., the back (left) arrow will take you directly to the previous module you were in.

## Segmentation and related explorations

Now it's time to learn one of the most important functions in Slicer: segmentation. This is where you separate an image into different parts and label them. In this case, we will be labeling a 3D volume, which consists of a whole bunch of 2D images. If this is your first time ever segmenting, or if you want more in-depth info or a refresher, check out [the official Slicer segmentation documentation.](https://slicer.readthedocs.io/en/latest/user_guide/image_segmentation.html) It's super informative and clear.

- Before you start segmenting, make sure you have the Sandbox extension installed. This will allow you to use the [Segment Editor Extra Effects](https://github.com/lassoan/SlicerSegmentEditorExtraEffects), which are extremely useful. They are covered in the tutorial below. Also install the [SurfaceWrapSolidify](https://github.com/sebastianandress/Slicer-SurfaceWrapSolidify) extension! 

- There are an absurd number of different ways to approach segmentation, and we can't cover all of them. However, we can get through the basic functions in Slicer using [this excellent tutorial put together by the SlicerMorph team.](https://github.com/SlicerMorph/Tutorials/tree/main/Segmentation) Work through it at your own pace, and try to experiment with as many of the tools as you can. They show their examples with the "MRBrainTumor1" sample data set, but you can test out the segmentation tools on any of the data sets we have looked at so far, or any of the data sets in the Sample Data module. Or, if you have your own data with you, feel free to use that!

- I would also encourage you to take a look at the descriptions of segmentation tools in the official Slicer [Segment Editor documentation](https://slicer.readthedocs.io/en/latest/user_guide/modules/segmenteditor.html).

- After you've done some segmentation, try out the [Colorize Volume](https://github.com/SlicerMorph/Tutorials/tree/main/ColorizeVolume) module, which is in the Sandbox extension we installed above. It makes stunning 3D renderings of the volume with color labeled by segment. You're gonna like it, I bet. 

- Obviously making your stuff look pretty is important, but you can also take important measurements on segments. Try out the [Segment Statistics module](https://slicer.readthedocs.io/en/latest/user_guide/modules/segmentstatistics.html) to get some quantitative info about the segmentations you make.

## 3D Mesh tools

Slicer is not incredible as a mesh editor, but you can accomplish some basic stuff that you're likely to need. 

Import the 3D mesh of a shrew vertebra listed above and try out some of the functions in the [Surface Toolbox](https://slicer.readthedocs.io/en/latest/user_guide/modules/surfacetoolbox.html) module. I have found the smoothing and mirroring tools to be especially useful for my work!

ALSO - there are a number of extensions available for doing specific edits to meshes. Try and see if you can find one by going to the Extension Manager and searching "mesh".