# Proyecto:  Agente conversacional de BanCom para Solicitud de Préstamos


## 1.Descripción breve del producto: 
El proyecto propone un asistente conversacional de BanCom que transforma la intención de solicitar un préstamo en un expediente digital completo, trazable y listo para evaluación utilizando WhatsApp como interfase del cliente. La inspiración nace de un problema operativo real del onboarding crediticio en banca peruana: solicitudes incompletas, validaciones manuales y dispersas, falta de guía al cliente y reprocesos internos. El enfoque de product-market fit se sustenta en resolver un dolor relevante del mercado, observar carencias de la competencia y diseñar una experiencia simple, útil y medible

## 2.Fuentes de inspiración

### 2.1 Marco conceptual de product-market fit:

- **Problema central:** Es la fricción en el onboarding de créditos: solicitudes incompletas, validaciones manuales, observaciones reiteradas y poca trazabilidad del expediente.	La intención del cliente no siempre se convierte en una solicitud lista para evaluación, lo que genera abandono, demoras y reprocesos.
- **Causas del problema:** El proceso actual depende de captura fragmentada de datos, revisión manual de documentos y escasa guía contextual para el cliente.	El usuario no siempre entiende qué debe completar, qué falta o cuál es el siguiente paso.
- **Consecuencias del problema:** La fricción afecta tanto al cliente como al banco.	Para el cliente: frustración, menor confianza y abandono. Para el banco: más costo operativo, más tiempo de ciclo y menor conversión digital.
- **Evaluación competitiva:** Los competidores relevantes son bancos con experiencia digital madura en originación: BCP, BBVA e Interbank.	La competencia ya cubre velocidad y autoservicio, pero aún existe espacio para una experiencia más guiada, explicativa y trazable.
- **Diferenciación esperada:**	El agente BanCom combina conversación guiada, checklist documental, observaciones accionables, timeline y derivación estructurada.	No compite solo como formulario digital, sino como experiencia asistida de principio a fin.

### 2.2 Formular el problema principal: que enfrenta el usuario o empresa objetivo, explicando el rol del agente, limites, y tipo de respuestas del agente.

### Problema
El agente resuelve la fricción operativa en el onboarding de créditos: solicitudes que se retrasan, se abandonan o requieren reprocesos porque la documentación está incompleta, las validaciones son manuales y dispersas, y no existe una guía clara para el cliente ni para los ejecutivos. El objetivo es convertir la intención de solicitar un préstamo en un expediente listo para evaluación/decisión, con mínimo error y máxima trazabilidad.

### Rol del agente
Su rol principal es ser un Asistente de Onboarding de créditos. Actúa como asistente porque guía al usuario paso a paso, resuelve dudas e indica qué información y documentos necesita; y como operador automático porque ejecuta validaciones, consulta sistemas internos/externos y prepara la precalificación o el expediente digital en casos de bajo riesgo.

### Límites
El agente no aprueba ni rechaza formalmente un crédito fuera de políticas, no modifica condiciones contractuales ni estados en Core, no promete aprobación garantizada, no omite controles de cumplimiento como KYC/AML y no brinda asesoría legal, tributaria o de inversión. Si no dispone de información suficiente, debe declararlo, pedir lo faltante y, si persiste la falta de datos críticos, derivar el caso a un ejecutivo o analista.

*En términos funcionales, el agente no debe:*
- Prometer aprobación definitiva del crédito;
- Alterar políticas reales del banco;
- Inventar documentos o validaciones regulatorias;
- Asesorar fuera del alcance de la solicitud de préstamo;
- Simular ser un ejecutivo humano cuando no lo es;
- Omitir observaciones si faltan datos o documentos;
- Entregar explicaciones confusas, ambiguas o contradictorias;
- Solicitar información no necesaria para el flujo definido;
- Saltarse pasos críticos de validación documental;
- Dar respuestas fuera del tono institucional de BanCom.

*Qué no debe hacer:*
- No debe cambiar el problema, rol, límites ni tipo de respuestas definidos en Sprint 1.
- No debe usar lenguaje técnico complejo para el cliente.
- No debe responder con textos robóticos o genéricos.
- No debe hacer diagnóstico financiero profundo ni asesoría legal.
- No debe aprobar préstamos “por insistencia” del usuario.
- No debe continuar el flujo si faltan datos mínimos o documentos obligatorios.
- No debe perder el contexto del paso en el que se encuentra el usuario.

### Tipo de respuestas:
El agente entrega guía paso a paso, listas de requisitos y documentos personalizados, mensajes de observación claros sobre faltantes o errores, estado de la solicitud, precalificación referencial y resúmenes estructurados para analistas con datos clave, riesgos detectados, documentos recibidos/faltantes y recomendación operativa. Su estilo de respuesta es breve a medio, claro, directo y estructurado en pasos, checklists o fichas.


## 3. Problema principal y oportunidad de mercado

- **Problema principal:** las solicitudes de préstamo se quedan a medio camino entre la intención del cliente y un expediente evaluable; esto genera abandono, reproceso y demoras.
- **Causas raíz:** Captura de datos fragmentada, múltiples validaciones manuales, documentos observados sin instrucciones claras, poca visibilidad del estado de la solicitud y alta dependencia del ejecutivo para tareas repetitivas.
- **Consecuencias para el cliente:** frustración, percepción de complejidad, menor confianza y mayor probabilidad de abandonar el trámite.
- **Consecuencias para el banco:** mayores costos operativos, ciclos de originación más largos, productividad comercial reducida, riesgos por errores manuales y menor conversión digital.
- **Oportunidad de mercado:** en Perú el crédito viene recuperándose y los créditos de consumo lideraron el crecimiento a setiembre de 2025; además, los canales y pagos digitales elevan la expectativa por experiencias bancarias móviles, rápidas y seguras.
- **Público objetivo:** El segmento principal está dirigido a personas naturales y pequeños negocios interesados en solicitar un préstamo con BanCom.
- **Contexto de uso:** Usuarios que ingresan desde WhatsApp  y esperan una atención ágil, guiada y entendible, sin fricción y sin sentir que están llenando un formulario tradicional.
- **Tono y personalidad**
	- Profesional
	- Cálido
	- Claro
	- Confiable
	- Orientado a la acción

### Propuesta de valor: 
Transforma una solicitud de crédito en una experiencia conversacional simple, guiada y humana, reduciendo fricción, ordenando la captura de datos y documentos, y dando al usuario visibilidad del avance de su solicitud en todo momento.

### Ventajas diferenciales:
  - Conversación natural y no tipo interrogatorio.
  - Guía paso a paso con progreso visible.
  - Checklist documental claro y accionable.
  - Estado de solicitud entendible para el usuario.
  - Experiencia coherente con una atención bancaria formal pero cercana.
  - Permite mantener continuidad con acciones persistentes como ver estado, subir documentos o hablar con un ejecutivo.

- **Dolor crítico:** expedientes incompletos y sin trazabilidad.
- **Trigger de adopción:** solicitud rápida, guiada y sin fricción.
- **Resultado esperado:** más conversión y menor reproceso.

## 4. Propósito principal del proyecto 

Guiar al usuario paso a paso en la solicitud de un préstamo BanCom, dentro de una experiencia tipo chat en WhatsApp, ayudándolo a:
• Elegir el tipo de préstamo,
• Responder preguntas clave de perfil,
• Completar datos de monto, plazo y moneda,
• Cargar documentos requeridos,
• Dar seguimiento al estado de la solicitud, y; 
• Recibir un resultado preliminar de evaluación.

Está orientado a usuarios que desean iniciar o completar su solicitud de crédito en un entorno digital simple, humano y asistido.

## 5. Insights clave y oportunidades de diferenciación

- El mercado peruano ya educó al cliente a esperar experiencias digitales, móviles y rápidas; la oportunidad no está solo en digitalizar, sino en digitalizar mejor los casos imperfectos: clientes con dudas, documentos observados o información parcial.
- Los grandes bancos compiten con escala, marca y velocidad. BanCom puede diferenciarse con un onboarding explicativo, trazable y asistido, donde el agente no solo captura datos, sino que reduce incertidumbre.
- El agente propuesto aporta una combinación poco visible en ofertas tradicionales: conversación guiada, checklist documental con estados, observaciones concretas, timeline de avance, número de solicitud y salida dual para cliente y analista.
- Para PYMES y convenios, la capacidad de operar con información parcial y derivar inteligentemente a humano es una ventaja relevante frente a experiencias excesivamente rígidas.
- El uso de IA agrega valor donde más duele: completitud del expediente, calidad del dato, explicación del siguiente paso y productividad del ejecutivo.

**¿Qué podría aportar este agente de IA que otros no ofrecen?** 
- Acompañamiento paso a paso orientado a reducir abandono y no solo a vender un crédito.
- Corrección temprana del expediente con observaciones accionables antes de llegar al analista.
- Experiencia híbrida: autoservicio cuando el caso es simple y escalamiento ordenado cuando el caso requiere intervención humana.
- Trazabilidad visible para cliente y ejecutivo en una misma lógica de flujo.
- Base clara para medir product-market fit con métricas como expedientes completos, conversión, abandono, tiempo de ciclo y feedback positivo.

## 6. Arquitectura del agente 

- Canales de entrada: portal web y/o WhatsApp
- Percepción y preparación de datos: captura, extracción, normalización y control de calidad.
- Agente de Onboarding (MVP): guía al cliente, gestiona subsanaciones y define la siguiente mejor acción con contexto.
- Integraciones criticas: para el producto final: Core, CRM, repositorio documental, buró/RENIEC y capa de integración (APIs/eventos).
- Gobierno y control: auditoría, trazabilidad, métricas, monitoreo/logging y controles de seguridad; además, ejecutivos en el loop para excepciones.
- Memoria / conocimiento:  Vector DB + políticas + historial de casos, para consistencia y decisiones explicables.

**𝐌𝐕𝐏 𝐝𝐞 𝟑 𝐦𝐞𝐬𝐞𝐬 𝐲 𝐩𝐨𝐬𝐢𝐛𝐥𝐞 𝐞𝐯𝐨𝐥𝐮𝐜𝐢ó𝐧**

La propuesta del proyecto es un 𝐌𝐕𝐏 𝐝𝐞 𝟑 𝐦𝐞𝐬𝐞𝐬, con alcance acotado y métricas claras (tiempo de ciclo, abandono, retrabajo, conversión).

Si el agente inicial genera valor real, recién ahí tiene sentido evolucionar a una 𝐚𝐫𝐪𝐮𝐢𝐭𝐞𝐜𝐭𝐮𝐫𝐚 más compleja donde se desarrollen toda la capa de integraciones críticas y posibles 𝐦𝐮𝐥𝐭𝐢-𝐚𝐠𝐞𝐧𝐭𝐞s, invocando agentes especializados (documental, KYC/Compliance, Buró, RENIEC, repositorio documental, CRM, RRHH (convenios), riesgo, comunicación CX).  

## 7. Conclusión

El agente conversacional de BanCom para solicitudes de Créditos es parte de un problema real, frecuente y costoso dentro del mercado bancario peruano. La oportunidad no consiste únicamente en tener un formulario digital, sino en construir una experiencia que convierta intención en expediente completo, con menor fricción, mejor información y mayor capacidad de decisión. Bajo el marco de product-market fit, la propuesta tiene sentido porque ataca un dolor relevante, identifica un público claro, encuentra brechas en la competencia y define métricas concretas para validar valor desde el MVP. En síntesis, el espacio estratégico para BanCom está en competir por inteligencia operativa, cercanía y trazabilidad, no por escala.
