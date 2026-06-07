# 🌾 AgroSensor — Sistema de Monitoreo Preventivo de Incendios Rurales

> 🥇 **Proyecto ganador del Primer Puesto en HackActiva 2026** — Agroactiva, Armstrong (Santa Fe).

🔗 **[Ver demo en vivo](https://matias42-dev.github.io/AgroSensor/)**

AgroSensor es un sistema de monitoreo ambiental en tiempo real diseñado para **anticiparse a los incendios rurales** antes de que ocurran. Combina sensores de campo, un índice de riesgo automático y alertas inmediatas al productor, con activación de un sistema de riego preventivo.

---

## 🔥 El problema

Durante las épocas de calor extremo, la combinación de altas temperaturas, baja humedad, fuerte radiación solar y viento genera condiciones propicias para incendios que arrasan grandes extensiones de campo en muy poco tiempo. El problema muchas veces no es solo el incendio, sino **detectarlo cuando ya es demasiado tarde**.

Provincias como Córdoba, La Pampa y Mendoza sufren cada año pérdidas económicas y ambientales enormes por esta razón.

---

## 💡 La solución

AgroSensor es un sistema de monitoreo preventivo basado en un **dron autónomo equipado con sensores ambientales**. El dron realiza recorridos programados sobre los campos y recopila información en tiempo real sobre cuatro variables ambientales clave, con las que se calcula un **índice de riesgo de incendio**:

- 💧 **Humedad del suelo**
- 🌡️ **Temperatura**
- 💨 **Velocidad del viento**
- ☀️ **Radiación solar**

Todos los datos se envían automáticamente a una aplicación móvil donde se procesan y visualizan. Cuando el sistema detecta condiciones críticas:

1. Envía **alertas inmediatas** al productor (app, WhatsApp, Telegram o email).
2. Puede **activar automáticamente un sistema de riego** para aumentar la humedad de la zona y reducir la probabilidad de incendio.

---

## 🖥️ Características del dashboard

- **Monitoreo en vivo** de los 4 sensores con indicadores de estado (óptimo / aviso / crítico).
- **Gráficos históricos** de las últimas 24 horas por variable.
- **Índice de riesgo de incendio** calculado dinámicamente combinando todos los factores.
- **Sistema de riego** con control manual y métricas de uso (tiempo, agua, cobertura).
- **Centro de alertas** con registro de eventos y notificaciones simuladas por WhatsApp/Email.
- **Diseño responsive** — funciona en escritorio, tablet y celular.

---

## 🛠️ Tecnologías utilizadas

- **HTML5**
- **CSS3** (diseño responsive, grid layout, animaciones)
- **JavaScript** (vanilla, sin frameworks)
- **Chart.js** — visualización de datos en tiempo real

---

## 🚀 Cómo ejecutarlo

No requiere instalación ni servidor. Simplemente:

```bash
# Cloná el repositorio
git clone https://github.com/matias42-dev/AgroSensor.git

# Abrí el archivo en tu navegador
cd AgroSensor
# Doble clic en index.html o abrilo desde el navegador
```

> 💡 **Probalo online sin instalar nada:** [https://matias42-dev.github.io/AgroSensor/](https://matias42-dev.github.io/AgroSensor/)
>
> También funciona directamente en el celular: abrí el archivo HTML con cualquier navegador móvil.

---

## 📊 Cómo funciona el índice de riesgo

El índice (0–100%) se calcula ponderando las cuatro variables:

| Variable | Peso | Lógica |
|----------|------|--------|
| Humedad del suelo | 35% | A menor humedad, mayor riesgo |
| Temperatura | 30% | A mayor temperatura, mayor riesgo |
| Viento | 20% | A mayor velocidad, mayor riesgo |
| Radiación solar | 15% | A mayor radiación, mayor riesgo |

Cuando el índice supera el 65%, se dispara una alerta automática.

---

## 🔮 Próximos pasos

- [ ] Integración con el dron autónomo y sensores IoT reales (sensores de temperatura, humedad, anemómetro y piranómetro embarcados).
- [ ] Planificación de rutas de vuelo automáticas sobre los lotes a monitorear.
- [ ] Backend para almacenar datos históricos y entrenar un modelo predictivo de riesgo.
- [ ] App móvil nativa con notificaciones push.
- [ ] Integración real con APIs de WhatsApp Business y Telegram.
- [ ] Validación con productores agropecuarios reales.

---

## 🏆 Reconocimiento

Proyecto desarrollado en el marco de **HackActiva 2026**, organizado por el **Gobierno de Venado Tuerto**, **NETI (No Está Todo Inventado)** y **Agroactiva**, en una jornada de hackathon con metodología Design Thinking.

🥇 **Primer Puesto**

---

## 👤 Autor

**Matías Nicolás Ailan Lorenzetti**
Estudiante de Técnico Superior en Desarrollo de Software — ICES Venado Tuerto

- LinkedIn: [Matías Ailan](https://www.linkedin.com/in/matías-ailan-9bab21352/)
- GitHub: [matias42-dev](https://github.com/matias42-dev)

---

## 📄 Licencia

Este proyecto está bajo la licencia MIT — ver el archivo [LICENSE](LICENSE) para más detalles.
