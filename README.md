# OpenGL_proj
Cuprins


1.	Cerinta proiect
2.	Prezentarea temei
3. Scenariul
3.1. Descrierea scenei și a obiectelor
3.2. Funcționalități
4. Detalii de implementare
	4.1 Functii si algoritmi
	4.2 Structuri de date
	4.3 Ierarhia de clase 
5. Manual de utilizare
6. Concluzii si dezvoltari ulterioare

1. Cerinta proiect

Proiectele au ca și scop realizarea unei prezentări fotorealiste a unor scene de obiecte 3D utilizând librăriile prezentate la laborator (OpenGl, GLFW, GLM, etc.). Utilizatorul trebuie să aibă posibilitatea de a controla scena prin intermediul mausului și tastaturii.

2. Prezentarea temei
	
	Pentru acest proiect am ales sa pun intr-o scena o cabana din lemn la marginea unui lac, inconjurata de mai multe obiecte. Interactiunea cu scena este posibila prin intermediul mouse-ului sau a tastaturii. Pentru implementare am folosit biblioteca grafica OpenGL, Blender si Microsoft Visual Studio.  

3. Scenariul

	Scena contine mai multe obiecte:
•	un plan cu denivelari (dealuri si un lac) cu textura de iarba pe care sunt asezate restul obiectelor si un skybox cu un apuc de soare.


•	copaci care inconjoara cabana


•	un caine care incepe sa se roteasca spre stanga si spre dreapta la apasarea unei taste (pazeste cabana)


•	o barca din lemn care poate fi miscata pe lac cu ajutorul tastaturii


•	cabana din lemn la marginea lacului

Navigarea prin scena se poate realiza foarte usor cu ajutorul mouse-ului si a tastaturii vizualizarea fiind posibila din orice unghi sau distanta. De asemenea, scena poate fi prezentata in mai multe moduri alese din tastatura: point, wireframe si solid.

4. Detalii de implementare

Majoritatea functiilor folosite la acest proiect provin din biblioteca OpenGL sau au fost implementate pe parcursul semestrului la orele de laborator. Functiile cele mai importante definite in proiect sunt: renderScene() care se ocupa de aproape toate datele, void initShaders() care realizeaza incarcarea shaderelor, void initModels() ce se ocupa cu incarcarea modelelor 3D.
Din punctul de vedere al datelor am avut nevoie de structuri specifice OpenGL, GLM si sunt destul de simple, de exemplu vec3, vec4, mat4 GLuint, GLfloat.
Ierarhie de clase:
o	Model3D: gestionarea modelelor 3D.
o	Camera: miscarile si directia camerei.
o	SkyBox: contine implementarea skybox
o	Shader: folosita la incarcarea si folosirea programelor de tip shader
o	Mesh: gestioneaza varfurile obiectelor







5. Manual de utilizare

Cu ajutorul mouse-ului se poate controla direstia de privire in scena.
Tastatura are mai multe functionalitati:
•	Q - incepe rotirea stanga dreapta a cainelui
•	E – opreste rotirea cainelui
•	W, A, S, D – miscarea camerei inainte, inapoi, stanga respectiv dreapta
•	UP, DOWN, LEFT, RIGHT – miscarea barcii pe lac
•	7 – point 
•	8 – wireframe
•	9 – solid    
•	1 – creste intensitate ceata
•	2 – scade intensitate ceata

6. Concluzii si dezvoltari ulterioare
In concluzie, OpenGL si Blender chiar daca nu sunt foarte usor de inteles te pot ajuta sa creezi o iluzie destul de buna a realitatii. Intelegerea acestor noi instrumente (noi pentru mine) nu a fost usoara, dar cu ajutorul lucrarilor de laborator de pe parcursul semestrului si a unor tutoriale de pe internet se poate spune ca am avansat semnificativ. Dupa parerea mea acest proiect nu a fost unul usor, dar in final s-a dovedit a fi unul interesant.
Ca si dezvoltari ulterioare pentru aceasta aplicatie am putea implementa:
•	spotlight or point light (surse de lumina)
•	shadows (umbre)
•	detectarea coliziunilor
•	noi elemente pentru a folosi mai mult spatiu din plan

