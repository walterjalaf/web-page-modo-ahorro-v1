# REQUERIMIENTOS TÉCNICOS 

1. [] Crear un sitio web de desplazamiento vertical (scroll web site) que permita una navegación fluida y atractiva.
2. [] Diseño y objetivo: Mantener un diseño limpio y minimalista con un objetivo claro. Incluir llamadas a la acción y optimización para dispositivos móviles. Utilizar el diseño actual como referencia para estructurar el frontend.
3. [] Navegación: Incluir enlaces a “Home”, “Servicios e Informes”, “Solicitarlo” y “Sobre Nosotros” con desplazamiento visual mediante #ID.
4. [] Login: Implementar un sistema de login con tres opciones de sesión: Clientes, Gestores y Consultores.
5. [] Clientes, leer apartado
6. [] Gestores, leer apartado
7. [] Consultores, leer apartado
8. [] Chatbot “Modito”: Incluir un icono de acceso al chatbot “Modito”. (Ver apartado Chatbot)
9. [] Tarjetas de informes: Analizar y diseñar las tarjetas de opciones de informes.
10. [] Formulario de solicitudes: Revisar y ajustar el formulario de solicitudes para asegurar su funcionalidad.
11. [] Testimonios: Incluir un apartado de testimonios opcional. Si no hay comentarios disponibles, desactivar mediante CSS hasta que se decida incluir experiencias.
12. [] Footer: Revisar el footer y asegurar la correcta inclusión de enlaces a redes sociales.
13. [] Paneles de informes: Crear diferentes paneles para cada tipo de perfil (Clientes, Gestores, Consultores) que permitan realizar diversas acciones.
14. [] Panel de administración: Desarrollar un panel propio para modificar tarifas, ver cantidades e información de clientes, gestores y demás.

# FRONTEND
1. [] Elegir frameworks a trabajar
2. [] Determinar participantes que conformen frontend
3. [] Elegir un responsable fijo
4. [] Determinar librerias para las muestras de Gráficos

# BACKEND
1. [] Elegir Frameworks a trabajar
2. [] Determinar participantes que conformen el Backend
3. [] Elegir un responsable fijo
4. [] Gestionar bases de datos

# CHATBOT
1. [] Elegir framework a trabajar
2. [] Determinar cantidad de participantes que se encarge del desarrolo del chatbot
3. [] Elegir un responsable fijo

# BASE DE DATOS
1. [] Elegir tipo de base de datos, tablas o colecciones, relacionales o no relacionales.
2. [] Determinar la cantidad de participantes que se encargan de bases de datos
3. [] Determinar si habra un responsable fijo.
4. [] Base de datos
      a. Clientes
      b. Gestores
      c. Consultores
      d. Informes


# CLIENTES
1. [] El registro de clientes es importante, ya que es la forma que se puedan hacer los informes solicitados
2. [] Los clientes tendrán id unicos, son necesarios todos los campos que sean revelante al informe que solicitan, no es lo mismo un cliente hogareño que al de una industria.
3. [] No olvidar de usar campos de informe para filtrar (hogar)
4. [] Determinar si los gestores puede completar el resto de los campos, basado en lo que se necesite, y si es así permitir desde su panel la opcion de modificar mediante fronEnd, dicho datos. 
5. [] Determinar si es suficiente con el login rápido al estilo authentificación de google.
6. [] Determinar si un cliente debe ser siempre una persona, o puede ser el nombre de una empresa
7. [] Dar muestras de importancia de politica de privacidad. {el gasto interno de una empresa es información confidencial}

  para hogar

    {
  "clienteId: "0c72b2f9b1e8a5f4c2f1d4"
  "nombre": "Juan Pérez",
  "tipoCliente": "hogar",
  "direccion": "Calle Falsa 123",
  "consultorAsignado": 60c72b2f9b1e8a5f4d3f4d3f
}

para Comercio  

       {
  "clienteId: "0c72b2f9b1e8a5f4c2f1d4"
  "nombre": "Julian Alvarez",
  "tipoCliente": "Comercio",
  "direccion": "Menzdoza 55 sur",
  "teléfono": "264123456,
  "otros_campos": "xxxx"
  "consultorAsignado": 60c72b2f9b1e8a5f4d3f4d3f
}


# GESTORES
1. [] Los gestores deben tener ID unico, para que se asocie con uno o varios clientes en lo cual este trabajando o haya finalizado, y para que tambien el Consultor pueda hacer las tareas de revision, control y aprobación
2. [] Los campos de los gestores deben ser completos, y deben estar cargadas todas sus capacidades profesionales, el sistema debe proveer a los candidatos idoneos. 
3. [] El sistema debe determinar sus proximidades de los clientes, no es lo mismo solicitar un gestor de Zonda para que vaya a Caucete, que uno de 9 de julio que lo haga.
4. [] Herramientas de carga, comparativas y muestreo de informes en el panel.
5. [] El sistema debe poder compartir hasta 3 gestores un mismo informes, ya que dependiendo del trabajo puede que necesite esa modalidad de trabajo.
6. [] En el llegado caso, el sistema debe tener en cuenta, proximidad, disponibilidad y capacidades de los gestores.
7. [] Los gestores, dependiendo el proyecto, en cantidad, se nombrarán, lider y ayudantes (todos cobran lo mismo)
8. [] Los gestores tendrán puntos de rangos por cantidad de trabajos realizados, determinando así trabajar en oferta más dificiles y como lideres.

{  
  "gestorId": "60c72b2f9b1e8a5f4d3f4d3f"
  "nombre": "Francisco Ormeño ",
  "tipoGestor": "Ingeniero",
  "especialización": "Ingenería Industrial"
  "direccion": "Calle Falsa 123",
  "teléfono" : "2644123456,
  "cantidadInformesCompletos": "X",
  "informe_pendiente": "true",
  "otros_campos": "xxxx"
}

# CONSULTORES
1. [] Los consultores tendrán id unicos, y podrá ver los informes que se les haya asignado a ellos para revision, control y aprobación
2. [] Cuando hay una solicitud de gestoría, el Consultor solicitará 1 o varios gestores.
3. [] El sistema tiene que proveerle, los gestores disponibles, candidatos en proximidad y capacidad. Tambien el sistema en caso de seleccionar 3 gestores, debe llevar 2 muy buenos y 1 como ayudante.
4. [] Ver si se puede implementar algun tipo de tecnologia Scrum, que permita hacer seguimientos de tiempos de trabajo de los informes.


 {
  "informeID": "0c72b2f9b1e8a5f4b2f4d5",
  "clienteId": "0c72b2f9b1e8a5f4c2f1d4",
  "nombre": "Julian Alvarez",
  "tipoCliente": "Industria",
  "direccion": "Calle 15 y ruta 40",
  "consultorAsignado": [
    "60c72b2f9b1e8a5f4d3f4d3f",
    "60c72b2f9b1e8a5f4d1f2d4f",
    "60c72b2f9b1e8a5f4d3f4d7f"
  ]
}

# INFORMES
1. [] Este panel contiene toda la lógica de la gestoría energética y la visualización
2. [] Debe haber una especie de view timeline, para determinar el tiempo de transcurso
3. [] input de entradas de datos por teclado
4. [] input de entrada de imagenes relevante 
5. [] averiguar si es necesario input de entradas de videos
6. [] item 4 y 5 no son datos a procesar, si no más bien de fundamentación, investigación y evidencia para las propuestas de mejoras, son los consultores, los que determinan la relevancia de esos datos
7. [] Los datos deben ser almacenado y respaldados por el equipo de backend
8. [] Los datos son calculados por el front-end
9. [] Investigar sobre librerias de procesamientos de datos para mostrarlo
10. [] Generar un panel de visualización estilo Dashboard
11. [] input de entradas de datos sobre consumos, servicios usados y los gastos.
12. [] input de entradas de los equipos y procesos que afecten
13. [] determinar como completar los campos, que prioridades o como organizarlo
14. [] Debemos construir medidas de KPI, indicador clave rendimiento, los cual podrán ser 
    1 - PEE propuesta de eficiencia de mejoras
    2 - PAE propuesta de actualización de equipos
    2 - PCE Propuesta de cultura de eficiencia

{
  "informeID": "0c72b2f9b1e8a5f4b2f4d5",
  "consumos": {
    "electricidad": {
      "enero": "123KWH",
      "febrero": "123KWH",
      "marzo": "123KWH"
    },
    "gas": {
      "enero": "50m³",
      "febrero": "45m³",
      "marzo": "55m³"
    }
  }
}

{
  "dispositivos": [
    {
      "tipo": "Iluminación",
      "nombre": "Foco",
      "Consumo_nominal_Equipo": 100,
      "Unidad_de_medida": "wht",
      "Cantidad_de_equipos": 2,
      "Factor_de_carga": 60,
      "Rendimiento": "X",
      "Horas_de_uso": 100,
      "Energia_Secundaria_Consumida": (100 * 2 * 60 / 100 * 100) / 1000,
      "Energia_Util_Consumida": (100 * 2 * 60 / 100 * 100 * X / 100) / 1000,
      "Unidad": "Kwh"
    },
    {
      "tipo": "Electrodoméstico",
      "nombre": "Heladera",
      "Consumo_nominal_Equipo": 150,
      "Unidad_de_medida": "wht",
      "Cantidad_de_equipos": 1,
      "Factor_de_carga": 80,
      "Rendimiento": "Y",
      "Horas_de_uso": 200,
      "Energia_Secundaria_Consumida": (150 * 1 * 80 / 100 * 200) / 1000,
      "Energia_Util_Consumida": (150 * 1 * 80 / 100 * 200 * Y / 100) / 1000,
      "Unidad": "Kwh"
    },
    {
      "tipo": "Electrodoméstico",
      "nombre": "Ventilador",
      "Consumo_nominal_Equipo": 50,
      "Unidad_de_medida": "wht",
      "Cantidad_de_equipos": 3,
      "Factor_de_carga": 50,
      "Rendimiento": "Z",
      "Horas_de_uso": 150,
      "Energia_Secundaria_Consumida": (50 * 3 * 50 / 100 * 150) / 1000,
      "Energia_Util_Consumida": (50 * 3 * 50 / 100 * 150 * Z / 100) / 1000,
      "Unidad": "Kwh"
    },
    {
      "tipo": "Electrodoméstico",
      "nombre": "Aire Acondicionado",
      "Consumo_nominal_Equipo": 2000,
      "Unidad_de_medida": "wht",
      "Cantidad_de_equipos": 1,
      "Factor_de_carga": 70,
      "Rendimiento": "W",
      "Horas_de_uso": 300,
      "Energia_Secundaria_Consumida": (2000 * 1 * 70 / 100 * 300) / 1000,
      "Energia_Util_Consumida": (2000 * 1 * 70 / 100 * 300 * W / 100) / 1000,
      "Unidad": "Kwh"
    }
  ]
}

# PANEL DE ADMINISTRACIÓN
1. [] Este panel es nuesto, cuenta con cuestiones administrativas
2. [] Nuestro panel nos deberia permitir
    a. chequeo de pagos recibido
    b. cantidad de informes realizado, en tramites y en espera
    c. lectura y envio de correos oficiales

 {
  "informeID": "0c72b2f9b1e8a5f4b2f4d5",
  "clienteId": "0c72b2f9b1e8a5f4c2f1d4",
  "nombre": "Julian Alvarez",
  "tipoCliente": "Industria",
  "direccion": "Calle 15 y ruta 40",
  "consultorAsignado": [
    "60c72b2f9b1e8a5f4d3f4d3f",
    "60c72b2f9b1e8a5f4d1f2d4f",
    "60c72b2f9b1e8a5f4d3f4d7f"
  ]
}

# CONSULTAS A LOS CONSULTORES
1. [] ¿Como se gestionarian los informes?
2. [] ¿Como serian las tarifas de esos servicios de Gestoria energética?
3. [] ¿Como tendria que hacer el sistema para evaluar a los candidatos dependiendo del proyecto?
4. [] ¿Hay que reconocer viaticos?
5. [] Evaluación de la logica de los informes
6. [] El portal se necesita certificaciones nacionales para poder operar en pyme y grandes industrias, o solamente los gestores