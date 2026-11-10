# Parking Smart V3

Prototipo de la app **Parking Smart V3**, proyecto estudiantil para la Feria de Bachillerato Técnico.

Propuesta para el parqueadero de la Hostería La Puesta del Sol (Catamayo, Ecuador), donde los fines de semana y feriados hay gran afluencia vehicular.

## Capacidad

| Área | Plazas |
|------|--------|
| Parqueadero general al aire libre (Zona A y Zona B) | 50 |
| Parking VIP bajo sombra, edificio de 2 niveles (15 por nivel) | 30 |
| **Total monitoreado** | **80** |

## Qué muestra la simulación

- **Inicio:** cupos libres en vivo y porcentaje de ocupación, por zona.
- **Plano:** vista de cada zona con luz verde (libre), roja (ocupada) o ámbar (reservada).
- **Reserva:** apartar una plaza por 15 minutos con cuenta regresiva.
- **Alertas:** aviso cuando se libera un cupo.
- **Panel de demo:** modo feriado / día normal, simular la llegada o salida de autos.

Los datos son simulados. En la versión real vendrían de los sensores.

## Cómo funciona el sistema

1. **Sensor** ultrasónico HC-SR04 sobre cada plaza.
2. **ESP32** decide libre/ocupado, enciende la luz y envía el dato por Wi-Fi.
3. **Nube**: base de datos en tiempo real (p. ej. Firebase).
4. **App y pantalla** en la entrada se actualizan solas.

## Versiones

- **V1:** contador de vehículos que entran y salen.
- **V2:** sensor y luz por plaza, pantalla de cupos en la entrada.
- **V3:** app móvil con plano en vivo, reservas y alertas (este prototipo).

## Ver la simulación

- Abrir `index.html` con doble clic en cualquier navegador (funciona sin internet).
- En línea con GitHub Pages: *Settings → Pages → Branch: `main` / root → Save*.
