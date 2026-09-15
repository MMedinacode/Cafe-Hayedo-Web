# Café del Hayedo — Rancagua · dossier verificado

> Verificado **en vivo en Google Maps, Instagram y Spotify el 15-09-2026**.
> **Nada acá está inventado.**

## Ficha Google Maps

| Dato | Valor |
|---|---|
| Nombre | Café del Hayedo |
| Categoría | Cafetería |
| Dirección | Membrillar 50, Loc 2, Rancagua, O'Higgins |
| Plus Code | R7H8+FC Rancagua |
| Teléfono | ❌ **NO tiene** ("Añadir número de teléfono del sitio") |
| Rating | **5,0 ★** — el rating perfecto de toda la tanda |
| Nº reseñas | 23 |
| Rango de precio | $5.000–10.000 por persona (notificado por 11 personas) |
| Servicios | Consumo en el lugar · Para llevar · **Entrega a domicilio** |
| Sitio web | NO tiene |
| Ficha reclamada | ❌ **NO** — dice "Reclamar esta empresa" |
| Otros | "Amigable con LGBTQ+" |

```
Place ID  : ChIJ6a1vOgBFY5YRTaWDtAtgO2s
CID hex   : 0x966345003a6fade9:0x6b3b600bb483a54d
Coordenadas: -34.1713121, -70.73398
```

---

## 🎯 EL GANCHO: su carta de Google está rota

Su ficha publica un botón **"Carta"** que apunta a Google Drive:

```
https://drive.google.com/file/d/1mUuKW8bHqHPx46b9vLXM7qQjP-mGstOr/view
```

**Está muerto.** Verificado dos veces, el 15-09-2026:

```
$ curl -o /dev/null -w "%{http_code}" https://drive.google.com/file/d/1mUu.../view
404
```

Y el mensaje que ve el cliente es **"Lo sentimos, el archivo que has
solicitado no existe"** — o sea **no es un problema de permisos**, el
archivo se borró o se movió. Cualquiera que haga clic en "Carta" desde
Google se topa con una página de error de Google.

> Es el mismo gancho que Kei Pastelería (su menú me-qr daba 404), pero acá
> es peor: **ese link es lo único que Google muestra como su carta.**

### Y el contraste que lo remata

El **único link de su bio de Instagram sí funciona**… y es una **playlist
de Spotify**:

```
tinyurl.com/Playlistdelhayedo → open.spotify.com/playlist/0JdZNand9zSd0FTIrzscPE
"Café del Hayedo PM", de Esteban Fagalde — HTTP 200 ✅
```

**Su playlist funciona. Su carta no.** Ese es el mensaje de outreach, y no
hay que adornarlo.

---

## Horario

| Día | Horario |
|---|---|
| Lunes a viernes | 08:00 – 17:00 |
| Sábado | **Cerrado** |
| Domingo | **Cerrado** |

```js
window.HORARIO = {
  dias: ["08:00 - 17:00","08:00 - 17:00","08:00 - 17:00","08:00 - 17:00",
         "08:00 - 17:00","Cerrado","Cerrado"],
  fuente: "Ficha de Google Maps, 15-09-2026"
};
```

⚠️ **Advertencia honesta sobre este dato:** la semana consultada cae en
**Fiestas Patrias**, y Google anota "El horario podría cambiar" en viernes
19 y sábado 20. El viernes igual aparece con su horario normal (8–17), así
que la anotación parece genérica y no una excepción cargada por el local.
Aun así, **el sábado conviene confirmarlo con ellos** antes de mandar el
mensaje.

**Es un café de días de semana.** Cierra a las 17:00 y no abre fin de
semana: encaja con la zona (Membrillar 50 está entre oficinas) y con que
sus reseñas hablen de **desayuno** y **estacionamiento gratuito**.

## 📱 Instagram VERIFICADO

**`@cafedelhayedo`** — **2.264 seguidores · 128 seguidos**.

Su bio, textual:

> "Buen café, **bollería, pastelería, helados artesanales y sándwiches
> gourmet**. ¡Visitanos!"

Esa línea es la única fuente de categorías de carta que tienen publicada,
así que la carta del sitio se arma sobre ella.

## Identidad: el haya, la pizarra y la playlist

- **El nombre.** Un *hayedo* es un bosque de hayas. Y la madera de haya es
  exactamente esa madera rubia clara de sus mesas — el nombre y el material
  coinciden. Es el eje visual.
- **La pizarra de letras.** Su carta de bebidas es un **letter board**
  gris grafito con letras blancas encajadas a mano. Es su objeto de marca
  más reconocible y el motivo gráfico del sitio.
- **La loza azul porcelana.** Platos y tazas de un azul pálido que se
  repite en todas sus fotos.
- **La música.** Su único link de bio es una playlist, y una reseña
  destaca "muy limpio, **buena música**". No es decorado: les importa.

→ **Paleta muestreada con Pillow de sus propias fotos:**

| Variable | Hex | De dónde salió |
|---|---|---|
| `--pizarra` | `#343943` | su letter board |
| `--haya` | `#D8B285` | la madera de sus mesas |
| `--porcelana` | `#C5DBE5` | sus platos y tazas |
| `--crema` | `#F6F3EC` | sus paredes |

> ⚠️ **Diferenciación:** Río Deva usa azul pizarra `#1C3A4F` + latón, pero
> ese sitio es **oscuro y de anticuario**. Éste es **claro y nórdico**: el
> grafito es la tinta, no el fondo, y el acompañante es madera rubia, no
> oro. Ninguno de los cuatro hex está usado en el portafolio (verificado
> por grep sobre los 60 `styles.css`).

**Tipografía: Brygada 1918 + Golos Text + Questrial.** Las tres verificadas
como no usadas (grep sobre todos los `index.html`). Questrial va en
versalitas espaciadas para imitar las letras de su pizarra.

---

## 💰 Carta con PRECIOS REALES

Su pizarra está fotografiada en su propia ficha. Transcrita de la foto
(`fotos/pizarra-precios.jpg`), a resolución 2× :

| Bebida | Precio |
|---|---|
| Espresso | $2.000 |
| Americano | $2.500 |
| Flat white | $2.990 |
| Capuccino | $3.200 |
| Capuccino vainilla | $3.700 |
| Latte | $3.500 |
| Latte caramelo / vainilla | $3.900 |
| **Mokaccino** | ⚠️ **sin precio en la pizarra** |
| Chocolate | $4.200 |
| Chai latte | $3.500 |
| Dirty chai | $3.900 |
| Jugos | $3.800 |
| Café helado | $6.000 |

⚠️ **Mokaccino aparece en la pizarra sin precio asignado** (la casilla está
vacía). Va como "Consultar" — no se le inventa un valor.

⚠️ **Sólo hay precios de bebidas.** De bollería, pastelería, helados y
sándwiches no hay ni uno publicado: esos van sin precio, con el motivo
escrito en la propia página.

### Productos confirmados (sin precio)

De su bio, sus fotos y sus reseñas:

- **Bollería** — croissants, caracolas y hojaldres (se ven en la vitrina)
- **Pastelería** — tortas por porción, **macarons** (Google los extrae como
  tema de sus reseñas), tortas enteras
- **Helados artesanales** — de su bio
- **Sándwiches gourmet** — de su bio; en una foto hay uno con jamón
  serrano y albahaca
- **Desayunos** — Diego Aliaga marcó su visita como "Tipo de comida:
  Desayuno"
- **Puré natural** — *"puré natural 10/10"* (Maite Baker)

## Reseñas reales — 3 de 3, todas 5★

1. **Maite Baker** — Local Guide · 10 reseñas · hace 5 meses
   > Rico café, atención agradable y muy amable. La comida estaba
   > deliciosa, puré natural 10/10. Muy recomendado

2. **Diego Aliaga** — Local Guide · 74 reseñas · hace un año
   > Es una excelente cafetería que se diferencia bastante de las demás,
   > tienen productos muy buenos y demasiado deliciosos, además sus
   > ingredientes son de bastante calidad, el café es buenísimo, e ido a
   > varias cafeterías tanto de Santiago, rancagua y el sur y está esta es
   > buenísima por sobre muchas igual **todo es preparado en el momento con
   > ingredientes frescos**. La recomiendo totalmente a todos.

3. **Arantxa Araya** — Local Guide · 24 reseñas · hace un año
   > Un latte de caramelo delicioso 🙂‍↔️ **en la vitrina tienen lleno de
   > cositas ricas**, me encantó

### Los datos extra de Diego Aliaga (valen oro)

En su reseña llenó los campos opcionales, y eso da hechos verificables que
normalmente hay que preguntarle al local:

- **Platos vegetarianos:** *"Tiene todas las opciones y pronto irán
  añadiendo más"*
- **Estacionamiento:** *"Estacionamiento gratuito"* · *"Es fácil llegar en
  auto sin problemas, sin pago"*
- **Adecuado para niños:** *"Totalmente, el espacio es cómodo, muy limpio
  buena música, muy recomendable para ir con la familia"*
- **Accesibilidad en silla de ruedas:** *"Es de fácil acceso y de espacio
  amplio, muy cómoda"*

**Temas que Google extrae de sus reseñas:** postres (3), macarrones (2),
chocolate caliente (2), rico (2), latte (2).

**Sin una sola reseña negativa** en las 23. Y **sin red flags**: Google no
marca opiniones sospechosas.

## Fotos reales → `fotos/` (5 usables)

Bajadas a 2000px y revisadas en hoja de contacto.

| Archivo | Qué es |
|---|---|
| `hero-cafe-helado.jpg` | **Café helado + torta de chocolate y naranja**, con una planta detrás — es el hero |
| `vitrina.jpg` | Su vitrina entera: croissants, hojaldres, macarons, torta |
| `mesa-compartida.jpg` | Mesa con sándwich de serrano, capuchino, latte y croissant |
| `pizarra-precios.jpg` | **La pizarra del menú con los precios** |
| `espresso.jpg` | Macro del espresso cayendo a la taza |

- En `mesa-compartida.jpg` **sólo se ven manos**, ninguna cara. Pasa.
- ⚠️ **No hay foto del salón ni de la fachada** más allá del Street View de
  Google (que no se baja: no es material del local). Igual que en Dulce
  Pols, conviene pedírsela.

## Lo que falta por verificar

- [ ] **Teléfono / WhatsApp**: no publican ninguno, en ningún canal.
- [ ] **Sábado**: confirmar si de verdad cierran (ver advertencia arriba).
- [ ] **TikTok**: no buscado.
- [ ] **Precio del mokaccino** y de todo lo que no sea bebida.
- [ ] **Una foto del salón.**
- [ ] Si "Esteban Fagalde" (dueño de la playlist) es el dueño del local —
      sería el nombre con el que abrir el mensaje.
