# Flujo de Trabajo Colaborativo - Entrega de Prácticas

A continuación se detalla el ciclo de trabajo que seguiré para la entrega de cada práctica del curso utilizando GitHub:

```mermaid
graph TD
    A[Inicio: Abrir terminal en el repositorio local] --> B(git pull <br> <i>Traer últimos cambios para evitar conflictos</i>)
    B --> C(Crear carpeta de la práctica <br> <i>Ej: Practica_01_Python</i>)
    C --> D(Desarrollar la práctica <br> <i>Crear y modificar archivos</i>)
    D --> E(git add . <br> <i>Preparar/Registrar los cambios locales</i>)
    E --> F(git commit -m 'Mensaje de entrega' <br> <i>Confirmar cambios localmente</i>)
    F --> G(git push <br> <i>Enviar archivos al repositorio en GitHub</i>)
    G --> H[Verificar en GitHub]
    H -.-> I{¿Es antes de la fecha límite?}
    I -- Sí --> J((Enviar enlace al docente))
    I -- No --> K((Entrega fuera de plazo))
    
    style J fill:#2ecc71,stroke:#27ae60,stroke-width:2px,color:black
    style K fill:#e74c3c,stroke:#c0392b,stroke-width:2px,color:white
