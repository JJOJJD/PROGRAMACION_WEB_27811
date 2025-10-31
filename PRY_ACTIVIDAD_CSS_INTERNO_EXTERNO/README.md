#Actividad CSS Interno y Externo


## Instrucciones de Ejecución

### Método 1: CSS Externo (externo.html)
1. Abre el archivo `view/externo.html` en tu navegador web
2. El archivo carga automáticamente los estilos desde `Public/css/estilos.css`
3. Observa el formulario estilizado mediante CSS externo

### Método 2: CSS Interno (interno.html)
1. Abre el archivo `view/interno.html` en tu navegador web
2. Los estilos están definidos dentro del mismo archivo HTML en la etiqueta `<style>`
3. Observa el formulario estilizado mediante CSS interno

### Requisitos
- Navegador web moderno (Chrome, Firefox, Edge, Safari)
- No se requiere servidor web, puedes abrir los archivos directamente

## Estructura del Proyecto
```
PRY_ACTIVIDAD_CSS_INTERNO_EXTERNO/
│
├── view/
│   ├── externo.html          # Formulario con CSS externo
│   └── interno.html          # Formulario con CSS interno
│
├── Public/
│   └── css/
│       └── estilos.css       # Hoja de estilos externa
│
└── README.md                 # Este archivo
```

##  Propiedades CSS Utilizadas

### **Archivo: externo.html** (CSS Externo)
Los estilos se definen en `Public/css/estilos.css`:

#### 1. **input[type="text"]** - Campo de texto
| Propiedad | Valor | Descripción |

| `border-radius` | 8px | **Redondea las esquinas** del campo de texto para un aspecto más suave y moderno 
| `padding` | 5px | **Añade espacio interno** entre el borde y el texto escrito, mejorando la legibilidad 
| `letter-spacing` | 5px | **Separa las letras** entre sí, dando un aspecto espaciado al texto ingresado 
| `border` | 2px solid #4a90e2 | **Define un borde** de 2px sólido en color azul alrededor del campo |
| `width` | 300px | **Establece el ancho fijo** del campo de texto en 300 píxeles |

#### 2. **textarea** - Área de texto
| Propiedad | Valor | Descripción |

| `border-radius` | 15px | **Redondea las esquinas** del área de texto con un radio más pronunciado |
| `background-color` | #89e8f5 | **Establece el color de fondo** en un tono azul claro/cian |
| `border-color` | rgb(69, 40, 235) | **Define el color del borde** en un azul púrpura |
| `resize` | none | **Deshabilita el redimensionamiento** manual del textarea por parte del usuario |
| `overflow-wrap` | break-word | **Permite que las palabras largas** se dividan y ajusten dentro del contenedor |

#### 3. **select** - Menú desplegable
| Propiedad | Valor | Descripción |

| `border-radius` | 8px | **Redondea las esquinas** del elemento select |
| `font-variant` | small-caps | **Convierte el texto** a versalitas (mayúsculas pequeñas) |
| `margin` | 5px | **Añade espacio externo** alrededor del elemento para separarlo de otros |
| `background-color` | #fff | **Establece el fondo blanco** para el menú desplegable |
| `appearance` | none | **Elimina el estilo predeterminado** del navegador para personalizar el select |

#### 4. **input[type="checkbox"]** - Casillas de verificación
| Propiedad | Valor | Descripción |

| `border-radius` | 4px | **Redondea ligeramente** las esquinas de las casillas |
| `cursor` | pointer | **Cambia el cursor** a una mano indicando que el elemento es clickeable |
| `width` | 18px | **Establece el ancho** de las casillas en 18 píxeles |
| `height` | 18px | **Establece la altura** de las casillas en 18 píxeles |
| `outline` | 2px solid #d17015 | **Añade un contorno** naranja alrededor de la casilla cuando está enfocada |

#### 5. **input[type="radio"]** - Botones de radio
| Propiedad | Valor | Descripción |

| `border-radius` | 50% | **Hace el botón circular** aplicando un radio del 50% |
| `box-shadow` | 0 0 10px 5px rgba(231, 8, 8, 0.2) inset | **Añade una sombra interna** roja suave, creando efecto de profundidad |
| `width` | 20px | **Establece el ancho** del botón radio en 20 píxeles |
| `height` | 20px | **Establece la altura** del botón radio en 20 píxeles |
| `transform` | rotate(0deg) | **Aplica una transformación** de rotación (aunque está en 0 grados, permite rotación futura) |

---

### **Archivo: interno.html** (CSS Interno)
Los estilos se definen dentro de la etiqueta `<style>` en el mismo archivo HTML:

#### 1. **input[type="text"]** - Campo de texto
| Propiedad | Valor | Descripción |

| `border-radius` | 15px | **Redondea las esquinas** con un radio más pronunciado que en externo.html |
| `padding` | 5px | **Añade espacio interno** entre el borde y el texto |
| `caret-color` | #df2db2 | **Cambia el color del cursor** de escritura (|) a un tono rosado/fucsia |

#### 2. **textarea** - Área de texto
| Propiedad | Valor | Descripción |

| `border-radius` | 15px | **Redondea las esquinas** del área de texto |
| `text-decoration` | underline | **Añade una línea subrayada** debajo del texto ingresado |
| `font-family` | 'Times New Roman', Times, serif | **Establece una fuente serif** clásica y formal para el texto |

#### 3. **select** - Menú desplegable
| Propiedad | Valor | Descripción |

| `border-radius` | 8px | **Redondea las esquinas** del elemento select |
| `border` | 2px solid #1c72d4 | **Define un borde** azul sólido de 2 píxeles |
| `text-transform` | uppercase | **Convierte automáticamente** todo el texto a mayúsculas |

#### 4. **input[type="checkbox"]** - Casillas de verificación
| Propiedad | Valor | Descripción |

| `border-radius` | 4px | **Redondea ligeramente** las esquinas de las casillas |
| `accent-color` | #dd521b | **Establece el color** de la marca de verificación cuando está seleccionada (naranja) |

#### 5. **input[type="radio"]** - Botones de radio
| Propiedad | Valor | Descripción |

| `border-radius` | 50% | **Hace el botón circular** aplicando un radio del 50% |
| `transform` | scale(1.5) | **Aumenta el tamaño** del botón radio al 150% de su tamaño original |

