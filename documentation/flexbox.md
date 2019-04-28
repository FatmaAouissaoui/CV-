            flexbox 

 le css a créé un modèle de disposition appelé `Flexible box` (qu’on appelle couramment le FlexBox) qui introduit la nouvelle valeur flex pour la propriété `display` ainsi que la propriété `flex` (et toutes ses sous propriétés).
 
     display: flex|inline-flex;
     
C'est ainsi qu'on définit un container flex, il est block par défaut ou inline selon la valeur donnée. Cela cée un contexte flex pour tous les descendants directs.

   `display: flex | inline-flex;`

`flex` : Cette valeur génère un container flex, de niveau block, à l'intérieur de l'élément.

`inline-flex` : Cette valeur génère un container flex, de niveau inline, à l'intérieur de l'élément.
     
         flex-direction
 
 La propriété flex-direction établit l'axe principal.
 
 `flex-direction: row | row-reverse | column | column-reverse`
 
 `row (valeur par défaut)`: de gauche à droite si la lecture se fait dans ce sens, de droite à gauche dans le cas inverse (1).
 
 `row-reverse` : inverse le sens
 
 `column` : comme row mais du haut vers le bas
 
 `column-reverse` : comme row-reverse mais du bas vers le haut
           
 
         justify-content
 
 La propriété `justify-content` définit l'alignement le long de l'axe principal. Elle permet de distribuer l'espace excédentaire lorsque tous les items flex sur une ligne sont inflexibles ou lorsqu'ils ont atteint leur taille maximale. Elle contrôle aussi l'alignement des items lorsqu'ils débordent.
 
 `justify-content`: flex-start | flex-end | center | space-between | space-around
 
 `flex-start (par défaut) `: les items sont regroupés en début de ligne
 
 `flex-end` : les items sont regroupés en fin de ligne
 
 `center` : les items sont centrés le long de la ligne
 
 `space-between` : les items sont répartis sur la ligne; le premier est collé du côté start, le dernier du côté end.
 
 `space-around` : les items sont répartis sur la ligne avec un espacement égal autour de chacun.
          
   
               align-content
   
   La propriété `align-content` aligne les lignes d'un container flex à l'intérieur de l'espace où il reste de l'espace sur l'axe cross, un peu comme justify-content aligne les items sur l'axe principal.
   
   Note : cette propriété n'a pas d'effet quand la flexbox n'a qu'une seule ligne.
   
   `align-content: flex-start | flex-end | center | space-between | space-around | stretch`
   
   `flex-start` : lignes regroupées au début du container
  
  `flex-end` : lignes regroupées à la fin du container
  
   `center` : lignes regroupées au centre du container
  
   `space-between` : les lignes sont réparties, la première est collée du côté start, la dernière du côté end.
  
   `space-around` : les lignes sont réparties avec un espacement égal autour de chacune.
  
   `stretch (par défaut)` : les lignes s'étirent pour remplir tout l'espace.       