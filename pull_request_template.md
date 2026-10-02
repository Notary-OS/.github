## Qué cambia

<!-- El problema y su impacto, y después lo que hace este PR. Que se entienda sin leer otros PR. -->

## Verificación

<!-- Qué se corrió en local antes del push: tests, gates de seguridad, build, pruebas manuales. -->

## Seguridad

<!-- Obligatorio si el PR toca código o infraestructura (skill notaria-seguridad). Las casillas que no aplican se borran, no se marcan. -->

- [ ] Autorización: guard explícito; tenant y usuario del token; probado 401, 403 y otra notaría
- [ ] Entradas validadas en el servidor (body, query, path, archivos)
- [ ] Sin secretos ni datos personales en código, logs, URLs o respuestas
- [ ] Eventos de seguridad y rate limit si toca credenciales, sesión o cuentas
- [ ] Acceso a documentos o datos de clientes registrado en la auditoría
- [ ] Frontend: sin HTML sin sanear ni scripts inline; CSP sin aflojar
- [ ] Infra: todo por Terraform; IAM mínimo; checkov sin hallazgos nuevos o con skip justificado
- [ ] Gates locales corridos: tests, SAST, gitleaks
- [ ] `docs/iso27001` actualizado si cambia un control, un riesgo o un proveedor

## Pendientes

<!-- Lo que queda fuera, lo que hay que hacer después del merge y el ticket (Notary-OS/<repo>#N). -->
