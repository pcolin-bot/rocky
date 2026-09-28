# ⚙️ 06. Especificaciones Técnicas de Producción y Pipeline de IA

## Manual de Ensamble Multimedia, Audio y Postproducción
* **Proyecto:** Miniserie "Sobreviviendo a Rogelio" (12 Micro-Episodios).
* **Compatibilidad de Pipeline:** Flow / Runway Gen-3 / Kling / Midjourney + Lip-Sync (Hedra/LivePortrait) / ElevenLabs / DaVinci Resolve / Premiere Pro.

---

### 1. Parámetros Técnicos de Video (Master Export)

| Parámetro | Especificación Requerida | Justificación Técnica |
| :--- | :--- | :--- |
| **Relación de Aspecto** | **9:16 Vertical** | Optimizado para consumo nativo en TikTok, Instagram Reels y YouTube Shorts. |
| **Resolución** | **1080 × 1920 px (Full HD Vertical)** | Estándar de nitidez en plataformas móviles sin compresión destructiva. |
| **Tasa de Cuadros (FPS)** | **24 fps ó 30 fps estables** | 24 fps para cadencia cinematográfica hiperrealista; 30 fps para fluidez estándar. |
| **Códec de Video** | **H.264 / MPEG-4 AVC (Perfil High)** | Máxima compatibilidad en navegadores y apps de redes sociales. |
| **Tasa de Bits (Bitrate)** | **15 Mbps a 20 Mbps (VBR 2 pases)** | Evita artefactos de pixelado en tomas con mucho movimiento (persecuciones). |
| **Duración por Episodio** | **18.5s a 19.2s (Media: 19.0s)** | Calibrado exacto para retención y loops algorítmicos. |
| **Espacio de Color** | **Rec.709 (Gamma 2.4)** | Rendimiento cromático equilibrado en pantallas OLED y LCD de celulares. |

---

### 2. Especificaciones de Audio y Síntesis Vocal (TTS / ElevenLabs)

#### A. Parámetros de Audio Master
* **Formato:** WAV 24-bit / 48 kHz (Export final en AAC Estéreo 320 kbps).
* **Nivel de Sonoridad (Loudness):** **-14 LUFS (Integrated)** con True Peak en **-1.0 dBTP** (Estándar para Meta y TikTok, evita distorsión del limitador de la plataforma).
* **Curva de Ecualización:** Realce sutil en presencia vocal (+2 dB en 3 kHz - 5 kHz) y corte de graves por debajo de 80 Hz para diálogos limpios en bocinas de celular.

#### B. Perfiles de Voz para Generación con IA (ElevenLabs / TTS)
* **Voz de Alex:**
  * *Género y Edad:* Femenina, ~28 años.
  * *Acento:* Mexicano neutro urbano contemporáneo (CDMX).
  * *Tono:* Juvenil, expresivo, emotivo, con capacidad de pasar de la ternura al pánico melodramático con rapidez.
  * *Ajustes ElevenLabs recomendados:* Stability: `0.45`, Clarity/Similarity: `0.80`, Style Exaggeration: `0.25`.
* **Voz de Sam:**
  * *Género y Edad:* Masculino, ~38 años.
  * *Acento:* Mexicano sobrio y relajado.
  * *Tono:* Grave, pausado, reconfortante, con una cadencia levemente irónica y resolutiva.
  * *Ajustes ElevenLabs recomendados:* Stability: `0.65`, Clarity/Similarity: `0.85`, Style Exaggeration: `0.10`.
* **Voz en Off Master (Cierre de Telenovela):**
  * *Género:* Masculino clásico de doblaje de telenovela mexicana / locución institucional cálida.
  * *Tono:* Envolvente, festivo, solemne pero pícaro.
  * *Texto de Cierre:* *«En los dramas de la vida real, tu tranquilidad está en WOOW. Porque con WOOW, ¡tooodo bien!»*

---

### 3. Librería y Cues de Diseño Sonoro (SFX & Foley)

Para acentuar el humor melodramático, cada micro-episodio lleva un paquete de efectos sonoros sincronizados al fotograma:

```
Librería SFX Telenovela:
├── sfx_telenovela_stinger_01.wav    -> Golpe de orquesta dramático (¡CHAN-CHAN-CHÁAAN!)
├── sfx_crack_pantalla_cel.wav        -> Ruptura seca de cristal templado contra piso
├── sfx_masticada_metal.wav          -> Crunch sordo de metal y plástico
├── sfx_resbalon_mango.wav           -> Whoosh cómico de caída slapstick
├── sfx_frenon_auto_derrape.wav      -> Rechinido prolongado de llantas en asfalto caliente
├── sfx_abolladura_cofre.wav         -> Thud metálico con vibración de lámina
├── sfx_rin_bicicleta_doblado.wav    -> Torsión metálica y caída en pasto
├── sfx_deglucion_gulp.wav           -> Sonido cómico de trago express
├── sfx_marcha_muerta_auto.wav       -> Click-click eléctrico descendente
├── sfx_chispas_tablero.wav          -> Zumbido eléctrico corto de cortocircuito
├── sfx_llaves_coladera_plash.wav    -> Tintineo metálico seguido de caída en agua
├── sfx_fuga_agua_presion.wav        -> Silbido de agua a presión saliendo de manguera
├── sfx_caja_registradora_crash.wav  -> Ka-ching clásico seguido de estruendo de platos
└── sfx_freeze_frame_telenovela.wav  -> Detención de cinta analógica + jingle WOOW
```

---

### 4. Flujo de Inserción de UI de la App WOOW (Motion Graphics)

Dado que las herramientas generativas de video por IA deforman interfaces de usuario y textos en pantalla, **todas las pantallas de la app WOOW se integran en postproducción**:

1. **Grabación de Video Base:** El actor / personaje sostiene un teléfono real o renderizado con pantalla verde o pantalla neutra mate apagada.
2. **Motion Tracking (2D / 4 Puntos):** En DaVinci Resolve (Fusion) o After Effects, rastrear las 4 esquinas de la pantalla del smartphone.
3. **Placas de UI Reales de WOOW:** Insertar las capturas oficiales limpias de la app en formato PNG 1080x2400 (con esquinas redondeadas):
   * *Cap. 1:* Módulo Protección Celular (botón "Solicitar Reparación").
   * *Cap. 2:* Módulo Seguro de Gadgets (botón "Reportar Daño").
   * *Cap. 3:* Módulo Accidentes Personales (pase médico directo).
   * *Cap. 4:* Módulo Seguro de Mascotas (Responsabilidad Civil / Placas).
   * *Cap. 5:* Módulo Seguro de Ciclistas (Reporte de asistencia en ruta).
   * *Cap. 6:* Wallet de Pólizas (Póliza de Mascotas / Gastos Veterinarios).
   * *Cap. 7:* Módulo Asistencia Vial (Botón amarillo "Paso de corriente + Grúa" con mapa GPS).
   * *Cap. 8:* Seguro de Auto (Adjuntar video de daños interiores).
   * *Cap. 9:* Asistencias de Hogar (Cerrajero y Plomero Express).
   * *Cap. 10:* Telemedicina 24/7 (Pantalla de videollamada con doctora).
   * *Cap. 11:* Pestaña "Mis Solicitudes" (Historial de folios resueltos en verde).
4. **Resplandor de Pantalla:** Aplicar un mapa de brillo sutil en el rostro del personaje (luz difusa turquesa/blanca) que coincida con el encendido de la pantalla.
