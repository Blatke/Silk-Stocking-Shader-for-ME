# Silk Stocking Shader for ME
A shader mod for HS2 / AIS MaterialEditor. It's based on [Blake/Silk Stocking Shader](https://github.com/Blatke/Silk-Stocking-Shader), which is a shaderlab coded shader in Unity.

## What is it?
It's for making an object more lika a silk stocking. As shown in the screenshot, the shader is loaded to the material of the pants that a character is wearing. By default, the closer it is near by the bumps on the legs, the more transparency it will show so that the character's skins could be seen (it's what they called Fresnel effect).

![AI_2024-12-20-18-52-54-666](https://github.com/user-attachments/assets/fdee0098-611b-4d87-b249-45d2e11b1222)

## How to install it?
Download the .zipmod file for the latest version on the **[Release](https://github.com/Blatke/Silk-Stocking-Shader-for-ME/releases)** page, and drag and drop it into your game's **/mods/** folder.

## How to use it?
Better to see the demonstration video: https://youtu.be/vOt1-2O9gvc

Select an object such as clothes, pants, stockings, or something else in Studio or Chara Maker mode, open it on MaterialEditor tab, change a particular material's default shader to **Blake/Silk Stocking Shader/v1.0.5** (the specific version you got might be greater than 1.0.5), then the material is re-shadered and loaded with some default maps. 

Like in the demonstration video, you can adjust the parameters of the properties shown on MaterialEditor tab in order to get the material a proper performance. The properties are listed below: 

**A_Color**
**A_MainTex**
**A_Glossiness**
**A_Metallic**
**A_Normal**
**A_NormalStrength**
**A_DetailNormal**
**A_DetailNormalStrength**
**A_TexDensity**
**A_TexLengthWidthRatio**
**A_TexRotation**
**A_FresnelExp**
**A_FresnelStrength**
**A_FresnelEmission**
**A_FresnelRevert**


**B_WetnessMap**
**B_WetnessDensity**
**B_WetnessStrength**
**B_WetnessBumpMap**
**B_WetnessBump**


**C_FluidMap**
**C_FluidNormal**
**C_FluidColor**
**C_FluidDensity**
**C_FluidStrength**
**C_FluidEmission**
**C_FluidBump**
**C_FluidRotation**

## Acknowledgement
I give special appreciation to [Hanmen](https://www.patreon.com/c/hanmen), who directly helped me with modding this shader to let MaterialEditor in HS2 and AIS successfully load it.

I also thank kky-is, [Pizdatyi](https://www.pixiv.net/users/86387918), [Getdowncrazy](https://www.patreon.com/c/realillusionGDC/), [enimaroah](https://github.com/enimaroah-cubic/Sb3UGS/wiki), ElusiveCake, who paid attention to my problems in shader modding.
