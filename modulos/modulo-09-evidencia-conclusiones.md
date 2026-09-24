# Módulo 9: Evidencia Digital, Desafíos y Conclusiones

**Responsable:** ALBA, Valentín Sebastián (`valentinalba0809@gmail.com`)  
**Estado:** Completo / Revisado  

---

## Índice de Contenidos
1. [La Evidencia Digital e Informática Forense](#1-la-evidencia-digital-e-informática-forense)
   - [1.1. Concepto de Evidencia Digital y Volatilidad de los Datos](#11-concepto-de-evidencia-digital-y-volatilidad-de-los-datos)
   - [1.2. Principios de Preservación y Adquisición Forense (ISO/IEC 27037)](#12-principios-de-preservación-y-adquisición-forense-isoiec-27037)
2. [Cadena de Custodia y Validez en Juicio](#2-cadena-de-custodia-y-validez-en-juicio)
   - [2.1. Procedimiento para Garantizar la Inalterabilidad de la Prueba](#21-procedimiento-para-garantizar-la-inalterabilidad-de-la-prueba)
   - [2.2. Desafíos de Admisibilidad Probatoria en el Proceso Penal](#22-desafíos-de-admisibilidad-probatoria-en-el-proceso-penal)
3. [Vinculación e Integración Temática (Apartado Obligatorio)](#3-vinculación-e-integración-temática-apartado-obligatorio)
   - [3.1. Conexión 1 — Unidad 1 (Derecho Constitucional): Impacto en Derechos y Garantías](#31-conexión-1--unidad-1-derecho-constitucional-impacto-en-derechos-y-garantías)
   - [3.2. Conexión 2 — Propiedad Intelectual y Contratos: Impacto Civil y Comercial del Ciberdelito](#32-conexión-2--propiedad-intelectual-y-contratos-impacto-civil-y-comercial-del-ciberdelito)
4. [Desafíos Futuros y Transnacionalidad](#4-desafíos-futuros-y-transnacionalidad)
   - [4.1. Jurisdicción y Extraterritorialidad del Ciberdelito](#41-jurisdicción-y-extraterritorialidad-del-ciberdelito)
   - [4.2. Inteligencia Artificial y Nuevos Tipos Delictivos Emergentes](#42-inteligencia-artificial-y-nuevos-tipos-delictivos-emergentes)
5. [Conclusiones Generales del Trabajo](#5-conclusiones-generales-del-trabajo)
6. [Fuentes y Referencias Consultadas](#6-fuentes-y-referencias-consultadas)

---

## 1. La Evidencia Digital e Informática Forense

### 1.1. Concepto de Evidencia Digital y Volatilidad de los Datos
La evidencia digital, también conocida como prueba informática, se define como cualquier información o dato con valor probatorio que es generado, almacenado o transmitido en formato binario. A diferencia de la prueba física tradicional (como un documento en papel o un arma), la evidencia digital posee una característica inherente que representa su mayor desafío jurídico: la **volatilidad**.

En los entornos informáticos, los datos (especialmente aquellos alojados en la memoria RAM, los registros de caché o las conexiones de red en curso) pueden ser alterados, sobrescritos, encriptados o destruidos en fracciones de segundo. Esta fragilidad extrema significa que una mala praxis durante un allanamiento o secuestro de dispositivos puede contaminar la prueba, provocando su nulidad absoluta en el proceso penal. Por lo tanto, el sistema judicial requiere que la manipulación de estos datos no altere el estado original en el que fueron hallados.

### 1.2. Principios de Preservación y Adquisición Forense (ISO/IEC 27037)
Para que un tribunal acepte la validez de un dato informático, los peritos deben aplicar metodologías científicas rigurosas. En este contexto, la norma internacional **ISO/IEC 27037** proporciona las directrices estandarizadas para la identificación, recolección, adquisición y preservación de la evidencia digital, dotando de seguridad jurídica al procedimiento técnico.

Esta norma se estructura sobre principios fundamentales para garantizar la integridad de la prueba:
*   **Identificación:** Consiste en reconocer y documentar qué elementos físicos (dispositivos de almacenamiento, teléfonos, servidores) o lógicos (cuentas en la nube, registros de logs) contienen evidencia potencial vinculada al delito investigado.
*   **Adquisición:** Es el proceso de extraer la información minimizando cualquier alteración del sistema. Para asegurar que la prueba sea idéntica al original, se utilizan herramientas de bloqueo de escritura (*write-blockers*) y se realizan copias "bit a bit" (clonación forense). Si el sistema está encendido, se debe respetar el "Orden de Volatilidad", capturando primero los datos que corren mayor riesgo de perderse.
*   **Preservación:** Su objetivo es garantizar que la evidencia adquirida se mantenga inalterable desde su recolección hasta su presentación en juicio. El estándar técnico y legal para demostrar esta inalterabilidad es el cálculo de algoritmos de **función hash** (como MD5 o SHA-256), que actúan como una huella digital única e irrepetible del archivo o disco clonado. Cualquier modificación posterior, por mínima que sea, cambiará el valor hash, evidenciando la manipulación de la prueba.

---

## 2. Cadena de Custodia y Validez en Juicio

### 2.1. Procedimiento para Garantizar la Inalterabilidad de la Prueba
La cadena de custodia es el procedimiento documentado, ininterrumpido y trazable que se aplica a los elementos probatorios desde el momento de su hallazgo o secuestro hasta su disposición final. En el ámbito de los delitos informáticos, este procedimiento es vital para garantizar la inalterabilidad de la prueba y certificar que la evidencia presentada en el tribunal es exactamente la misma que se extrajo de la escena del crimen, física o virtual.

El resguardo de la evidencia digital posee una doble dimensión normativa y técnica:
*   **Custodia física:** Implica el correcto embalaje, sellado y etiquetado del hardware secuestrado (discos rígidos, teléfonos celulares, pendrives). Se deben utilizar bolsas antiestáticas o "jaulas de Faraday" (para evitar el borrado remoto de datos en dispositivos móviles) y las actas de secuestro deben estar firmadas por testigos hábiles y los funcionarios intervinientes.
*   **Custodia lógica:** Es el resguardo del contenido digital propiamente dicho. Se materializa mediante el cálculo de la función hash en el momento exacto de la adquisición forense. El valor hash original se asienta en el acta notarial o judicial; al momento de realizar la pericia en el laboratorio, el perito debe recalcular el hash de su copia de trabajo y verificar que coincida de manera idéntica con el del acta. Si los valores difieren, la cadena de custodia lógica se ha roto y la prueba se considera contaminada.

### 2.2. Desafíos de Admisibilidad Probatoria en el Proceso Penal
El sistema procesal penal argentino se rige por el principio de libertad probatoria, lo que significa que los delitos pueden probarse por cualquier medio, siempre que su obtención sea lícita y no afecte las garantías constitucionales. Sin embargo, la evidencia digital presenta desafíos singulares para su admisibilidad en juicio:
1.  **Garantía de intimidad y licitud de la obtención:** La intromisión en un sistema informático, la interceptación de correos electrónicos o la requisa de un dispositivo móvil sin la debida orden judicial previa y fundada constituye una violación a la privacidad. Toda evidencia digital obtenida de manera ilegal es pasible de exclusión bajo la doctrina del *"fruto del árbol envenenado"*, anulando cualquier prueba derivada de ella.
2.  **Autenticidad y repudio:** A diferencia de un documento con firma hológrafa, la evidencia digital es fácilmente manipulable. La simple presentación de capturas de pantalla (*screenshots*) o correos impresos suele ser insuficiente si no está respaldada por metadatos o por la intervención de un perito informático. La defensa suele atacar la prueba alegando que los registros pudieron ser alterados, fabricados o que el titular de la cuenta no fue quien originó la comunicación (suplantación de identidad).
3.  **Dependencia de terceros y proveedores de servicios:** Gran parte de la evidencia actual (registros de WhatsApp, correos en Gmail, alojamientos en la nube) no reside en dispositivos físicos en poder del imputado, sino en servidores de empresas tecnológicas internacionales. La admisibilidad de estos registros requiere transitar por complejos procesos de requerimientos judiciales a plataformas que, en ocasiones, aplican políticas de retención de datos sumamente breves, provocando que la evidencia desaparezca antes de ser formalmente judicializada.

---

## 3. Vinculación e Integración Temática (Apartado Obligatorio)

El estudio de los delitos informáticos no puede concebirse como una rama aislada del derecho penal, sino que atraviesa de manera transversal el ordenamiento jurídico general. En este sentido, la irrupción de las nuevas tecnologías y la cibercriminalidad generan una profunda interacción con otras unidades del programa de estudio, destacándose especialmente su vinculación con el **Derecho Constitucional** y las normativas de **Propiedad Intelectual y Contratos**.

### 3.1. Conexión 1 — Unidad 1 (Derecho Constitucional): Impacto en Derechos y Garantías
El fenómeno de la delincuencia informática pone constantemente en tensión los preceptos fundamentales de la Constitución Nacional (CN), obligando a los operadores jurídicos a reinterpretar las garantías históricas en el entorno digital:

*   **Art. 18 CN (Principio de Legalidad y Debido Proceso):** La máxima *"nullum crimen, nulla poena sine praevia lege"* fue el motor que obligó a la sanción de la Ley 26.388. Antes de esta reforma, los jueces se encontraban ante el vacío legal de no poder condenar ciertas conductas digitales porque la analogía está prohibida en el derecho penal (por ejemplo, el "daño" exigía la destrucción de una cosa física, no de un software). Asimismo, el debido proceso rige la obtención de evidencia digital: cualquier injerencia del Estado en dispositivos tecnológicos sin orden judicial vulnera la garantía de defensa en juicio.
*   **Art. 19 CN (Intimidad y Privacidad):** El principio de reserva consagra que las acciones privadas están exentas de la autoridad de los magistrados. En la actualidad, el espectro de privacidad más sensible de un individuo reside en su correo electrónico, sus redes sociales y su teléfono celular. Delitos como el acceso ilegítimo (*hacking*), el ciberacoso o la interceptación de comunicaciones vulneran directamente el núcleo de este artículo, por lo que la ley penal busca proteger la expectativa de privacidad que los ciudadanos tienen sobre su identidad y sus datos digitales.
*   **Art. 14 CN (Libertad de Expresión):** La persecución del ciberdelito requiere encontrar un delicado equilibrio frente al derecho a publicar las ideas sin censura previa. Las medidas judiciales orientadas a bloquear sitios web, dar de baja perfiles o filtrar contenidos (por ejemplo, en casos de injurias o apología del delito en redes) rozan peligrosamente la censura. El desafío constitucional radica en reprimir el delito informático sin coartar la libertad de expresión y el libre flujo de información en Internet.

### 3.2. Conexión 2 — Propiedad Intelectual y Contratos: Impacto Civil y Comercial del Ciberdelito
El accionar delictivo en el ciberespacio excede la sanción penal, proyectando consecuencias directas sobre el derecho privado y comercial de las empresas tecnológicas:

1.  **Propiedad Intelectual:** En Argentina el software es protegido como una obra literaria (**Ley 11.723**). Cuando ocurre un delito de daño o sabotaje informático (Art. 183 CP), como la introducción de un código malicioso (*malware*) que corrompe una base de datos o el código fuente de un programa, el sujeto pasivo no solo sufre un menoscabo penal, sino una afectación directa a sus derechos de autor y a la explotación comercial de su propiedad intelectual.
2.  **Derecho Contractual y Responsabilidad Civil:** La provisión de servicios IT (alojamiento en la nube, servidores, mantenimiento) se rige por contratos que incluyen Acuerdos de Nivel de Servicio (SLA) y cláusulas de confidencialidad. Si una empresa proveedora es víctima de un delito informático (como un ataque DDoS o un *ransomware*), la caída de sus sistemas configura automáticamente un incumplimiento contractual frente a sus clientes. De esta manera, el delito informático actúa como el elemento desencadenante de una compleja red de responsabilidades civiles, obligando a indemnizar daños y perjuicios derivados de la vulneración del software propietario y la pérdida del servicio.

---

## 4. Desafíos Futuros y Transnacionalidad

### 4.1. Jurisdicción y Extraterritorialidad del Ciberdelito
El principal paradigma que quiebra el ciberdelito es el concepto tradicional de frontera y territorialidad. En el derecho penal clásico, la jurisdicción suele determinarse por el lugar físico donde se comete el hecho (Art. 1 del Código Penal Argentino). Sin embargo, la arquitectura de Internet permite que un ataque sea ejecutado desde un país, utilizando servidores intermediarios (*botnets*) ubicados en múltiples naciones, para finalmente vulnerar el bien jurídico de una víctima residente en la Argentina.

Esta transnacionalidad inherente genera enormes fricciones procesales:
*   **Conflictos de competencia:** Dificultad para establecer si debe investigar el juez del país del atacante, el del lugar donde se alojan los datos o el del domicilio de la víctima.
*   **Cooperación internacional:** La lentitud de los exhortos diplomáticos tradicionales es incompatible con la volatilidad de la evidencia digital. Si bien instrumentos como el **Convenio de Budapest** (al cual Argentina está adherida) buscan agilizar la asistencia legal mutua y la preservación rápida de datos informáticos en el extranjero, la disparidad de legislaciones y la falta de tratados de extradición dificultan la persecución efectiva del delincuente.

### 4.2. Inteligencia Artificial y Nuevos Tipos Delictivos Emergentes
La irrupción de la Inteligencia Artificial (IA) generativa plantea el próximo gran desafío legislativo. Las herramientas automatizadas están abaratando los costos de la cibercriminalidad y perfeccionando la ejecución de los delitos.

Entre los nuevos horizontes delictivos impulsados por la IA se destacan:
*   **Deepfakes y biometría sintética:** La capacidad de clonar voces humanas o generar videos hiperrealistas abre la puerta a nuevas modalidades de extorsión, suplantación de identidad avanzada (fraudes bancarios donde se burla el reconocimiento facial) y generación de material de abuso sexual infantil (MASI) sintético, dificultando la pericia para distinguir lo real de lo artificial.
*   **Phishing e Ingeniería Social automatizada:** Los modelos de lenguaje natural permiten a los ciberdelincuentes generar correos electrónicos y mensajes de fraude con una gramática perfecta, personalizados en masa y adaptados al contexto de cada víctima.
*   **Malware inteligente:** Desarrollo de códigos maliciosos capaces de mutar autónomamente y evadir los sistemas de detección tradicionales (antivirus) mediante el aprendizaje automático (*Machine Learning*).

El desafío futuro para el legislador ya no será únicamente tipificar nuevas conductas, sino dotar a las fuerzas de seguridad y al Poder Judicial de las herramientas tecnológicas y las capacidades técnicas necesarias para investigar delitos perpetrados por máquinas autónomas en nombre de operadores humanos.

---

## 5. Conclusiones Generales del Trabajo

Tras el desarrollo de este Trabajo Práctico de Investigación, el **Grupo 141-A** ha arribado a las siguientes conclusiones fundamentales sobre el tratamiento de los delitos informáticos en Argentina:

1.  **Cambio de Paradigma:** Es innegable que la tecnología ha transformado de manera irreversible el paradigma del derecho penal. El sistema informático ya no es solo una herramienta, sino que se ha consolidado como un medio de comisión para potenciar delitos tradicionales y como un nuevo bien jurídico protegido en sí mismo (ante sabotajes o intrusiones).
2.  **Avance Normativo y Cuello de Botella Probatorio:** La sanción de la Ley 26.388 marcó un hito fundamental al sacar al ordenamiento jurídico argentino de la obsolescencia y adaptarlo a los estándares del Convenio de Budapest. No obstante, el verdadero "cuello de botella" del sistema penal radica en la capacidad probatoria: la volatilidad de la evidencia digital, las exigencias de la cadena de custodia y los conflictos jurisdiccionales transnacionales provocan que muchas investigaciones naufraguen antes de llegar a juicio.
3.  **Desafío Dinámico:** El surgimiento de tecnologías disruptivas, especialmente la Inteligencia Artificial, advierte que la legislación no puede ser estática. El derecho informático está condenado a perseguir a la innovación tecnológica. Por lo tanto, el éxito futuro dependerá menos de la constante creación de nuevas leyes y más de la capacitación técnica permanente de los operadores judiciales (peritos, fiscales y jueces) y de la consolidación de canales de cooperación internacional ágiles y efectivos.

---

## 6. Fuentes y Referencias Consultadas

*   **Código Penal de la Nación Argentina** — Arts. 131, 153 bis, 173 inc. 16, 183 y concordantes.
*   **Constitución Nacional Argentina** — Arts. 14, 18 y 19.
*   **Ley N.º 26.388** — Modificatoria del Código Penal en materia de Delitos Informáticos.
*   **Ley N.º 26.904** — Incorporación del delito de Grooming (Art. 131 C.P.).
*   **Ley N.º 11.723** — Régimen Legal de la Propiedad Intelectual (Protección de Software).
*   **Ley N.º 27.411** — Aprobación del Convenio de Budapest sobre Ciberdelincuencia.
*   **Norma ISO/IEC 27037:2012** — *Directrices para la identificación, recolección, adquisición y preservación de evidencia digital*.



