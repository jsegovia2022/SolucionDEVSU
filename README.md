# SolucionDEVSU
# Sistema de Banca por Internet - Entidad BP
## Documento de Diseño de Arquitectura de Solución (Modelo C4)

### 1. Resumen del Proyecto
Diseño técnico de la plataforma omnicanal de banca por internet para la entidad financiera BP, cubriendo consultas de movimientos, transferencias (propias e interbancarias vía SPI) y pagos de servicios.

### 2. Atributos de Calidad Principales
- **Disponibilidad:** 99.9% mensual bajo topología Multi-AZ y DR pasivo en AWS.
- **Seguridad:** Paradigma Zero Trust, OAuth 2.0 con Authorization Code + PKCE, cifrado AES-256 / TLS 1.3.
- **Rendimiento:** Latencia p95 < 800 ms mediante estrategias de Cache-Aside (Redis) y read-models.
- **Auditoría e Inmutabilidad:** Pistas transaccionales mediante Transactional Outbox y retención WORM de 10 años acorde a la normativa financiera local.

### 3. Contenido en Desarrollo
- [x] Alcance y levantamiento de requerimientos
- [ ] Registros de Decisión Arquitectónica (ADRs)
- [ ] Modelado C4 (Contexto, Contenedores y Componentes)
- [ ] Diagramas de Secuencia e Infraestructura Cloud AWS
- [ ] Documento PDF consolidado de entrega
