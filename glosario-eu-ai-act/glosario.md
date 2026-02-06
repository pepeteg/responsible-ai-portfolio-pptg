# Glosario de Ética y Gobernanza en IA  
## (Basado en el EU AI Act y conceptos clave de Responsible AI)

**Última actualización:** Febrero 2026  
**Autor:** Pablo Tirado  
**Repositorio:** https://github.com/tu-usuario/responsible-ai-portfolio  
**Portafolio completo en Notion:** https://daily-fish-b51.notion.site/Portafolio-Responsible-AI-Pablo-Tirado-2e2d9934f4878046aa4ecf94a58071f6

Este glosario recoge los términos más importantes que he estudiado y aplicado en mi serie de proyectos Responsible AI. Incluye definiciones claras, referencias al EU AI Act y ejemplos prácticos de mis partes 1-5.

### 1. Conceptos básicos

- **Responsible AI (IA Responsable)**  
  Conjunto de principios y prácticas para desarrollar y desplegar IA de forma ética, segura, transparente y respetuosa con los derechos humanos. Incluye fairness, explainability, privacy, robustness y accountability.

- **EU AI Act**  
  Reglamento europeo sobre inteligencia artificial (Reglamento (UE) 2024/1689). Clasifica sistemas de IA por riesgo y establece obligaciones como transparencia, evaluación de riesgos y mitigación de bias.

### 2. Bias y Fairness

- **Bias (Sesgo)**  
  Tendencia sistemática en un modelo que favorece o perjudica a ciertos grupos (por género, raza, edad, etc.). Puede venir de datos, etiquetas o algoritmo.

- **Fairness (Equidad)**  
  Propiedad de un modelo que trata a grupos de forma justa. No hay una definición única – depende del contexto (ej. equal opportunity, demographic parity).

- **Disparate Impact**  
  Métrica de fairness. Tasa de positivos en grupo no privilegiado / tasa en privilegiado. Ideal ≈1.0. Umbral aceptable: >0.8 (regla de los 80%).

- **Equal Opportunity**  
  Todos los grupos tienen la misma tasa de verdaderos positivos (TPR).

- **Demographic Parity**  
  La predicción positiva es independiente del atributo sensible (misma tasa de positivos en todos los grupos).

### 3. Explicabilidad (Explainability)

- **Explainable AI (XAI)**  
  Técnicas para que las decisiones de un modelo sean comprensibles para humanos.

- **SHAP (SHapley Additive exPlanations)**  
  Método basado en teoría de juegos para asignar importancia a cada feature en predicciones individuales y globales.

- **LIME (Local Interpretable Model-agnostic Explanations)**  
  Explica predicciones individuales aproximando el modelo localmente con uno interpretable (lineal).

- **Integrated Gradients**  
  Método de atribución para ver qué partes del input (tokens en LLMs) influyen más en la salida.

### 4. Mitigación de Bias

- **Pre-processing**  
  Corregir datos antes de entrenar (ej. Reweighing en AIF360 – dar más peso a muestras subrepresentadas).

- **In-processing**  
  Modificar el algoritmo durante entrenamiento (ej. MinDiff, adversarial debiasing).

- **Post-processing**  
  Ajustar predicciones después de entrenar (ej. threshold adjustment por grupo para mejorar disparate impact).

### 5. Clasificación de riesgo (EU AI Act)

- **Prohibidos**  
  IA que manipula comportamiento, scoring social, reconocimiento facial en tiempo real en espacios públicos.

- **Alto riesgo**  
  Sistemas en educación, empleo, crédito, justicia, salud. Obligaciones: evaluación de riesgos, transparencia, datos de calidad, auditorías.

- **Riesgo limitado**  
  Chatbots, deepfakes → transparencia obligatoria (decir que es IA).

- **Riesgo mínimo**  
  IA sin impacto significativo → sin obligaciones.

### 6. Otros términos clave

- **Model Cards**  
  Documento que describe uso previsto, limitaciones, métricas de rendimiento y fairness de un modelo.

- **Data Cards**  
  Similar, pero para datasets (fuente, sesgos conocidos, representatividad).

- **Hallucinations**  
  En LLMs, generar información falsa con confianza.

- **Adversarial Robustness**  
  Capacidad de resistir ataques que intentan engañar el modelo.

### Recursos recomendados

- EU AI Act (texto oficial): https://eur-lex.europa.eu/legal-content/ES/TXT/?uri=CELEX:32024R1689  
- Google Responsible AI Practices  
- Microsoft Responsible AI Standard  
- AIF360, SHAP, LIME (librerías open source)

Este glosario se actualiza con cada proyecto nuevo. ¡Feedback bienvenido! 🤖⚖️
