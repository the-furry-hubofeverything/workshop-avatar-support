# **Tank Weasel Manual**

> This manual assumes that you have knowledge about uploading avatars and a texturing workflow. 
> 
> If you have trouble with anything, please contact me with the information in the last section of this manual. 
>
> This manual is updated regularly on [avatardocs.gulo.dev](http://avatardocs.gulo.dev). It is licensed under CC0. Feel free to contribute!
>
> Thank you for supporting me by purchasing this avatar!  
> \- Hubble the Wolverine

## **Usage License**

- Due to this product being a digital product, refunds are NOT possible.

- If you are selling any customizations, modifications, or retextures of the Tank Weasel model, make sure that both you (the artist) and the customer own the model.

- Please don’t claim the Tank Weasel model (or its default textures and assets) as your own work.

- Please don’t resell, redistribute, or share any of the Tank Weasel files. 

  - If you are an asset creator, please find a way to distribute the changes on their own.

- Please ask before using this model for commercial purposes.

- Please do not use this model for anything related to Cryptocurrency or NFTs.

- Please ask before using this model for use in machine learning algorithms, or “AI”, especially (but not limited to) generative models.


## **Version guarantee**

As long as the major version of the avatar base stays the same (the first number of the version, like 1.x.x), the UV map and file structure of the project should stay the same.

If you see an inconsistency, please contact me with methods outlined in the last section of this manual.


## **Default Gesture/Expression mappings**

| Gesture | Expression |
|---------|------------|
| Neutral/HandOpen | Relaxed (non-emotive) face |
| Fist | Blep |
| FingerPoint | Sus |
| Victory | Happy |
| RockNRoll | Annoyed |
| HandGun | Shock |
| ThumbsUp | Smug/Annoyed |


## **Project setup**

Please refer to <https://creators.vrchat.com/sdk/> to set up VCC and the avatar project. VCC is strongly recommended for this avatar.

The tank weasel assets are based on **Unity** [**2022.3.22f1**](https://unity.com/releases/editor/whats-new/2022.3.22), and Blender 3.6 LTS. Blender is not required for uploading the avatar.

When setting up the project, open “default.scene” for a preconfigured scene. **It is strongly recommended to make a copy of this scene for customization.** 

The avatar is nested into the prefab. In the side bar, you’ll see “Tank Weasel > _Avatar_ > (contents)”. Avatar is where the avatar root (VRC avatar descriptor, blueprint ID etc.) is.   
![](https://lh7-us.googleusercontent.com/docsz/AD_4nXeSg4Vjb3MwL-YMtgTVWPFVRTg7KC0Jg2zziFcaEJWsWXnrD5xcJDvWAD8ehFYcL12TZ5gT41OSVTlE2BH2buvYsd4AjvIuocYVc32dwcl9mgCpYs4v-OdPD4OKdMYx2SymTNA8o42HjwW2rrGiRPQ4B3bG?key=leSC4NkGoMp6FWrTEOeY3Q)

Please do not unpack the prefab, as it will prevent the avatar from updating. The changes will be preserved as overrides to the prefab.

To view changes to the prefab from the default, select “Tank Weasel” and open the overrides menu from the inspector.

Here’s an example of this from the Tank Weasel public avatar:![](https://lh7-us.googleusercontent.com/docsz/AD_4nXdVb9MRmP5lZqz6m9KHvFazJ_umUOvIX-iQ_LjO-L_c1MbxA_awT_dGmERh9ppx8n5wb6WhWx_InGg4HBMWFB1BFmOFcYq9Uv-t8f4-QVgj3M-1io8dtPE4k6E9OHoLatXD_AM3FjDY3mt3dXCFqGgL2-hA?key=leSC4NkGoMp6FWrTEOeY3Q)


### Updating

The Tank Weasel is designed to be directly updatable. Just import the package and that’s it! 

**Make sure you uncheck any files that’s different from the default (i.e. Materials, animation controllers), or else those files will be reset to default.** It’s recommended to make a copy of the file you’ve changed so this won’t happen.

As mentioned in the previous section, all of the changes that you’ve made in the prefab (deletions, additions etc.) will be kept as overrides.


### Import prefabs and assets

#### Required dependencies

- VRCFury (<https://vrcfury.com/download>) (1.xx)


#### Recommended additions

- GoGo Loco (<https://www.gogoloco.net/>)

  - Adds sitting and prone animations. Strongly recommended for QoL.

- Poiyomi Toon Shader (<https://github.com/poiyomi/PoiyomiToonShader>) 

  - For Audiolink, better shading, rim lighting, glitter, and so on.

- VRCFT Jerry's Templates (<https://github.com/Adjerry91/VRCFaceTracking-Templates>)

  - _Required for face tracking._ 

  - Use the Unified Expressions VRCFury Prefab.

  - It’s recommended to remove the debug tools from the prefab for performance reasons.

Please refer to the documentation for these addons for installation instructions.


### Customization

#### UV map layout

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXekhzhcoBPXKvGy4j-CrlfhILsKHk8nx_ATK44Q08EYJlkQxpZ_t3pFxDyx89AW75OWKAiQ0FMj52SI7aSGnV2fNgz8q6CVIjhcxizvc-01uhUAj5ehJ-nzN8ZPqeGpl676Ps5cN_Jgx5UzIgj5Qs8uRHU?key=leSC4NkGoMp6FWrTEOeY3Q)

As long as the version of the tank weasel remains “1.x.x”, this UV map will stay consistent. If there’s any deliberate changes to the UV map at all, the major version will be bumped. 

If you spot any problems with the UV map, please contact me via the methods outlined at the last section of the manual.


#### Textures

The textures are under the “texture” folder. If a custom texture is used, it’s recommended to import the texture as its own file and then use the related import preset, like “albedo” for albedo textures.

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXcZtGlbXEbI_jRykMhZ0ugwI9e0qBMyLhLLcCd2VjkN-caLGHdfySD7u9E55awzzashoMvYbeGCjfOO_BoWhPLN1QSrEA_BI7_k9CMQapRTneUVrpQnNESquUC3oBTTW3qImTXouTaL3NY4T0NCUyNwGk1x?key=leSC4NkGoMp6FWrTEOeY3Q)

#### Materials

The materials are under the “Materials” folder.

There are both PC and Quest versions of the material (Quest versions end with \_Quest). The PC version is using the Unity standard shader, which is chosen to reduce dependencies needed. If features like audiolink, more shading options, glitter, and so on are desired, you can add the Poiyomi toon shader to the project.

For the Unity standard shader, a metallic smoothness map (with smoothness being the alpha channel of the metallic map) and a normal map is included.


#### Maker card

To remove the maker card, expand the prefab, and find the maker card under Armature > Hips > Spine > Chest > maker card, and delete it. 

The texture is imported with a resolution of 512x512 to minimize performance impact.

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXcnj6z6Cvz2fd4ET0vDM8_N8MYJmVDEq7hflIVC8I5JJzYP4iSeOQhYde4AVDFRag8RvwoOuVBLmJ5vuwX8yFl0kZCdMHMfoYRkKrlzWz0_4dn3SiXdEJGwnebnkdrGIXGtCdfNatBRiM9KcP3U5_ak9eQ2?key=leSC4NkGoMp6FWrTEOeY3Q)


#### Physbones

There are Physbones for the ear, the belly, and the tail. The Physbone settings are separated out using empties for ease of use. 

Remember to update the physbone components on the Quest version to make sure that the settings remain the same on both versions.

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXewWeL7ZncmiDSHpPTRvRk7gG81f-VjQtwNoL8UqItEkjkb_TAmBwnrj6SkbTX68kzRk6BKnefzTuw4g2rfhqaLI5VttLMZSitRzkygCXxFe2xUZFdHfYGA9vIivTHqu5TFjEi-cgNZD-H0aZwC7-OYEnO-?key=leSC4NkGoMp6FWrTEOeY3Q)


#### Gestures and Expressions

The tank weasel uses custom FX and gesture layers for its expression and gestures, under Assets > Animation > FX.

The reason that the tank weasel doesn’t use VRCFury gesture components is because of a limitation - At the time of making, it doesn’t include a toggle where you can prevent gestures from triggering expressions. I’ve included this toggle under “Expressions > Settings > Lock Face” in the radial menu.

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXcDA8XbMymX9UKDwUOR91rIIrB_58-2LrhGxPVGARE3tlg5JUn1qfqp3zDNMjjUkadAuHC_1EqgUVak-Hjh1dXh4m2T2tHQ7Seq6nMFmFC-hapd5hFcF6POWQux1ZBgJWRJu9NqoasB4oFH4aoYgTAL1bh7?key=leSC4NkGoMp6FWrTEOeY3Q)

All expression clips are under Assets > Animation > Clips > Expressions, animated using Unified Expression blendshapes. There are no dedicated blendshapes for specific expressions.


##### Automatic Thumb Detection

The automatic thumb detection is a system that is added in the “Expressions” empty. It consists of VRC contact receivers parented on the elbow bone, contact senders on the thumb, and the blend tree in the gesture layer.

When you perform a thumbs up, the thumb would be touching the contact receiver, making a smug expression by default, and vice versa. The elbow receiver stays in place while the wrist/hand bone rotates.

You can lock this detection by going into “Expressions > Settings > Thumb Detection Mode”, where you can force the thumbs up/down expression.

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXeC0BjxoqPZBCXP0l-TpJ9hRGvhW8l2nUqeQJ95Wa4MQ2-43NXTREgHstoRk-qaRXN5Ip0AmFACbW_kQpix2MUnJ__tALVH73QGTRZEng2tgZKTy90hdR0VatpTlEhEh3KZkBmzqiHXK4j3EkfctdFkMkM?key=leSC4NkGoMp6FWrTEOeY3Q)

In the FX layer, the automatic thumb detection is implemented in the “ThumbsUp” state in each hand’s animation layer.

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXciYBHhdp3owgVEA4tKz0g_5Vq0H6fVLxptbvGpCZW44ESp32TmGf_ZURYxqb8t678AYnZ5CvEKh2ahp8znUWXhb1hvuE2UEAgTMeqGWeG0ksQiPUwdnm-7vd9vYGslJfip6NMIYyxk2y1jhcEf5ntaaPSg?key=leSC4NkGoMp6FWrTEOeY3Q)

Inside is a blend tree, which looks like something like this:

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXc5GM85WwWRDkZakq55YsGe9zcwcGxrk4X2iVYKC9VAyKfCD2C6HX514NJ-XmiBrQqvDKE-ktSKEMzK1T3dPiLWbtBprNhtLQqTKewjTCq1EcWUwRbNe9SpRikhooUjNYkeFv3sMZdeOWBaiEvYXcdypNp6?key=leSC4NkGoMp6FWrTEOeY3Q)

It takes two parameters as input - ThumbMode and ThumbsUpL/ThumbsUpR. 

ThumbMode is the thumb override parameter.

- 0 turns automatic thumb detection on

- 1 forces the thumbs up expression

- 2 forces the thumbs down expression

ThumbsUpL/R represents the distance that the thumb contact sender is to the receiver if it was touching (“Proximity” Receiver type).

- 0 is away from the contact (thumbs down)

- 1 is in the center of the contact (thumbs up)

TL;DR - You can replace the thumbs up/down expression by replacing the corresponding clips: “Smug” for thumbs up, “Angry” for thumbs down.


##### Nose lick

When enabled, the animated tongue will have the model lick its own nose every \~30 seconds. You can disable this by going into Expressions > Settings > Nose Lick under the radial menu.

The nose licking behavior is controlled by the “Nose Lick” layer in the FX animation controller. By default, it will pause licking when GestureLeft or GestureRight is fist, since it corresponds to a tongue out expression. Other expressions that pause the nose lick animation are Raspberry and Pog. 

To create a custom expression that pauses the nose lick behavior, set the FX float “PauseNoseLick” to 1.


##### Body Settings

Most of the body settings should be saved and available via the “Body” menu. 

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXfYyzVpXj2T6k84fWXjbVCS2-c1XJuEBvrlZIeM05RcoCDHTUIvibLYs6sOy_Oc56z6kflxutzX9Vuyo9zRIu35-WTHtvcrdpijjzzay85noZimBucikjLX5q17djd9YY4Fio--k_Em7e91xPXsAK_XJWYI?key=leSC4NkGoMp6FWrTEOeY3Q)

The idle animation blend tree (for breathing, twitching etc) is located inside the FX controller, under the base layer.

It’s not recommended, but if you want to “lock in” some blendshapes for optimization, you can do so via Blender (see “exporting model”). Make sure to remove the subsequent menu option from the “Body Control” empty. 


#### Pooltoy mode (experimental)
> [!WARNING]
> This will add a new skinned mesh to your character, dropping its performance ranking.

To add pooltoy mode, simply drag the prefab (Assets/Pooltoy Mode/Pooltoy mode) to the avatar root ("Avatar", not "Tank Weasel"), then let VRCFury do the rest.

To change what the pooltoy material is based on, change the parent of the material (below "Shader") to the QUEST version of your body material. This will ensure quest compatibility.

If you made a duplicate material for editing, you also must edit the animation clip, by assigning the FX animation controller to the avatar root, drag the animation clip into the controller, and then assign the new material to the animation clip to set it up as a key. If you made a duplicate of the animation clip, make sure to switch the clip out in the prefab as well.

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXflwVDfwi0l7a7dSl4zmY4-E6-0cdp3vZieOS2JlzFrl58M5-iVEWOfg02QVsaW6JM3ozaT1lT4JNp8sJhAl34CW3nJHyjAu-Z-3Ahs5ROPmF4O2iTZFSI3GwyXkSKJutJ4XcGcW1iny2qeSiJ6nFg82W__?key=leSC4NkGoMp6FWrTEOeY3Q)

Make sure to override both keys on frame 0 and frame 1, or it will flicker between the original material and the edited one.

_If you have a more user-friendly way of doing this, please contact me via methods outlined in the last section of this manual._


## **Files**

> [!IMPORTANT]
> As most of my software stack in my workflow is open source, I’m unable to provide Substance Painter or Photoshop files.  
>  
> Krita is able to export files as psd, but [photoshop files are not an open standard and are very hard to work with](https://docs.krita.org/en/general_concepts/file_formats/file_psd.html). YMMV


### Included files

| Folder/File name | Description |
| --- | --- |
| textures | See [Textures](#textures-1) |
| `<version number>`.blend file | Blender (3.6+) file for mesh editing and texturing. <https://www.blender.org/download/lts/3-6/> |
| Pooltoy Parts.fbx | fbx file for the pooltoy nozzle and handles, includes blendshapes to adjust to the main model. |
| TankWeasel-`<version number>`.unitypackage | Contains Unity Scene, prefabs, and assets for VRChat. |
| tankWeasel.fbx | fbx file for the main model. |
| tankWeasel_Quest.fbx | fbx file for the Quest version of the main model. |
| TexturePadding.blend | Blender file for [Texture dilation/padding](#uv-paddingtexture-paddingtexture-dilation) |
| texturePostProcessing.kra | Krita (5.2+) file for texturing. <https://krita.org/en/download/> |

### Textures 

| Folder/File name | Description |
| --- | --- |
| Masks | These textures are not necessary for the avatar to work, but may be useful for texture creation, baking, and filtering specific parts of the avatar.|
| Generic | Albedo and flattened default texture map of the “Generic” variant. |
| Forest | Albedo and flattened default texture map of the “Forest” variant. |
| Spirit | Albedo and flattened default texture map of the “Spirit” variant. |
| AO.png | Ambient Occlusion map. |
| MetallicSmoothness.png | Metallic smoothness map for default Unity shaders. |
| Normal.png | Normal map that adds the bumpiness on the nose, mouth, and paws. |
| Smoothness.png | Smoothness map for other shaders that are not compatible with metallic smoothness maps. |


## **Texturing**

_Shameless self promo: If you like to commission me for a retexture, check_ [_https://gulo.dev_](https://gulo.dev) _for the status and pricing of my retexture commissions!_

> [!IMPORTANT]
> With certain shape keys (like feminine, pooltoy and the chub slider), the texture will be slightly distorted. It’s recommended to texture the model with the shape key at the desired value.

The texture files and fbx file are provided in the package for setting up your own workflow. See the “Files” section above for file descriptions.

A Blender file is provided for Blender specific workflows, such as mesh editing or texture painting, but it isn’t necessary.

If you want to customize the eye color, or add ambient occlusion to the texture, you can use the Krita file. 

A UV layout overlay is included in the krita file for 2d texturing workflows. The UV map is the same for both the Quest and the PC version of the mesh.


### UV padding/texture padding/texture dilation

A blender file “TexturePadding.blend” is included in the package. 

The image file must have a transparent area for the area being filled.

To use it, make sure the resolution in the render settings is set to the desired dimensions (4096x4096 is set for default for albedo textures), then render!

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXetjisQJzeWgcmS1CV_g_6320Sb6uobeXEkC3H5lXw4j7zUUBlhlpoHZZP1jcN7e4K41anzZGfw2zTwqzT5aqr_eHMMsDHVjOVaJdxMOblhJ1VAuwEU2xSJzhu5fcW_ZvkK3Xwe0LpOIA2DzsfF0sht46pY?key=leSC4NkGoMp6FWrTEOeY3Q)


### Example workflow

1. Make the albedo (color) texture in a software of your choice. You don’t have to texture the eyes or the nostril.

2. Open the krita file (file ending in .kra)

3. Replace “textures/Albedo.png” with your own albedo texture
   - _Note: if you want to use a different file path, change the file path under layer properties._\
   ![](https://lh7-us.googleusercontent.com/docsz/AD_4nXdzG6FkqueMuHjWZm3E-UG2oUs5N8-cS6wyrD4aVemJ_LXlrY4aCR_hNMqYalNVPUzn4VSuHqSdmL7brM-VpYP4sUWhgtXZdEHhdWUsNZ-gEh8HREzgjIOBNm0ZODjneS0h4s66t7bcc9DYZjL3mw6dtDQL?key=leSC4NkGoMp6FWrTEOeY3Q)

4. Change the color of the iris, pupil, and the Sclera (white part) of the eye by going into layer properties of each of the fill layers. 

   - If painting is needed, you can right click the layer, go to ‘convert’ and convert the layer to a paint layer.

5. Export the file as an PNG, and import it into the Unity project. (see the “Project setup” section for specifics.)


## **Exporting model**

**!!! IMPORTANT !!! You do not need to use Blender to upload or customize the texture of the Tank Weasel. See “Project setup” or “Texturing” for more information.**


### Customizing model  

When customizing the model itself, make sure to make the changes to the PC model (Body) instead of the Quest model (Body\_Quest). Read the previous section for more details on how to switch between them.

With the PC model, there’s a bunch of highlighted green lines that are marked on the model. Those are freestyle edge marks, but they are not used for that purpose. _Those highlighted loops are the difference between the PC and the Quest model._

When you are finished with the changes, simply duplicate the model, select one of those edges, and then go to Select > Select Similar > Freestyle Edge Marks to select all of the marks.

After selecting all the marks, dissolve the edges by pressing “X” and then “Dissolve Edges”.

This is done to preserve shape keys and UVs on both variants.
![](https://lh7-us.googleusercontent.com/docsz/AD_4nXcsIx6My23x3V326VQDPNqHPNnGBXjwLXmX8i2RBTtZnY0q6BzPYZdlTa69JY4lF64fZqxsEa0OM0fx028v0dj0dz1EUMIWOFoRXxJeOHU4_6gEOFAOp-E3XBfkwe4ZN_ol2zdNXWgCPtXvPdV6R1MZ3bht?key=leSC4NkGoMp6FWrTEOeY3Q)


### Quest model  
![](https://lh7-us.googleusercontent.com/docsz/AD_4nXcRI6yOigbMvJmXAx2N6obB4Evy80UbP3odv8tPCyOD4KYHasQDtdUIU82vZCI09YeTVKTt-TEC9QAaJG_zUulIXVTEMOeTeXAlavYkgj-DbkOK5NArxShK_2tYjflXavCkAcSOa16ZP6PBjOeYLE-Zi7Kz?key=leSC4NkGoMp6FWrTEOeY3Q)

The Quest version of the model is included in the .blend file. To select it, simply go to the mesh menu on the sidebar, and then change the mesh from “Body” to “Body\_Quest”.

This is done to preserve the hierarchy structure for custom animations, MMD etc.


### FBX Export  
![](https://lh7-us.googleusercontent.com/docsz/AD_4nXcgII1_33qZNY8YWvAR-DSlNh5YoyRdeEPts_6KLekkFckHjcjGxwhZi13-E6uDAgfw5CLNTOTRp4hby6iq9I9xK3HJcNfgIxDOvtChvwYzmN0PEg_FwVgj__bQcgq0GPUun2dRf505Y8-IxPnHVvadMXy6?key=leSC4NkGoMp6FWrTEOeY3Q)

**Select “Armature” and “Body”,** and then make the following changes to the FBX export settings: 

- Turn on “Selected Objects” 

- Transform

  - “FBX All” under “Apply Scalings”

- Armature

  - Turn off “Add Leaf Bones”.

- Turn on Bake Animation


### VRM Export

Since the Tank Weasel uses VRCFury primarily, the avatar from the scene cannot be directly exported as an VRM. However, you can try [this method](https://www.youtube.com/watch?v=XMQ43O65TXo) to make a compiled copy of the avatar. (Build VRCFury Test Copy)

This method is not officially supported, but if it works, please let me know (contact information is at the last section of this manual).


## **Acknowledgements**

> My deepest appreciation for the following people, the Tank Weasel wouldn’t be the model that it is without them:
> 
> Bionic the Weird, for sharing some artistic notes and references that informed the shape of the model.
> 
> Fractarine, Freeborn, Fane, Tong, Cliff, Ozlo, Arlow, Pioneer, and Steele for providing feedback and helping with beta testing.
> 
> Haydy Zeth, Midnightweasel and Spitly for helping me make the ‘feminine’ shape key. I’m not good at feminine anatomy.
> 
> Simmer22, bigdaddyrhino and ectoimp for advice on packaging and UX design.
> 
> Bluefish, Tox, Voxian, ZealotDKD, and others in the Virtual Limb Discord for advice and company while packaging the avatar.
> 
> Hiyu, who also inspired some design/packaging decisions from their work in the longboi.
> 
> Ludwig Göff, for providing many facts about wolverines and feedback on the model.
> 
> Tresch, Ella Fox, Vivi, Kay Ohtie, and others in the Furry VRChat Creators telegram chat, for helping me with troubleshooting Blender and Unity.


## **Contact**

Most of my contact information is on <https://gulo.dev>

Feel free to ask questions about implementation or usage specific details!

Email: <hubblethewolverine@gmail.com>

Telegram: <https://t.me/hubofeverything>
