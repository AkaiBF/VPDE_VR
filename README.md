# Tanks VR

Para crear el juego en VR, hemos de añadir desde el Package Manager XR Plugin Management y XR Interaction Toolkit.
Una vez hecho esto, crearemos un GameObject con un XR Origin, un objeto vacío dentro (el offset de nuestra cámara) y la Main Camera dentro de éste.
Tras mover la Main Camera, hemos de transformarma en una VR Camera. Para ello le añadiremos el componente Tracked Pose Driver. Teniendo en cuenta el dispositivo que trabajaremos, cambiamos sus parámetros. Por ejemplo, yo utilizo unas Oculus Rift, por lo que el Tracking Type será de Rotation And Position.

Para colocar la cámara sobre el tanque, se debe crear un script para que la cámara siga al tanque. Sin embargo, he optado por una cámara superior para ver todo el terreno de mapa.

Los controles se pueden asignar desde el Input Manager de Unity, que también reconoce los controles de Oculus Rift.

Tras probarlo, afirmo que la decisión de la cámara superior produce Motion Sickness.