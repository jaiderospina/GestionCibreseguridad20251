# GestionCiberseguridad20251

## Ejercicio en Clase.

### **Ejercicio Dialéctico: Gestión de Riesgo Cibernético en "Banco Digital Seguro S.A."**  

**Contexto:**  
"Banco Digital Seguro S.A." es un banco con un fuerte enfoque en banca digital (70% de sus operaciones son en línea). Tiene USD 8,000 millones en activos y ha invertido USD 50 millones anuales en ciberseguridad. Sin embargo, en los últimos 6 meses ha enfrentado dos intentos de ransomware y un ataque de phishing exitoso que comprometió datos de 5,000 clientes.  

El Comité de Riesgo está reevaluando su postura de ciberseguridad ante el aumento de amenazas.  

1. **Balance y Regulaciones:**  
   - **Activos totales:** USD 8,000 millones.  
   - **Patrimonio:** USD 1,000 millones.  
   - **Fondo de contingencia cibernética:** USD 100 millones.  
   - **Liquidez regulatoria mínima (exigida por el Banco Central):** USD 50 millones *(no puede usarse para ciberseguridad)*.  
   - **Cobertura de seguro cibernético:** USD 30 millones por año (con deducible de USD 5 millones por incidente).  

2. **Costos de Incidentes:**  
   - **Ransomware:** USD 15-25 millones (dependiendo de la criticidad).  
   - **Brecha de datos:** USD 10-20 millones (multas + notificaciones a clientes).  
   - **Ataque DDoS prolongado:** USD 5-10 millones (pérdida operacional).  

3. **Probabilidades Anuales (Basadas en datos históricos + industria):**  
   - **Ransomware:** 20% de probabilidad.  
   - **Brecha de datos:** 15% de probabilidad.  
   - **DDoS crítico:** 10% de probabilidad.
  
---  

### **Preguntas Orientadoras (Dialéctica):**  

#### **1. Capacidad de Riesgo Cibernético (¿Cuánto riesgo PUEDE asumir?)**  
- **Cuantitativo:**  
  - El banco tiene un fondo de contingencia de USD 100 millones para incidentes cibernéticos. Si un ataque exitoso podría costar hasta USD 20 millones (respuesta, multas, reputación), ¿cuántos incidentes de este nivel podría absorber sin afectar su liquidez?  
  - Si el banco tiene un *coeficiente de resiliencia cibernética* del 85% (frente al 90% del sector), ¿qué brechas en su infraestructura limitan su capacidad?  

- **Cualitativo:**  
  - ¿Su estructura de gobierno (**CISO** directamente reportando a la junta) le permite responder rápidamente a amenazas?  

#### **2. Tolerancia al Riesgo Cibernético (¿Cuánto riesgo ESTÁ DISPUESTO a aceptar?)**  
- **Cuantitativo:**  
  - La junta ha establecido que no aceptará más de **1 incidente grave por año** (pérdidas > USD 10M). ¿Qué medidas reducirían la probabilidad actual (estimada en 30% anual) a menos del 10%?  
  - Si el banco tiene un *SLA de recuperación* de 4 horas para sistemas críticos, ¿es suficiente ante un ataque masivo de DDoS?  

- **Cualitativo:**  
  - ¿La cultura de "innovación rápida" (ej.: lanzar apps sin pruebas de penetración completas) aumenta su exposición?  

#### **3. Apetito de Riesgo Cibernético (¿Cuánto riesgo QUIERE tomar para crecer?)**  
- **Cuantitativo:**  
  - Si el banco quiere lanzar una **nueva plataforma de criptoactivos** (rentabilidad esperada: USD 30M/año; riesgo: incremento del 40% en ataques dirigidos), ¿el beneficio justifica el riesgo?  
  - ¿Cómo priorizar inversiones? (Ej.: ¿USD 20M en IA para detección de fraudes vs. USD 10M en capacitación de empleados?).  

- **Cualitativo:**  
  - ¿Está dispuesto a sacrificar experiencia de usuario (ej.: autenticación multifactor estricta) por mayor seguridad?  

---  

### **Bloque de Resolución y Justificación:**  

#### **1. Capacidad de Riesgo Cibernético**  
- **Cálculos clave:**  
  - **Fondo vs. Pérdidas Máximas:**  
    - USD 100M / USD 20M por incidente = **5 incidentes graves** antes de agotar reservas.  
    - Pero la regulación exige mantener al menos USD 50M en liquidez → capacidad real: **2-3 incidentes/año**.  
  - **Resiliencia:**  
    - El 85% implica que el 15% de sus sistemas son vulnerables (ej.: APIs obsoletas). Mitigar esto costaría USD 15M (según auditoría).  

#### **2. Tolerancia al Riesgo**  
- **Umbrales definidos:**  
  - **Probabilidad aceptable de incidente grave:** <10% anual (vs. 30% actual).  
    - Requeriría invertir USD 25M en:  
      - Migración a _cloud seguro_ (USD 10M).  
      - _Red team_ permanente (USD 5M/año).  
      - Seguro cibernético para cubrir USD 50M en pérdidas (USD 10M/año).  
  - **Cultural:**  
    - Implementar un "Security by Design" (ej.: pruebas de penetración obligatorias para nuevos productos).  

#### **3. Apetito de Riesgo**  
- **Análisis Costo-Beneficio:**  
  - **Plataforma de criptoactivos:**  
    - Beneficio neto: USD 30M - USD 10M (mayor seguridad) = **USD 20M**.  
    - Riesgo: Aumento del 40% en ataques → probabilidad de incidente grave subiría a 42% (inaceptable según tolerancia).  
    - **Solución:** Lanzarla con un piloto en un mercado pequeño (riesgo controlado).  
- **Inversiones prioritarias:**  
  - **IA para fraude** (ROI: 3:1) vs. **capacitación** (reduce phishing en 60%). Ambas son necesarias, pero la capacitación tiene mayor impacto a corto plazo.  

---  

### **Conclusión Didáctica:**  
Los estudiantes deben inferir que:  
- **Capacidad:** Moderada (fondos limitados y resiliencia subóptima).  
- **Tolerancia:** Baja (no acepta impacto operacional o reputacional grave).  
- **Apetito:** **Selectivo** (asume riesgos calculados en innovación, pero con controles estrictos).  

**Solución propuesta:**  
1. Rechazar el lanzamiento de criptoactivos hasta mejorar controles (aumentar resiliencia > 90%).  
2. Asignar USD 20M a capacitación y USD 10M a IA, priorizando mitigar el factor humano (origen del 70% de brechas).  
3. Adquirir seguro cibernético para transferir riesgo financiero.  

---  
**Nota:** Este ejercicio integra métricas duras (costos, probabilidades) con aspectos blandos (cultura, prioridades estratégicas), reflejando decisiones reales en ciberseguridad bancaria.


4. **Objetivos del Banco:**  
   - **Tolerancia al riesgo:** Máximo **1 incidente grave/año** (pérdida > USD 10M).  
   - **Apetito:** Incrementar un 20% la banca digital, aceptando un aumento del **10% en riesgo cibernético**.  


