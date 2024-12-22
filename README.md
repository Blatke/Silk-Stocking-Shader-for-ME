# Silk Stocking Shader for ME
A shader mod for HS2 / AIS MaterialEditor. It's based on [Blake/Silk Stocking Shader](https://github.com/Blatke/Silk-Stocking-Shader), which is a shaderlab coded shader in Unity.

## What is it?
It's for making an object more like a silk stocking. As shown in the screenshot, the shader is loaded to the material of the pants that a character is wearing. By default, the closer it is near by the bumps on the legs, the more transparency it will show so that the character's skins could be seen (it's what they called Fresnel effect).

![AI_2024-12-20-18-52-54-666](https://github.com/user-attachments/assets/fdee0098-611b-4d87-b249-45d2e11b1222)

## How to install it?
Download the .zipmod file for the latest version on the **[Release](https://github.com/Blatke/Silk-Stocking-Shader-for-ME/releases)** page, and drag and drop it into your game's **/mods/** folder.

## How to use it?
Better to see the demonstration video: https://youtu.be/vOt1-2O9gvc

> [!NOTE]
> Since this mod is updated, the names of some of the properties shown in the screenshot and the demonstration video above might be different.

Select an object such as clothes, pants, stockings, or something else in Studio or Chara Maker mode, open it on MaterialEditor tab, change a particular material's default shader to **Blake/Silk Stocking Shader/v1.0.5** (the specific version you got might be greater than 1.0.5), then the material is re-shadered and loaded with some default maps. 

Like in the demonstration video, you can adjust the parameters of the properties shown on MaterialEditor tab in order to get the material a proper performance. The properties are listed below: 

> [!TIP]
> The prefixes like _A__, _B__ or _C__ only serve for sequencing the properties on MaterialEditor tab. They're not meaningful.

### Maps
**MainTex** is empty by default, and it serves for only cutout. The transparent patterns or background of a image imported into this slot can cull the slik stocking.

**Normal** is empty by default, and it provides another normal map slot for you to import a custom texture for bump effect. 

**A_StockingAlbedo** loads automatically the default diffuse map of silk stocking.

**A_StockinglNormal** loads automatically the default normal map of silk stocking.

**B_WetnessBumpMap** loads automatically the default bump map for wetness.

**B_WetnessMap** loads automatically the default diffuse map for wetness.

**C_FluidMap** loads automatically the default the diffuse map for fluid.

**C_FluidNormal** loads automatically the default normal map for fluid.

### Colors
**A_Color** refers to the tint color of silk stocking.

**C_FluidColor** refers to the tint color of the fluid, if there is it.

### Parameters
**A_MainTexCutout** controls the strength of culling conducted by MainTex if there is semi-transparent patterns on the texture. Any values in the MainTex's alpha channel lower than A_MainTexCutout will let the silk stocking cull the corresponding parts.

**A_StockingNormalStrength** refers to the intensity of the bump effect that silk stocking's normal map can perform (A_StockingNormal).

**A_FresnelStrength** uses Fresnel effect that lets silk stocking have rims around its edges. Where there are more rims, stocking is more like opaque; where less, more like transparent and thus lets the object like skins behind the stocking can be seen through the stocking. This option controls the transparency of the rims.

**A_FresnelExp** refers to the width of the rims of silk stocking.

**A_FresnelEmission** lets the rims of silk stocking have light emission according to the tint color (A_Color).

**A_FresnelRevert** flips the rims from the edges of stocking to the center when its value is changed to 1.

**A_Glossiness** is the instensity of the smoothness with reflection the stocking can perform.

**A_Metallic** is the instensity of the metallic with reflection the stocking can perform.

**A_NormalStrength** refers to the intensity of the bump effect that your imported normal map can perform (Normal).

**A_TexDensity** refers to the density of silk stocking's diffuse map (A_StockingAlbedo). A greater value makes denser the "fishnets" on the map.

**A_TexLengthWidthRatio** means the ratio of the length to the width of the silk stocking's diffuse map (A_StockingAlbedo). Use it to make the "fishnets" on the map wider or longer.

**A_TexRotation** controls the rotation degree of the silk stocking's diffuse map (A_StockingAlbedo).

**B_WetnessStrength** lets there be wetness on silk stocking, and means to what extent the wetness's diffuse map (B_WetnessMap) can perform in its glossiness and metallic. 0 means no wetness at all.

**B_WetnessBump** decides the intensity of the bump effect that wetness can perform (B_WetnessBumpMap).

**B_WetnessDensity** controls the density of the wetness's diffuse map (B_WetnessMap). A greater value makes denser the wetness patterns on the map.

**C_FluidStrength** lets there be fluid on silk stocking (C_FluidMap). 0 means no fluid at all.

**C_FluidBump** decides the intensity of the bump effect that fluid can perform (C_FluidNormal).

**C_FluidColor** defines the tint color of the fluid.

**C_FluidDensity** controls the density of the fluid.

**C_FluidEmission** lets the fluid have light emission according to its tint color (C_FluidColor).

**C_FluidRotation** rotates the fluid to change its dripping direction.

## For modders
If you are modding for HS2 or AIS and would like to use this shader in your mods, you can download the .shader file as well as the .unitypackage pack on the [Blake/Silk Stocking Shader](https://github.com/Blatke/Silk-Stocking-Shader/releases) and import them as assets in Unity.

> [!IMPORTANT]
> If you allow the users to adjust your mods, using this shader, on MaterialEditor tab, you need to suggest them installing this shader mod so that the related options can be shown on the tab.

## Acknowledgement
I give special appreciation to [Hanmen](https://www.patreon.com/c/hanmen), who directly and generously helped me with modding this shader to let MaterialEditor in HS2 and AIS successfully load it.

I also thank kky-is, [Pizdatyi](https://www.pixiv.net/users/86387918), [Getdowncrazy](https://www.patreon.com/c/realillusionGDC/), [enimaroah](https://github.com/enimaroah-cubic/Sb3UGS/wiki) and ElusiveCake, who spent time in kindly replying to my questions about shader modding, and thus have brought me with enlightenment.
