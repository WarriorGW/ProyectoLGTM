# PayFlow MX

## Arquitectura

- **Microservicio**: Node.js + Express
- **Métricas**: LGTM
- **Logs**: Loki
- **Trazas**: OpenTelemetry
- **CI/CD**: GitHub Actions
- **Despliegue**: Blue/Green en Kubernetes

## Estructura del Proyecto

```
payflow-project/
├── microservice/       # Código del microservicio
├── pipeline/          # Configuración CI/CD
├── monitoring/        # Stack de observabilidad
├── docs/             # Documentación técnica
└── tests/            # Pruebas de carga (k6)
```

## Endpoints

- `GET /health` - Health check
- `GET /ready` - Readiness check
- `POST /api/v1/validate` - Validar transacción
- `GET /metrics` - Métricas Prometheus

## SLO/SLA

- **Disponibilidad**: 99.5% mensual
- **Latencia p95**: < 300ms
- **Tasa de error**: < 1%
