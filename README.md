[![logo-fine-alpha-25.png](https://i.postimg.cc/B6sz8w5P/logo-fine-alpha-25.png)](https://postimg.cc/wtf2Z2G9)
# FiNE
CG render multi denoising Toolbox. 
Intel OID, Nvidia Optix & RenderMan Hyperion.
Release v3.31
https://github.com/ChristopheMoreau/FiNE/releases/tag/v3.31

# INSTALL
Unzip the FiNE_v3.30 folder.
Launch the FiNE_v3.30.exe.
Enjoy !
For NVidia Optix denoiser, Nvidia drivers must be updated. (at least version 436)


# Change Log
**v3.31**
You can now spool Intel & Nvidia denoiser job on Tractor. (More options will be available if needed)
Temporary files in the /temp folder are now deleted after each frame. (not at the end of the sequence)
Albedo and Normal aov will be merge with the filtered image if they are present in the original unfiltered image.

**v3.30**
- New Intel OID 1.4
- New UI
- FiNE will check at startup if the system variable **FINE_PATH** exist. 

**v3.24**
RenderMan Hyperion Denoiser :
- L’option crossFrame fonctionne à nouveau.
- Ajout d’une option “Clean Variance”, qui permet de renommer correctement les channels des différents layers d’une variance éditée dans Nuke. (Vous pourrez ensuite denoiser cette passe “clean”.

Le drop down menu des threads est toujours visible sur la fenêtre principale


**v3.2**
- Correction de crash si présence d’une “double beauty” (defaut RGB + Beauty)
- Possibilité de denoise les layers avec ou sans l’utilisation de la Albedo & Normal.
- Possibilité de denoise des images 8bits JPG ou PNG. (plus d’excuses de montrer des images noisées sur Ftrack…)
- Mémorisation des layers déjà sélectionnés.


**v3.1**
- Correction d’un bug qui pouvait ne pas denoiser l’image du layer defaut (RGB) s’il avait été sauvegardé par Nuke ou un autre moteur de rendu que Renderman.
- Possibilité de denoiser une image ‘single’ (sans padding) monImage.exr
- Correction d’un crash causé par la présence d’un fichier portant le même nom mais sans padding dans le même dossier que la séquence d’images à dénoise monImage.####.exr
- monImage.exr
- Décalage des fenêtres popup par Thread pour plus de lisibilité.
