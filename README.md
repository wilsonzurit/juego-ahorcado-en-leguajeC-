# Juego del Ahorcado 🎮

Juego de ahorcado desarrollado en C# con Windows Forms y .NET 8.0. Usa sonido y una API para obtener palabras aleatorias; no requiere carpeta `datos` en el repositorio.

## Características ✨

- 🎵 Efectos de sonido para aciertos y errores
- 🖼️ Interfaz gráfica de escritorio con Windows Forms
- 🌐 Obtiene palabras aleatorias de una API externa
- 🎯 Control de vidas, letras intentadas y progreso de la palabra
- 🧠 Fallback local: usa "PROGRAMACION" si la API no responde

## Requisitos 📋

- .NET 8.0 SDK o superior
- Windows
- Dependencia NAudio 2.3.0

## Instalación 🚀

1. Clona el repositorio:
```bash
git clone https://github.com/tu-usuario/juego_ahorcado.git
cd juego_ahorcado
```

2. Restaura las dependencias:
```bash
dotnet restore
```

3. Compila el proyecto:
```bash
dotnet build
```

4. Ejecuta la aplicación:
```bash
dotnet run
```

## Estructura del proyecto 📁

```
juego_ahorcado/
├── Program.cs
├── juego_ahorcado.csproj
├── README.md
├── LICENSE
├── .gitignore
├── bin/                  # Archivos compilados
│   └── Debug/net8.0-windows/
│       ├── audio/        # Sonidos (.mpeg)
│       └── imagenes/     # Imágenes de la interfaz
└── obj/                  # Archivos de compilación
```

## Archivos importantes 🎵

- `ganoJuego.mpeg` — Sonido de victoria
- `perdioJuego.mpeg` — Sonido de derrota
- `tecleoCorrecto.mpeg` — Sonido de letra correcta
- `tecleoIncorrecto.mpeg` — Sonido de letra incorrecta

> Nota: no existe carpeta `datos`; el juego obtiene la palabra desde la API y usa `PROGRAMACION` cuando la API falla.

## Uso 🎲

1. Ejecuta el juego
2. Adivina la palabra leyendo la pista de letras
3. Selecciona letras en el teclado virtual
4. Evita perder todas las vidas

## Licencia 📄

Este proyecto se distribuye bajo la Licencia MIT. Consulta el archivo `LICENSE` para más detalles.

## Autor ✍️

Wilson Zurita Ugarte
