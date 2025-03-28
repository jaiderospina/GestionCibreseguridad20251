### **Reducción de Probabilidad de Incidentes**  

#### **Objetivo:**  
Reducir la probabilidad de que ocurra **al menos un incidente grave** (ransomware, brecha de datos o DDoS) del **35% actual al 10% anual**, mediante inversiones en controles de ciberseguridad.  

---

## **1. Fórmulas Clave**  
### **A. Probabilidad de "Al Menos un Incidente"**  
Para calcular la probabilidad de que ocurra **uno o más incidentes** en un año, usamos el complemento de que **no ocurra ningún incidente**:  

\[
P(\geq 1 \text{ incidente}) = 1 - P(\text{ningún incidente})
\]  

Donde:  
- \( P(\text{ningún incidente}) \) es la probabilidad conjunta de que **todos los tipos de incidentes no ocurran**.  

### **B. Probabilidad Conjunta de Ningún Incidente**  
Si los incidentes son independientes, multiplicamos las probabilidades de que cada uno no ocurra:  

\[
P(\text{ningún incidente}) = P(\text{no ransomware}) \times P(\text{no brecha}) \times P(\text{no DDoS})
\]  

---

## **2. Aplicación al Caso del Banco**  
### **Datos Iniciales (Antes de Inversiones):**  
- **Probabilidades anuales individuales:**  
  - Ransomware: 20% → \( P_{\text{ransom}} = 0.20 \).  
  - Brecha de datos: 15% → \( P_{\text{brecha}} = 0.15 \).  
  - DDoS crítico: 10% → \( P_{\text{DDoS}} = 0.10 \).  

- **Probabilidad de ningún incidente:**  
\[
P(\text{ningún incidente}) = (1 - 0.20) \times (1 - 0.15) \times (1 - 0.10) = 0.80 \times 0.85 \times 0.90 = 0.612 \quad (61.2\%)
\]  

- **Probabilidad de al menos un incidente:**  
\[
P(\geq 1 \text{ incidente}) = 1 - 0.612 = 0.388 \quad (\text{38.8%})
\]  

*(Nota: En el enunciado original se decía 35%, pero con estos datos da 38.8%. Ajustaremos los valores para mantener coherencia).*  

---

### **Paso 1: Inversión en Controles**  
El banco implementa:  
1. **Migración a cloud seguro (USD 10M):**  
   - Reduce probabilidad de ransomware del 20% al 10% → \( P_{\text{ransom}} = 0.10 \).  
2. **Encriptación de datos (USD 5M):**  
   - Reduce brechas del 15% al 5% → \( P_{\text{brecha}} = 0.05 \).  
3. **DDoS se mantiene en 10%** (no se invierte aún en esto).  

**Nueva probabilidad de ningún incidente:**  
\[
P(\text{ningún incidente}) = (1 - 0.10) \times (1 - 0.05) \times (1 - 0.10) = 0.90 \times 0.95 \times 0.90 = 0.7695 \quad (76.95\%)
\]  

**Nueva probabilidad de al menos un incidente:**  
\[
P(\geq 1 \text{ incidente}) = 1 - 0.7695 = 0.2305 \quad (\text{23.05%})
\]  

**Resultado:**  
- La probabilidad bajó del **38.8% al 23.05%**, pero aún no se llega al **10% deseado**.  

---

### **Paso 2: Inversión Adicional (Monitoreo 24/7)**  
Para alcanzar el 10%, el banco invierte **USD 5M más** en:  
- **Monitoreo 24/7:** Reduce probabilidad de DDoS del 10% al 2% → \( P_{\text{DDoS}} = 0.02 \).  

**Cálculo final:**  
\[
P(\text{ningún incidente}) = 0.90 \times 0.95 \times (1 - 0.02) = 0.90 \times 0.95 \times 0.98 = 0.8379 \quad (83.79\%)
\]  

\[
P(\geq 1 \text{ incidente}) = 1 - 0.8379 = 0.1621 \quad (\text{16.21%})
\]  

**¡Todavía no se alcanza el 10%!**  

---

### **Paso 3: Ajuste de Controles (Fórmula General)**  
Para lograr \( P(\geq 1 \text{ incidente}) \leq 10\% \), se necesita:  
\[
P(\text{ningún incidente}) \geq 90\%.
\]  

**Despejando las probabilidades individuales:**  
\[
0.90 \times P_{\text{brecha}} \times P_{\text{DDoS}} \geq 0.90 \\
\Rightarrow P_{\text{brecha}} \times P_{\text{DDoS}} \geq 1.0 \quad \text{(Imposible, ya que cada probabilidad es } \leq 1\text{)}
\]  

**Conclusión:**  
- **No es posible** llegar al 10% solo con mitigar **brechas y DDoS**.  
- **Solución realista:**  
  - Reducir **ransomware a 5%** (inversión adicional en backups automáticos).  
  - Reducir **brechas a 3%** (doble encriptación).  
  - Reducir **DDoS a 1%** (proveedor especializado).  

**Nuevo cálculo:**  
\[
P(\text{ningún incidente}) = 0.95 \times 0.97 \times 0.99 = 0.912 \quad (91.2\%)
\]  
\[
P(\geq 1 \text{ incidente}) = 8.8\% \quad (\text{Meta cumplida})
\]  

---

## **3. Costo Total para Alcanzar el 10%**  
| **Control**               | **Costo (USD)** | **Reducción de Probabilidad**      |  
|---------------------------|-----------------|------------------------------------|  
| Migración a cloud seguro  | 10M             | Ransomware: 20% → 10%              |  
| Encriptación de datos     | 5M              | Brechas: 15% → 5%                  |  
| Monitoreo 24/7            | 5M              | DDoS: 10% → 2%                     |  
| Backups automáticos       | 7M              | Ransomware: 10% → 5%               |  
| Doble encriptación        | 3M              | Brechas: 5% → 3%                   |  
| Proveedor anti-DDoS       | 5M              | DDoS: 2% → 1%                      |  
| **Total**                 | **35M**         | **Probabilidad final: 8.8%**       |  

---

## **4. Fórmula General para Otros Casos**  
Para ajustar riesgos en cualquier empresa:  
1. **Identificar probabilidades individuales** de cada incidente.  
2. **Calcular** \( P(\text{ningún incidente}) = \prod (1 - P_{\text{incidente}}) \).  
3. **Definir meta** (ej.: \( P(\geq 1 \text{ incidente}) \leq 10\% \)).  
4. **Invertir en controles** hasta que:  
   \[
   \prod (1 - P_{\text{incidente}}) \geq 0.90
   \]  

**Ejemplo simplificado:**  
- Si hay 3 tipos de incidentes con \( P = 5\% \) cada uno:  
  \[
  P(\geq 1) = 1 - (0.95 \times 0.95 \times 0.95) = 14.3\%.
  \]  
- Para llegar al 10%, se necesita reducir al menos un riesgo al **2%**.  

---

**Conclusión:**  
Este método permite cuantificar el impacto de cada inversión en seguridad y priorizar recursos para cumplir con la tolerancia al riesgo definida.