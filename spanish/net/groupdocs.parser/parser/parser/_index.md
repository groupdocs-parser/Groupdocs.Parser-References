---
title: Parser
second_title: Referencia de API de GroupDocs.Parser para .NET
description: Inicializa una nueva instancia delParsergroupdocs.parser/parser clase para extraer datos de una base de datos.
type: docs
weight: 10
url: /es/net/groupdocs.parser/parser/parser/
---
## Parser(DbConnection) {#constructor_2}

Inicializa una nueva instancia del[`Parser`](../../parser) clase para extraer datos de una base de datos.

```csharp
public Parser(DbConnection connection)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| connection | DbConnection | La conexión de la base de datos. |

### Observaciones

**Aprende más:**

* [Extraer datos de bases de datos.](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)

### Ejemplos

El siguiente ejemplo muestra cómo extraer datos de la base de datos Sqlite:

```csharp
// Crear objeto DbConnection
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// Crear una instancia de la clase Parser para extraer tablas de la base de datos
using (Parser parser = new Parser(connection))
{
    // Comprobar si se admite la extracción de texto
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // Comprobar si se admite la extracción de toc
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // Obtener una lista de tablas
    IEnumerable<TocItem> toc = parser.GetToc();
    // Iterar sobre tablas
    foreach (TocItem i in toc)
    {
        // Imprime el nombre de la tabla
        Console.WriteLine(i.Text);
        // Extrae el contenido de una tabla como texto
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Ver también

* class [Parser](../../parser)
* espacio de nombres [GroupDocs.Parser](../../parser)
* asamblea [GroupDocs.Parser](../../../)

---

## Parser(DbConnection, ParserSettings) {#constructor_3}

Inicializa una nueva instancia del[`Parser`](../../parser) clase para extraer datos de una base de datos.

```csharp
public Parser(DbConnection connection, ParserSettings parserSettings)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| connection | DbConnection | La conexión de la base de datos. |
| parserSettings | ParserSettings | La configuración del analizador que se utiliza para personalizar la extracción de datos. |

### Observaciones

**Aprende más:**

* [Extraer datos de bases de datos.](https://docs.groupdocs.com/display/parsernet/Extract+data+from+databases)
* [Inicio sesión](https://docs.groupdocs.com/display/parsernet/Logging)

### Ejemplos

El siguiente ejemplo muestra cómo extraer datos de la base de datos Sqlite:

```csharp
// Crear objeto DbConnection
DbConnection connection = new SQLiteConnection(string.Format("Data Source={0};Version=3;", Constants.SampleDatabase));
// Crear una instancia de la clase Parser para extraer tablas de la base de datos
using (Parser parser = new Parser(connection))
{
    // Comprobar si se admite la extracción de texto
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    // Comprobar si se admite la extracción de toc
    if (!parser.Features.Toc)
    {
        Console.WriteLine("Toc extraction isn't supported.");
        return;
    }
    // Obtener una lista de tablas
    IEnumerable<TocItem> toc = parser.GetToc();
    // Iterar sobre tablas
    foreach (TocItem i in toc)
    {
        // Imprime el nombre de la tabla
        Console.WriteLine(i.Text);
        // Extrae el contenido de una tabla como texto
        using (TextReader reader = parser.GetText(i.PageIndex.Value))
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
```

### Ver también

* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* espacio de nombres [GroupDocs.Parser](../../parser)
* asamblea [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection) {#constructor}

Inicializa una nueva instancia del[`Parser`](../../parser) clase para extraer datos de un servidor de correo electrónico remoto.

```csharp
public Parser(EmailConnection connection)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| connection | EmailConnection | La conexión de correo electrónico. |

### Observaciones

**Aprende más:**

* [Extraiga correos electrónicos del servidor remoto a través de los protocolos POP, IMAP o Exchange Web Services](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)

### Ejemplos

El siguiente ejemplo muestra cómo extraer correos electrónicos de Exchange Server:

```csharp
// Crear el objeto de conexión para el protocolo de servicios web de Exchange 
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// Crear una instancia de la clase Parser para extraer correos electrónicos del servidor remoto
using (Parser parser = new Parser(connection))
{
    // Comprobar si se admite la extracción de contenedores
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// Extraer mensajes de correo electrónico del servidor
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // Iterar sobre adjuntos
    foreach (ContainerItem item in emails)
    {
        // Crea una instancia de la clase Parser para el mensaje de correo electrónico
        using (Parser emailParser = item.OpenParser())
        {
            // Extraer el texto del correo electrónico
            using (TextReader reader = emailParser.GetText())
            {
                // Imprimir el texto del correo electrónico
                Console.WriteLine(reader == null ? "Text extraction isn't supported." : reader.ReadToEnd());
            }
        }
    }
}   
```

### Ver también

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [Parser](../../parser)
* espacio de nombres [GroupDocs.Parser](../../parser)
* asamblea [GroupDocs.Parser](../../../)

---

## Parser(EmailConnection, ParserSettings) {#constructor_1}

Inicializa una nueva instancia del[`Parser`](../../parser) clase para extraer datos de un servidor de correo electrónico remoto.

```csharp
public Parser(EmailConnection connection, ParserSettings parserSettings)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| connection | EmailConnection | La conexión de correo electrónico. |
| parserSettings | ParserSettings | La configuración del analizador que se utiliza para personalizar la extracción de datos. |

### Observaciones

**Aprende más:**

* [Extraiga correos electrónicos del servidor remoto a través de los protocolos POP, IMAP o Exchange Web Services](https://docs.groupdocs.com/display/parsernet/Extract+emails+from+remote+server+via+POP%2C+IMAP+or+Exchange+Web+Services+protocols)
* [Inicio sesión](https://docs.groupdocs.com/display/parsernet/Logging)

### Ejemplos

El siguiente ejemplo muestra cómo extraer correos electrónicos de Exchange Server:

```csharp
// Crear el objeto de conexión para el protocolo de servicios web de Exchange 
EmailConnection connection = new EmailEwsConnection(
    "https://outlook.office365.com/ews/exchange.asmx",
    "email@server",
    "password");
 
// Crear una instancia de la clase Parser para extraer correos electrónicos del servidor remoto
using (Parser parser = new Parser(connection))
{
    // Comprobar si se admite la extracción de contenedores
    if (!parser.Features.Container)
    {
        Console.WriteLine("Container extraction isn't supported.");
        return;
    }

// Extraer mensajes de correo electrónico del servidor
IEnumerable<ContainerItem> emails = parser.GetContainer();
 
    // Iterar sobre adjuntos
    foreach (ContainerItem item in emails)
    {
        // Crea una instancia de la clase Parser para el mensaje de correo electrónico
        using (Parser emailParser = item.OpenParser())
        {
            // Extraer el texto del correo electrónico
            using (TextReader reader = emailParser.GetText())
            {
                // Imprimir el texto del correo electrónico
                Console.WriteLine(reader == null ? "Text extraction isn't supported." : reader.ReadToEnd());
            }
        }
    }
}   
```

### Ver también

* class [EmailConnection](../../../groupdocs.parser.options/emailconnection)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* espacio de nombres [GroupDocs.Parser](../../parser)
* asamblea [GroupDocs.Parser](../../../)

---

## Parser(string) {#constructor_7}

Inicializa una nueva instancia del[`Parser`](../../parser) clase.

```csharp
public Parser(string filePath)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| filePath | String | La ruta al archivo. |

### Observaciones

**Aprende más:**

* [Cargar documento desde disco local](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Ejemplos

El siguiente ejemplo muestra cómo cargar el documento desde el disco local:

```csharp
// Crear una instancia de la clase Parser con filePath
using (Parser parser = new Parser(filePath))
{
    // Extraer un texto en el lector
    using (TextReader reader = parser.GetText())
    {
        // Imprime un texto del documento
        // Si no se admite la extracción de texto, un lector es nulo
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Ver también

* class [Parser](../../parser)
* espacio de nombres [GroupDocs.Parser](../../parser)
* asamblea [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions) {#constructor_8}

Inicializa una nueva instancia del[`Parser`](../../parser) clase con[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) .

```csharp
public Parser(string filePath, LoadOptions loadOptions)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| filePath | String | La ruta al archivo. |
| loadOptions | LoadOptions | Las opciones para abrir el archivo. |

### Observaciones

**Aprende más:**

* [Cargar formatos de archivo específicos](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Carga de documentos protegidos con contraseña](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Cargar documento desde disco local](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Ejemplos

La contraseña del documento es pasada por la clase LoadOptions:

```csharp
try
{
    // Crea una instancia de la clase Parser con la contraseña:
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // Comprobar si se admite la extracción de texto
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Imprime el texto del documento
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    // Imprimir el mensaje si la contraseña es incorrecta o está vacía
    Console.WriteLine("Invalid password");
}
```

### Ver también

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* espacio de nombres [GroupDocs.Parser](../../parser)
* asamblea [GroupDocs.Parser](../../../)

---

## Parser(string, LoadOptions, ParserSettings) {#constructor_9}

Inicializa una nueva instancia del[`Parser`](../../parser) clase con[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) y[`ParserSettings`](../../../groupdocs.parser.options/parsersettings) .

```csharp
public Parser(string filePath, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| filePath | String | La ruta al archivo. |
| loadOptions | LoadOptions | Las opciones para abrir el archivo. |
| parserSettings | ParserSettings | La configuración del analizador que se utiliza para personalizar la extracción de datos. |

### Observaciones

**Aprende más:**

* [Cargar formatos de archivo específicos](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Carga de documentos protegidos con contraseña](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Inicio sesión](https://docs.groupdocs.com/display/parsernet/Logging)
* [Cargar documento desde disco local](https://docs.groupdocs.com/display/parsernet/Load+document+from+local+disk)

### Ejemplos

El siguiente ejemplo muestra cómo recibir la información a través de[`ILogger`](../../../groupdocs.parser.options/ilogger) interfaz:

```csharp
// probar
{
    // Crea una instancia de la clase Logger
    Logger logger = new Logger();
    // Crea una instancia de la clase Parser con la configuración del analizador
    using (Parser parser = new Parser(filePath, null, new ParserSettings(logger)))
    {
        // Comprobar si se admite la extracción de texto
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Imprime el texto del documento
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    ; // Ignorar la excepción
}
 
private class Logger : ILogger
{
    public void Error(string message, Exception exception)
    {
        // Imprimir mensaje de error
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // Imprimir mensaje de evento
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // Imprimir mensaje de advertencia
        Console.WriteLine("Warning: " + message);
    }
}
```

### Ver también

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* espacio de nombres [GroupDocs.Parser](../../parser)
* asamblea [GroupDocs.Parser](../../../)

---

## Parser(Stream) {#constructor_4}

Inicializa una nueva instancia del[`Parser`](../../parser) clase.

```csharp
public Parser(Stream document)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| document | Stream | El flujo de entrada de origen. |

### Observaciones

**Aprende más:**

* [Cargar documento desde flujo](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### Ejemplos

El siguiente ejemplo muestra cómo cargar el documento desde la secuencia:

```csharp
// Crea una instancia de la clase Parser con la transmisión
using (Parser parser = new Parser(stream))
{
    // Extraer un texto en el lector
    using (TextReader reader = parser.GetText())
    {
        // Imprime un texto del documento
        // Si no se admite la extracción de texto, un lector es nulo
        Console.WriteLine(reader == null ? "Text extraction isn't supported" : reader.ReadToEnd());
    }
}
```

### Ver también

* class [Parser](../../parser)
* espacio de nombres [GroupDocs.Parser](../../parser)
* asamblea [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions) {#constructor_5}

Inicializa una nueva instancia del[`Parser`](../../parser) clase con[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) .

```csharp
public Parser(Stream document, LoadOptions loadOptions)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| document | Stream | El flujo de entrada de origen. |
| loadOptions | LoadOptions | Las opciones para abrir el archivo. |

### Observaciones

**Aprende más:**

* [Cargar formatos de archivo específicos](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Carga de documentos protegidos con contraseña](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Cargar documento desde flujo](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)

### Ejemplos

En algunos casos es necesario definir[`FileFormat`](../../../groupdocs.parser.options/fileformat). Tanto para casos especiales (bases de datos, servidor de correo) como para detectar tipos de archivos por el contenido:

La contraseña del documento es pasada por[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) clase:

```csharp
// Crear una instancia de la clase Parser para el documento de rebajas
using (Parser parser = new Parser(stream, new LoadOptions(FileFormat.Markup)))
{
    // Comprobar si se admite la extracción de texto
    if (!parser.Features.Text)
    {
        Console.WriteLine("Text extraction isn't supported.");
        return;
    }
    using (TextReader reader = parser.GetText())
    {
        // Imprime el texto del documento
        // Se detecta rebaja; se imprime texto sin símbolos especiales
        Console.WriteLine(reader.ReadToEnd());
    }
}
```

```csharp
try
{
    // Crea una instancia de la clase Parser con la contraseña:
    using (Parser parser = new Parser(filePath, new LoadOptions(password)))
    {
        // Comprobar si se admite la extracción de texto
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Imprime el texto del documento
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    // Imprimir el mensaje si la contraseña es incorrecta o está vacía
    Console.WriteLine("Invalid password");
}
```

### Ver también

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [Parser](../../parser)
* espacio de nombres [GroupDocs.Parser](../../parser)
* asamblea [GroupDocs.Parser](../../../)

---

## Parser(Stream, LoadOptions, ParserSettings) {#constructor_6}

Inicializa una nueva instancia del[`Parser`](../../parser) clase con[`LoadOptions`](../../../groupdocs.parser.options/loadoptions) y[`ParserSettings`](../../../groupdocs.parser.options/parsersettings) .

```csharp
public Parser(Stream document, LoadOptions loadOptions, ParserSettings parserSettings)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| document | Stream | El flujo de entrada de origen. |
| loadOptions | LoadOptions | Las opciones para abrir el archivo. |
| parserSettings | ParserSettings | La configuración del analizador que se utiliza para personalizar la extracción de datos. |

### Observaciones

**Aprende más:**

* [Cargar formatos de archivo específicos](https://docs.groupdocs.com/display/parsernet/Loading+specific+file+formats)
* [Carga de documentos protegidos con contraseña](https://docs.groupdocs.com/display/parsernet/Password-protected+documents)
* [Cargar documento desde flujo](https://docs.groupdocs.com/display/parsernet/Load+document+from+stream)
* [Inicio sesión](https://docs.groupdocs.com/display/parsernet/Logging)

### Ejemplos

El siguiente ejemplo muestra cómo recibir la información a través de[`ILogger`](../../../groupdocs.parser.options/ilogger) interfaz:

```csharp
// probar
{
    // Crea una instancia de la clase Logger
    Logger logger = new Logger();
    // Crea una instancia de la clase Parser con la configuración del analizador
    using (Parser parser = new Parser(stream, null, new ParserSettings(logger)))
    {
        // Comprobar si se admite la extracción de texto
        if (!parser.Features.Text)
        {
            Console.WriteLine("Text extraction isn't supported.");
            return;
        }
        // Imprime el texto del documento
        using (TextReader reader = parser.GetText())
        {
            Console.WriteLine(reader.ReadToEnd());
        }
    }
}
catch (InvalidPasswordException)
{
    ; // Ignorar la excepción
}
 
private class Logger : ILogger
{
    public void Error(string message, Exception exception)
    {
        // Imprimir mensaje de error
        Console.WriteLine("Error: " + message);
    }
    public void Trace(string message)
    {
        // Imprimir mensaje de evento
        Console.WriteLine("Event: " + message);
    }
    public void Warning(string message)
    {
        // Imprimir mensaje de advertencia
        Console.WriteLine("Warning: " + message);
    }
}
```

### Ver también

* class [LoadOptions](../../../groupdocs.parser.options/loadoptions)
* class [ParserSettings](../../../groupdocs.parser.options/parsersettings)
* class [Parser](../../parser)
* espacio de nombres [GroupDocs.Parser](../../parser)
* asamblea [GroupDocs.Parser](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for GroupDocs.Parser.dll -->
