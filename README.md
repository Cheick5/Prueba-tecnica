# Prueba-tecnica-webcursos

Dejaré los pasos que utilicé para mayor transparencia

1.- Descargué xampp, moodle(en inglés) y eMarketing, no sabía que php 8.x no funcionaba con moodle y estuve 30 mins viendo que hacer
2.- Descargué un xampp con php 7.4.15 y creé la prueba de emarking
3.- Tras intentar descifrar de donde venia la string "Detalles de la prueba" (Que para mí era "Exam details"), usé inspeccionar elemento y la herramienta de debugg de moodle
4.- Sabía por la url que estaba viendo un archivo llamado exam.php, por lo que abrí ese archivo y no encontré nada
5.- Decidí cambiar el lenguaje de moodle para evitar confusiones y me percaté que "Exam details" cambiaba a "Detalles de la prueba" así que decidí buscar los archivos de lenguaje
6.- En la carpeta lang estaban los archivos de lenguaje del inglés y el español, usando control+f encontré la frase que quería cambiar, pero cuando la cambié en el archivo de lenguaje no pasaba nada
7.- Me di cuenta de que se estaba creando una variable "examdetails" por lo que la busqué exam.php para ver si era llamada en algún momento
8.- Cambié el get_string(“examdetails”,”mod_emarking”) por "Quiero ingresar al equipo de desarrollo de Webcursos", dejando el "&nbsp", ya que este equivale a los bordes derechos.
9.- Cree un nuevo emarking para ver si el texto aparecía
