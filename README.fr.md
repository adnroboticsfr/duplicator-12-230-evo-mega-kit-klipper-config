# Duplicator 12 230 EVO MEGA-KIT klipper config
[![Français](https://img.shields.io/badge/langue-français-blue)](./README.fr.md)

Printer.cfg et firmware pour d12-230 evo mega-kit avec une carte 0327001-V3.0 et drivers TMC2225.

# **Guide d'installation du Klipper pour le D12-230 Evo Mega-Kit**

![D12-230 EVO MEGA KIT](img/D12-230_EVO_MEGA-KIT_1.png)

### **Avant de commencer : Important à savoir**
Cette procédure d'écrit comment installer Klipper sur votre imprimante 3D. Suivez chaque étape avec attention, car une erreur pourrait endommager votre matériel. Le processus a été testé, mais vous en êtes responsable. Assurez-vous de bien comprendre les instructions avant de commencer.

### **Matériel requis :**
1. **Pad** préconfiguré (connecté à votre réseau Wi-Fi ou via un câble Ethernet).
2. **Câble USB Type A mâle vers Type B mâle** (privilégiez un câble blindé pour minimiser les interférences).
3. **Carte MicroSD** pour mettre à jour le firmware.

### **Étape 1 : Télécharger le firmware**
1. Téléchargez le fichier **`Robin_nano.bin`** ainsi que le fichier de configuration **`printer.cfg`** dans le dossier **BL TOUCH** si votre imprimante 3D dispose du BL TOUCH (3d Touch) ou sinon NO BL TOUCH.

   <img src="img/D12-230_EVO_MEGA-KIT_2.png" alt="NO BL TOUCH or BL TOUCH" width="300">


### **Étape 2 : Mettre à jour le firmware de l’imprimante**
1. Copiez le fichier `Robin_nano.bin` renommé à la racine de votre carte MicroSD. Il ne doit avoir aucun autre fichier que le fichier  `Robin_nano.bin` sur votre carte MicroSD.
2. Insérez la carte dans votre imprimante et allumez-la.
3. La mise à jour démarre automatiquement. **Ne coupez pas l’alimentation** pendant la mise à jour.

   <img src="img/D12-230_EVO_MEGA-KIT_3.png" alt="firmware - D12-230 Evo Mega-Kit" width="300">

4. Une fois terminé, retirez la carte MicroSD et redémarrez l’imprimante.

## Étape 3 : Connecter le Pad/Dispositif à l'Imprimante
1. Connectez le pad à votre imprimante à l'aide du câble USB.
2. Vérifiez que votre pad est bien connecté au réseau ou via un câble Ethernet.
3. Accédez à l'interface Klipper en ouvrant `http://[adresse IP du pad]` dans votre navigateur.

## Étape 4 : Configurer les paramètres de l’imprimante
1. Dans l'interface web Klipper, allez dans l'onglet **Machine**.

    <img src="img/D12-230_EVO_MEGA-KIT_4.png" alt="Mainsail - Machine Tab" width="900">

2. Remplacez le fichier `printer.cfg` existant par celui que vous avez téléchargé depuis GitHub.
3. Cliquez sur **Save** puis redémarrez l'imprimante pour appliquer les modifications.

## Étape 5 : Configuration du slicer (OrcaSlicer)
1. Téléchargez OrcaSlicer depuis le lien suivant : [Télécharger OrcaSlicer](https://github.com/SoftFever/OrcaSlicer/releases).
2. Ajoutez le profil de l’imprimante Wanhao D12 300 aux profils d'imprimantes prédéfinis dans OrcaSlicer.
3. Ensuite, importez le profil D12-230 disponible au lien suivant : [Profil D12-230](https://github.com/Yumi-Lab/yumi-wiki/raw/main/Profile_Slicer/Orcaslicer/WanhaoD12Orcaslicer.zip). Il existe deux versions : avec 3D Touch et sans.

    <img src="img/D12-230_EVO_MEGA-KIT_4.png" alt="Orca Slicer" width="900">

## Étape 76 : Calibrations et réglages avant impression
1. **Calibration de l'extrudeur**  
   - Assurez-vous que l'extrudeur pousse la bonne quantité de filament. 

2. **Réglage du Z-offset**  
   - Un bon réglage du Z-offset est essentiel pour obtenir une première couche de qualité.

3. **PID Tuning**  
   - Effectuez le PID Tuning pour l'extrudeur et le lit chauffant afin de maintenir une température stable. 

4. **Test de résonnance (ADXL)** 


### **Tests à effectuer avant d’imprimer :**
1. **Test de première couche** : Assurez-vous d’un bon nivellement avec un test spécifique.
 
   <img src="img/D12-230_EVO_MEGA-KIT_6.png" alt="Première couche" width="250">

2. **Cube de calibration** : Imprimez un cube 20x20x20 mm pour vérifier les dimensions et l'extrusion.

   <img src="img/D12-230_EVO_MEGA-KIT_7.webp" alt="Cube de calibration" width="250">

Des modèles sont disponibles sur [Thingiverse](https://www.thingiverse.com/) et [Printables](https://www.printables.com/).




