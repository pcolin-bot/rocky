# 📸 05. Hoja Maestra de Prompts de Video e Imagen

## Guía de Consistencia Visual y Generación por Inteligencia Artificial
* **Estilo:** Hiperrealista Cinematográfico (*Hyperrealistic Cinematic Commercial*).
* **Relación de Aspecto:** 9:16 Vertical (1080x1920).
* **Parámetros de Cámara:** Lentes 35mm y 50mm, f/1.8, bokeh suave, textura de piel y pelaje realista, iluminación natural matutina en CDMX.

---

### 1. Bloque de Consistencia de Personajes (Character Prompt Locks)

> [!IMPORTANT]
> Para garantizar que el dálmata, Alex y Sam no cambien de apariencia física entre capítulos, se debe incluir su respectivo bloque de texto maestro en cada prompt de generación.

#### 🐶 Rogelio (El Dálmata — Hero Asset)
```text
[ROGELIO_PROMPT_LOCK]: A photorealistic young male Dalmatian dog, 2 years old, pure white short sleek coat with distinct crisp black spots evenly distributed, expressive floppy spotted ears, soulful amber-brown eyes, lean athletic build, wearing a fitted sky-blue fabric chest harness with a matte black buckle, extremely expressive innocent and slightly guilty puppy facial expressions, cinematic natural lighting, highly detailed fur texture, 8k resolution, photorealistic.
```

#### 👩 Alex (Mujer, 28 años — Dueña de Rogelio)
```text
[ALEX_PROMPT_LOCK]: A 28-year-old Mexican woman, contemporary urban CDMX lifestyle, natural wavy dark brown hair tied in a loose stylish morning bun, warm olive skin tone, expressive big dark eyes, slender build. In home scenes wearing cozy light-grey ribbed pajama pants and an off-white cotton tank top; in street scenes wearing black joggers, white sneakers, and an olive green zip-up hoodie. Very expressive, dramatic, comedic facial reactions, hyperrealistic skin pores and natural daylight, shot on 35mm lens, f/1.8.
```

#### 👨 Sam (Hombre, 38 años — El Roomie)
```text
[SAM_PROMPT_LOCK]: A 38-year-old Mexican man, handsome mature features, neatly trimmed short dark hair with subtle salt-and-pepper dusting at the temples, neat short designer stubble beard, calm amused eyes, athletic-lean build. Wearing a dark navy-blue crewneck cotton t-shirt and charcoal lounge sweatpants, holding a ceramic coffee mug, relaxed, ironic, pragmatic posture, photorealistic, natural ambient morning lighting.
```

#### 🏡 Locación Principal (Departamento en CDMX)
```text
[APARTMENT_PROMPT_LOCK]: Modern bright apartment in Mexico City Roma-Condesa, Scandinavian-Mexican minimalist interior design, light natural oak hardwood floors, large floor-to-ceiling windows with sheer white linen curtains diffusing soft warm morning sunlight, potted indoor monstera and ficus plants, low wooden bed frame with messy beige linen sheets, cozy warm atmosphere, cinematic depth of field.
```

---

### 2. Negative Prompts Maestros (Para todos los motores)
```text
[UNIVERSAL_NEGATIVE_PROMPT]: cartoon, 3d render, anime, CGI illustration, deformed paws, extra legs, mutated dog anatomy, dog with patches instead of spots, pitbull, golden retriever, two dogs, extra fingers, disfigured hands holding phone, distorted smartphone screen, unreadable alien text, harsh artificial flash lighting, oversaturated neon colors, blurred face, double faces, plastic skin, uncanny valley.
```

---

### 3. Prompts de Generación de Video Escena por Escena (Inglés Técnico)

#### 📱 Capítulo 01: El cel nuevo
* **Toma 1 (00:00 - 00:04) — Macro mordisco:**
  ```text
  Macro close-up shot: Under a wooden bed, [ROGELIO_PROMPT_LOCK] lying on light hardwood floor happily chewing on a white braided smartphone charger cable. Camera slowly pushes in. Shallow depth of field, dust motes in soft morning light beam. High frame rate, 4k hyperrealistic. --ar 9:16
  ```
* **Toma 2 (00:04 - 00:09) — La caída:**
  ```text
  Medium shot: In a sunlit bedroom [APARTMENT_PROMPT_LOCK], [ALEX_PROMPT_LOCK] reaches her sleepy hand down from the bed, accidentally yanks the white charging cable. The smartphone slips from the wooden nightstand and smashes face down onto the hard floor with a visible screen crack impact. Cinematic motion blur. --ar 9:16
  ```
* **Toma 3 (00:09 - 00:14) — El drama y la foto:**
  ```text
  Medium-close shot: Alex sits up on the edge of the bed looking in pure despair at the shattered smartphone glass. [SAM_PROMPT_LOCK] enters the doorway holding a coffee mug, whips out his own smartphone with a calm smile and snaps a clear photo of the cracked screen. [ROGELIO_PROMPT_LOCK] lies innocently beside the bed. --ar 9:16
  ```
* **Toma 4 (00:14 - 00:19) — El Cliffhanger de la laptop:**
  ```text
  Low angle medium shot: [ROGELIO_PROMPT_LOCK] lets go of the cable, perks his ears up, turns his head slowly and stares with intense playful curiosity at an open metallic laptop sitting on the low desk in the corner. Dramatic telenovela push-in zoom into the dog's eyes. Suspenseful lighting. --ar 9:16
  ```

---

#### 💻 Capítulo 02: Sabotaje laboral
* **Toma 1 (00:00 - 00:05) — Flashback masticada:**
  ```text
  Sepia warm memory flashback: Slow motion close-up of [ROGELIO_PROMPT_LOCK] vigorously gnawing on the aluminum corner of a modern laptop on an office desk, tooth marks biting into metal, tail wagging innocently. Dreamy cinematic vignette. --ar 9:16
  ```
* **Toma 2 (00:05 - 00:12) — Desesperación de Alex:**
  ```text
  Medium shot: [ALEX_PROMPT_LOCK] holding the chewed laptop with crushed corner, desperately pressing the power button with wide panicked eyes. [SAM_PROMPT_LOCK] stands beside her, tapping quickly on his modern smartphone screen, registering the incident calmly. --ar 9:16
  ```
* **Toma 3 (00:12 - 00:19) — La puerta de la cocina:**
  ```text
  Medium shot: Sam walks towards the kitchen door, pushes it open, freezes completely in place with jaw dropped and wide eyes. Sam slowly turns his head back towards Alex with a grim expression. Slow push-in on Sam's frozen face. --ar 9:16
  ```

---

#### 🥭 Capítulo 03: Caída libre
* **Toma 1 (00:00 - 00:06) — El resbalón:**
  ```text
  High-angle top-down shot: Kitchen floor covered in organic trash and yellow mango peels. [ALEX_PROMPT_LOCK] dashes in, steps directly on a slippery mango peel, both feet fly up into the air in a comical slapstick stunt, landing flat on her back on the clean tile. --ar 9:16
  ```
* **Toma 2 (00:06 - 00:13) — Tobillo y la app:**
  ```text
  Close-up medium shot: Alex grimacing on the floor holding her swollen ankle. [SAM_PROMPT_LOCK] kneels beside her showing his glowing smartphone screen while placing an ice pack wrapped in a kitchen towel on her foot. --ar 9:16
  ```
* **Toma 3 (00:13 - 00:19) — El escape:**
  ```text
  Dynamic low angle: The apartment front door is slightly ajar. [ROGELIO_PROMPT_LOCK] pushes the wooden door wide open with his wet nose and sprints like a bullet down the hallway towards the exit stairs. Alex yells pointing in panic. --ar 9:16
  ```

---

#### 🚗 Capítulo 04: La fuga
* **Toma 1 (00:00 - 00:07) — El brinco al cofre:**
  ```text
  Wide tracking shot on a sunny Mexico City residential street: [ROGELIO_PROMPT_LOCK] dashes across asphalt. A sleek grey sedan screeches to an emergency halt with smoke from tires. The Dalmatian leaps playfully onto the car's hood, leaving a noticeable dent in the metal sheet before hopping off. --ar 9:16
  ```
* **Toma 2 (00:07 - 00:14) — El vecino furioso y WOOW:**
  ```text
  Medium shot: An angry middle-aged Mexican driver steps out pointing furiously at the hood dent. [ALEX_PROMPT_LOCK] limping quickly to the scene, holding up her smartphone with a friendly reassuring smile, pointing to the active digital policy screen. --ar 9:16
  ```
* **Toma 3 (00:14 - 00:19) — Carrera al parque:**
  ```text
  Tracking camera: Rogelio sees an open green gate of an urban park and bolts at full speed through the grass towards a busy paved bike lane. High energy cinematic motion. --ar 9:16
  ```

---

#### 🚲 Capítulo 05: Frenón en bici
* **Toma 1 (00:00 - 00:06) — La caída en la ciclovía:**
  ```text
  Fast tracking shot: A stylish cyclist on a road bike suddenly swerves to avoid [ROGELIO_PROMPT_LOCK] who paused in the middle of the bike lane. The cyclist tumbles safely onto the soft green lawn, while the front wheel of the bicycle hits a curb and buckles into a warped figure-eight. --ar 9:16
  ```
* **Toma 2 (00:06 - 00:13) — Solidaridad digital:**
  ```text
  Medium shot: The cyclist sits on the grass dusting off his helmet, smiles and pulls his own smartphone out showing the WOOW app interface to Alex. [ROGELIO_PROMPT_LOCK] sits next to them panting happily with his head tilted. --ar 9:16
  ```
* **Toma 3 (00:13 - 00:19) — El chocolate:**
  ```text
  Extreme close-up: Rogelio's snout sniffing a dark rectangular chocolate bar wrapped in shiny foil dropped on the grass. In one swift gulp, his jaws open and swallow the entire bar. Extreme push-in zoom with high dramatic tension. --ar 9:16
  ```

---

#### 🏥 Capítulo 06: Urgencias
* **Toma 1 (00:00 - 00:07) — La clínica veterinaria:**
  ```text
  Interior modern veterinary clinic: [ROGELIO_PROMPT_LOCK] lying on a stainless steel examination table with a rounded bloated tummy and very sad droopy eyes. A Mexican veterinarian in green scrubs checks him with a stethoscope and speaks to [ALEX_PROMPT_LOCK]. --ar 9:16
  ```
* **Toma 2 (00:07 - 00:14) — El pago sin drama:**
  ```text
  Medium shot: Alex at the reception desk confidently tapping her smartphone on the payment counter, displaying the active pet health insurance coverage in WOOW. The receptionist smiles and stamps the medical release form. --ar 9:16
  ```
* **Toma 3 (00:14 - 00:19) — Marcha muerta:**
  ```text
  Night exterior: Dimly lit parking lot. Alex sits in the driver seat of her car, turning the ignition key. Dead battery clicks. In the passenger seat, Rogelio sits wearing a huge transparent plastic Elizabethan cone of shame, staring blankly ahead. --ar 9:16
  ```

---

#### 🛞 Capítulo 07: Varados de noche
* **Toma 1 (00:00 - 00:06) — Doble tragedia:**
  ```text
  Wide night shot: A parked hatchback under a flickering street lamp. Alex stands outside shivering in her hoodie, looking down at a completely flat rear tire on the rim. [ROGELIO_PROMPT_LOCK] inside with his cone peering through the foggy window. --ar 9:16
  ```
* **Toma 2 (00:06 - 00:13) — Auxilio vial en camino:**
  ```text
  Medium-close shot: Alex smiles with relief as her smartphone screen illuminates her face, showing the real-time GPS tracking icon of an incoming roadside assistance truck. Yellow flashing safety lights reflect in her eyes. --ar 9:16
  ```
* **Toma 3 (00:13 - 00:19) — El salto al portavasos:**
  ```text
  Interior car shot: Bright yellow flashing lights shine into the car. Rogelio with his wide cone gets startled and leaps awkwardly towards the front center console right next to a full tall cardboard cup of hot steaming coffee. High tension camera freeze. --ar 9:16
  ```

---

#### ☕ Capítulo 08: Café en el tablero
* **Toma 1 (00:00 - 00:06) — La inundación de café:**
  ```text
  Slow motion close-up: The rim of the dog's cone knocks against the cardboard coffee cup. Dark hot coffee splashes generously over the automatic gear shift, digital climate controls, and buttons. Tiny sparks and flickering dashboard lights. --ar 9:16
  ```
* **Toma 2 (00:06 - 00:13) — Resignación de Alex:**
  ```text
  Medium shot: [ALEX_PROMPT_LOCK] gripping the steering wheel, taking a deep meditative breath with closed eyes, smiling ironically. She holds up her smartphone recording a 3-second diagnostic video clip of the blinking dashboard for the WOOW app. --ar 9:16
  ```
* **Toma 3 (00:13 - 00:19) — Bolsillos vacíos:**
  ```text
  Midnight shot outside the apartment door: Alex urgently searching through all the pockets of her hoodie and jeans. Eyes widening in sudden horror as she realizes her keys are missing. Deep shadow lighting. --ar 9:16
  ```

---

#### 🔑 Capítulo 09: Coladera y fuga de agua
* **Toma 1 (00:00 - 00:05) — Flashback coladera:**
  ```text
  High-contrast black-and-white comic flashback: When Alex jumped earlier in the park, a metal keychain with shiny keys flies out of her pocket in slow motion and drops cleanly between the metal iron bars of a street sewer drain with a metallic splash. --ar 9:16
  ```
* **Toma 2 (00:05 - 00:12) — Inundación sonora:**
  ```text
  Medium shot: Alex with ear pressed against the wooden apartment door, hearing intense loud water gushing inside. [SAM_PROMPT_LOCK] appears at the top of the stairs, smartphone in hand, tapping the home assistance button with urgency. --ar 9:16
  ```
* **Toma 3 (00:12 - 00:19) — Rescate del hogar:**
  ```text
  Medium wide shot: Inside the apartment, a professional locksmith with tools opens the door lock while a plumber in uniform turns off the master valve and fixes a leaking silver pipe under the sink. Alex collapses onto the living room sofa, completely exhausted and pale. --ar 9:16
  ```

---

#### 🩺 Capítulo 10: La consulta digital
* **Toma 1 (00:00 - 00:06) — El colapso en el sillón:**
  ```text
  Medium close-up: [ALEX_PROMPT_LOCK] wrapped in thick wool blankets on the grey living room sofa, a damp white compress on her forehead, foot tightly bandaged resting on decorative cushions. [SAM_PROMPT_LOCK] brings her a steaming mug of tea and hands her a smartphone on a call. --ar 9:16
  ```
* **Toma 2 (00:06 - 00:13) — La videoconsulta:**
  ```text
  Over-the-shoulder shot: Alex talking to a friendly Mexican female doctor in a white medical coat via high-definition video call on her smartphone screen. A digital medical prescription PDF notification pops up on the screen. --ar 9:16
  ```
* **Toma 3 (00:13 - 00:19) — La libreta de cuentas:**
  ```text
  Close-up shot: Alex opening a spiral notebook with a pen, beginning to jot down large financial numbers with a furrowed comedic brow of panic. Dramatic musical push-in. --ar 9:16
  ```

---

#### 🧾 Capítulo 11: La suma final
* **Toma 1 (00:00 - 00:06) — Desglose de gastos:**
  ```text
  Macro top-down shot of handwritten notebook page showing itemized expenses in Mexican Pesos with red underlines totaling $47,500 MXN. Clear legible handwriting, cinematic tabletop lighting. --ar 9:16
  ```
* **Toma 2 (00:06 - 00:13) — El milagro de los $0:**
  ```text
  Medium shot: [ALEX_PROMPT_LOCK] excitedly flips the page to reveal a giant bold green handwritten number: 'TOTAL PAGADO: $0 MXN'. [SAM_PROMPT_LOCK] nods proudly holding up the WOOW app claim history screen showing green checkmarks. --ar 9:16
  ```
* **Toma 3 (00:13 - 00:19) — El vaso en la orilla:**
  ```text
  Low angle suspense shot: [ROGELIO_PROMPT_LOCK] tiptoeing slowly toward the glass coffee table where a full glass of ice water sits right on the edge. The dog's tail swishes dangerously close to the glass. Extreme tension frame. --ar 9:16
  ```

---

#### 🏆 Capítulo 12: El gran cierre (Final de Telenovela)
* **Toma 1 (00:00 - 00:06) — Paz efímera:**
  ```text
  Medium wide shot: [ALEX_PROMPT_LOCK] and [SAM_PROMPT_LOCK] resting peacefully under blankets on the cozy sofa drinking tea. [ROGELIO_PROMPT_LOCK] lies contentedly at their feet with innocent puppy eyes. Warm golden evening living room lighting. --ar 9:16
  ```
* **Toma 2 (00:06 - 00:11) — El vaso volador:**
  ```text
  Slow motion comic disaster: Rogelio gets up to stretch, wags his energetic spotted tail, and his front paw accidentally nudges the tall glass of water. Water cascades through the air toward the electronics on the rug. --ar 9:16
  ```
* **Toma 3 (00:11 - 00:14) — FREEZE FRAME CÓMICO:**
  ```text
  Freeze frame mid-air: Action instantly frozen. Alex and Sam with mouths wide open screaming in comedic horror, hands clutching their hair, while Rogelio looks directly into the camera lens with a happy goofy grin. High-fashion telenovela final freeze. --ar 9:16
  ```
* **Toma 4 (00:14 - 00:19) — Cortinilla y Logo WOOW:**
  ```text
  Clean motion graphic outro: Elegant golden Mexican telenovela title card 'FIN... ¿O CONTINUARÁ?'. Smooth transition into official WOOW logo animation with turquoise and yellow branding against clean white background. --ar 9:16
  ```
