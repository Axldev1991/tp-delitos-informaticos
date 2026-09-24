# Módulo 6: Delitos en Particular II — Phishing y Estafas Digitales

**Responsable:** CASTELLANO GUTIERREZ, Axel (`castellanoaxl@gmail.com`)  

---

## Índice de Contenidos
1. [Phishing e Ingeniería Social](#1-phishing-e-ingeniería-social)
   - [1.1. Concepto y Taxonomía del Phishing](#11-concepto-y-taxonomía-del-phishing)
   - [1.2. Mecanismos de Engaño y Vectores de Ataque](#12-mecanismos-de-engaño-y-vectores-de-ataque)
2. [Fraude e Identidad Digital](#2-fraude-e-identidad-digital)
   - [2.1. Encuadre Penal: Art. 173 inc. 16 del Código Penal (Ley 26.388)](#21-encuadre-penal-art-173-inc-16-del-código-penal-ley-26388)
   - [2.2. Suplantación de Identidad y Modalidades Delictivas Complejas](#22-suplantación-de-identidad-y-modalidades-delictivas-complejas)
3. [Responsabilidad Bancaria y de Plataformas](#3-responsabilidad-bancaria-y-de-plataformas)
   - [3.1. Marco Regulatorio del Banco Central de la República Argentina (BCRA)](#31-marco-regulatorio-del-banco-central-de-la-república-argentina-bcra)
   - [3.2. Deber de Seguridad y Responsabilidad Civil Objetiva](#32-deber-de-seguridad-y-responsabilidad-civil-objetiva)
4. [Fuentes y Referencias Consultadas](#4-fuentes-y-referencias-consultadas)

---


## 1. Phishing e Ingeniería Social

### 1.1. Concepto y Taxonomía del Phishing
El *phishing* es una técnica de ingeniería social orientada a la manipulación psicológica de los usuarios para la obtención ilegítima de datos confidenciales (credenciales de acceso, claves bancarias, números de tarjetas de crédito o tokens de autenticación). A diferencia de los ataques dirigidos puramente a vulnerabilidades de software, explota el factor humano mediante la suplantación de identidad de entidades de confianza.

Entre sus variantes principales se destacan:
*   **Phishing Tradicional:** Envíos masivos e indiscriminados de correos electrónicos falsificados que redirigen a sitios web apócrifos.
*   **Spear Phishing:** Ataque altamente personalizado y dirigido a individuos o sectores específicos dentro de una organización, previa recolección de información objetivo.
*   **Smishing:** Modalidad ejecutada a través de mensajes de texto (SMS) o mensajería instantánea (WhatsApp, Telegram) invitando a ingresar a enlaces maliciosos o descargar archivos.
*   **Vishing:** Engaño por vía telefónica o voz sobre IP (VoIP), donde el atacante personifica a un operador bancario, de soporte técnico o de organismos públicos para extraer datos de seguridad en tiempo real.

### 1.2. Mecanismos de Engaño y Vectores de Ataque
Los ataques de ingeniería social operan combinando factores de urgencia, autoridad y oportunidad:
1.  **Suplantación de Dominios y Marcas (Typosquatting / Domain Spoofing):** Registro de nombres de dominio visualmente idénticos a los oficiales.
2.  **Captura Activa de Credenciales:** Uso de portales intermediarios (*man-in-the-middle*) creados para interceptar credenciales y códigos de segundo factor de autenticación (2FA/OTP).
3.  **Descarga de Payload Malicioso:** Infección colateral por *malware* (trojano bancario o *keylogger*) a partir del enlace o adjunto recibido.

---

## 2. Fraude e Identidad Digital

### 2.1. Encuadre Penal: Art. 173 inc. 16 del Código Penal (Ley 26.388)
En el derecho penal argentino, las defraudaciones digitales encuentran su tipo normativo específico en el **artículo 173, inciso 16 del Código Penal**, incorporado por la **Ley 26.388** de Delitos Informáticos:

> *"El que defraudare a otro mediante cualquier técnica de manipulación informática que altere el normal funcionamiento de un sistema informático o la transmisión de datos."*

*   **Diferencia dogmática con la Estafa Tradicional (Art. 172 C.P.):** Mientras la estafa clásica requiere la secuencia *ardid → error → disposición patrimonial → perjuicio*, en el fraude informático la conducta típicamente altera el procesamiento autómata o la transmisión digital de datos sin que necesariamente medie el vicio de la voluntad en el acto de transferencia de la víctima.
*   **Bien Jurídico Protegido:** El patrimonio, en confluencia con la integridad e intangibilidad de los sistemas de procesamiento de datos.

### 2.2. Suplantación de Identidad y Modalidades Delictivas Complejas
*   **SIM Swapping (Duplicación no autorizada de SIM):** Maniobra en la cual el delincuente engaña a la empresa proveedora de telefonía móvil para tomar el control de la línea del usuario, interceptando los códigos SMS de verificación bancaria.
*   **Vishing Bancario y Falsos Gestores:** Modalidad muy frecuente donde la víctima es guiada telefónicamente hacia un cajero automático o app bancaria para autorizar tokens o modificar su clave Token.
*   **Fraude mediante DEBIN (Débito Inmediato):** Utilización engañosa de la herramienta de débito solicitando a la víctima "autorizar una transferencia a su favor", cuando en realidad autoriza la extracción de fondos propios.

---

## 3. Responsabilidad Bancaria y de Plataformas

### 3.1. Marco Regulatorio del Banco Central de la República Argentina (BCRA)
Frente al incremento exponencial del cibercrimen financiero, el BCRA dictó normativas de cumplimiento obligatorio para las entidades financieras:
*   **Comunicación "A" 7319:** Establece controles estrictos para el otorgamiento de **créditos preaprobados** vía homebanking. Obliga a verificar de forma fehaciente la identidad del solicitante mediante validación biométrica o prueba de vida, además de verificar la no modificación reciente de los canales de contacto (email/teléfono) y fijar plazos de diferimiento en la acreditación.
*   **Comunicación "A" 7326:** Regula las operaciones por **DEBIN**, imponiendo la notificación clara y destacada al usuario indicando expresamente que la transacción implicará la extracción de fondos de su cuenta.

### 3.2. Deber de Seguridad y Responsabilidad Civil Objetiva
En la jurisprudencia argentina actual, la relación entre el usuario y la entidad bancaria se encuadra en una **relación de consumo** regulada por la **Ley 24.240 (Ley de Defensa del Consumidor)** y el Código Civil y Comercial de la Nación:
*   **Art. 40 de la Ley 24.240:** Consagra la **responsabilidad objetiva** por el vicio o riesgo del servicio. La banca electrónica constituye un servicio riesgoso cuya seguridad debe ser garantizada por la entidad financiera que lucra con el sistema.
*   **Deber de Seguridad e Incumplimiento de Normas BCRA:** La inobservancia de los estándares fijados por el BCRA (ej. acreditación inmediata de préstamos sin validación biométrica frente a patrones inusuales de conducta) configura negligencia bancaria.
*   **Tendencia Jurisprudencial:** Salvo supuestos excepcionales de culpa grave imputable con exclusividad a la víctima, la justicia condena de forma reiterada a los bancos a declarar la nulidad de los préstamos fraudulentos, restituir los débitos indebidos y reparar el daño moral y punitivo del usuario afectado.

---

## 4. Fuentes y Referencias Consultadas

*   **Código Penal de la Nación Argentina** — Ley N° 11.179 (t.o. 1984) y modificatorias (Ley N° 26.388 de Delitos Informáticos).
*   **Banco Central de la República Argentina (BCRA)** — Comunicaciones "A" 7319 y "A" 7326 sobre seguridad en canales electrónicos.
*   **Ley de Defensa del Consumidor N° 24.240** — Art. 40 y concordantes.
*   **CERT.ar & UFECI** — Informes y recomendaciones técnicas sobre prevención de ciberdelitos e ingeniería social.
*   **Jurisprudencia Nacional:** Fallos de la Cámara Nacional de Apelaciones en lo Comercial y Tribunales Provinciales en materia de nulidad de préstamos y responsabilidad bancaria por phishing.

