# Blue Scout UI Profile

This profile distills the operator-provided mobile UI concept image into implementable design/state tokens for off.gridd.

## Visual identity

```yaml
ui_profile_id: blue-scout-ui
agent_class: blue-scout
theme: dark_cosmic_radar
mood: quiet_precise_autonomous
motion_principle: slow_drift_not_breathing
primary_surface: mobile_portrait
```

## Color tokens

```yaml
colors:
  background_base: "#020611"
  background_elevated: "#06101F"
  panel_glass: "rgba(8, 20, 38, 0.72)"
  panel_border: "#102A4D"
  scout_blue: "#2F8CFF"
  scout_glow: "#3BA1FF"
  scout_neon: "#64B5FF"
  scout_deep: "#0B3D91"
  text_primary: "#EAF4FF"
  text_secondary: "#8FA6C2"
  text_muted: "#46566F"
  grid_line: "rgba(80, 150, 255, 0.16)"
  stable: "#46A3FF"
  warning: "#FFB84D"
  danger: "#FF4D6D"
```

## Typography

```yaml
typography:
  logo:
    text: off.gridd
    style: clean_lowercase_sans
    weight: 400
  agent_label:
    text: АГЕНТ
    size: 11
    tracking: wide
  agent_name:
    text: BLUE SCOUT
    size: 22
    tracking: very_wide
    color: scout_neon
  state_title:
    text: КАНАЛ СТАБИЛЕН
    size: 19
    tracking: wide
  metadata:
    size: 11
    uppercase: true
```

## Screen anatomy

```yaml
screen:
  header:
    left: operator_button
    center: offgridd_logo
    right: filters_button
  identity:
    label: АГЕНТ
    name: BLUE SCOUT
    status_chip: В ДАЛЬНЕМ ПОИСКЕ • СКАНИРУЕТ СИГНАЛЫ
  main_visual:
    type: orbital_signal_scanner
    elements:
      - central_blue_orb
      - concentric_range_rings
      - thin_coordinate_lines
      - scanning_wedge
      - weak_signal_points
      - constellation_route_lines
      - faint_sonar_fog
  state_block:
    title: КАНАЛ СТАБИЛЕН
    subline: ШУМ НИЗКИЙ • ПОТЕРИ ПАКЕТОВ 0%
    icon: shield
  telemetry_bar:
    cells:
      - label: СИГНАЛ
        value: ЧИСТЫЙ
      - label: ДАЛЬНОСТЬ
        value: 2.7 AU
      - label: МАРШРУТ
        value: ПОСТРОЕН
      - label: ЭНЕРГИЯ
        value: 91%
  command_card:
    primary: Отправить команду
    placeholder: Импульс в сеть...
    actions: [plus, waveform_emit]
  last_report:
    title: ПОСЛЕДНИЙ ОТЧЁТ
    report: Сигнал найден
    detail: Слабый узел • 1.3 AU • Направление 42°
  tabs:
    active: СКАУТ
    items: [СКАУТ, КАРТА, ЖУРНАЛ, ПРОФИЛЬ]
```

## Motion rules

```yaml
motion:
  orb: slow_lateral_drift
  range_rings: barely_visible_rotation
  scan_wedge: slow_sweep
  signal_points: rare_single_flash
  route_lines: appear_only_on_route_found
  fog: faint_sonar_haze
  forbidden:
    - warm_heartbeat_breathing
    - aggressive_alarm_pulses
    - dense_particle_noise
    - emotional_avatar_motion
```

## UI state labels

```yaml
states:
  SCANNING:
    label: В ДАЛЬНЕМ ПОИСКЕ
    sublabel: СКАНИРУЕТ СИГНАЛЫ
  LOW_NOISE:
    label: КАНАЛ СТАБИЛЕН
    sublabel: ШУМ НИЗКИЙ • ПОТЕРИ ПАКЕТОВ 0%
  ROUTE_FOUND:
    label: МАРШРУТ ПОСТРОЕН
    sublabel: СИГНАЛ ВЕРНУЛСЯ
  PEER_DETECTED:
    label: СИГНАЛ НАЙДЕН
    sublabel: СЛАБЫЙ УЗЕЛ ОБНАРУЖЕН
  RELAY_AVAILABLE:
    label: RELAY ДОСТУПЕН
    sublabel: МОЖНО ПЕРЕДАТЬ ENVELOPE
  LONG_RANGE_LINK:
    label: ДАЛЬНЯЯ СВЯЗЬ ОТКРЫТА
    sublabel: КАНАЛ СТАБИЛЕН
  SIGNAL_RETURNED:
    label: СИГНАЛ ВЕРНУЛСЯ
    sublabel: ОТЧЁТ ГОТОВ
```

## Implementation note

Use this UI profile for the Blue Scout surface only. Purple Orb should keep its own warmer/violet companion-consciousness design language. The bridge between the two is packet resonance, not visual merging.
