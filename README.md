[logo-fine-alpha.png](https://i.postimg.cc/HnZf5430/logo-fine-alpha.png)

# FiNE
CG render multi denoising Toolbox. 
Intel OID, Nvidia Optix & RenderMan Hyperion.
(**F**inal **I**mage **N**oise **E**radicator)


# INSTALL
Copy the "Denoiser" folder on the C:\ (root level).
Copy FiNE_v3.24.exe where you want.
Enjoy !
For NVidia Optix denoiser, Nvidia drivers must be updated. (at least version 436)


# Change Log
Change Log **v3.24**

RenderMan Hyperion Denoiser :
L’option crossFrame fonctionne à nouveau.
Ajout d’une option “Clean Variance”, qui permet de renommer correctement les channels des différents layers d’une variance éditée dans Nuke. (Vous pourrez ensuite denoiser cette passe “clean”.

Le drop down menu des threads est toujours visible sur la fenêtre principale


Change Log **v3.2**

Correction de crash si présence d’une “double beauty” (defaut RGB + Beauty)
Possibilité de denoise les layers avec ou sans l’utilisation de la Albedo & Normal.
Possibilité de denoise des images 8bits JPG ou PNG. (plus d’excuses de montrer des images noisées sur Ftrack…)
Mémorisation des layers déjà sélectionnés.


Change Log **v3.1**

Correction d’un bug qui pouvait ne pas denoiser l’image du layer defaut (RGB) s’il avait été sauvegardé par Nuke ou un autre moteur de rendu que Renderman.
Possibilité de denoiser une image ‘single’ (sans padding) monImage.exr
Correction d’un crash causé par la présence d’un fichier portant le même nom mais sans padding dans le même dossier que la séquence d’images à dénoise monImage.####.exr
monImage.exr
Décalage des fenêtres popup par Thread pour plus de lisibilité.
